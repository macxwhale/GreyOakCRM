# Email and SMS Notification Feature for Grey Oak CRM

## Overview

Adding **email** and **SMS** notification capabilities will improve communication with clients and keep internal users informed about important events (e.g., new lead assignment, status changes, upcoming appointments). The feature should be:
- Configurable per agency (enable/disable, templates, sender IDs).
- Extensible (future channels like WhatsApp, push notifications).
- Secure and GDPR‑compliant (opt‑out handling, audit logs).

## Functional Requirements

1. **Trigger Points**
   - New lead created.
   - Lead status moves to a new stage.
   - Appointment scheduled / reminder time reached.
   - Task assigned or overdue.
2. **Notification Types**
   - **Email** – rich‑HTML with merge fields (client name, lead details, links).
   - **SMS** – plain‑text limited to 160 characters, includes essential info and a short link.
3. **User Settings**
   - Global toggle for email/SMS.
   - Per‑user preferences (receive email, SMS, both, or none).
   - Template editor for admins.
4. **Delivery Guarantees**
   - Retry logic (up to 3 attempts).
   - Store delivery status (sent, delivered, failed) in an **Audit** table.
5. **Compliance**
   - Unsubscribe link in emails.
   - Opt‑out handling for SMS.
   - Log of personal data usage.

## Technical Design

### Architecture
```
[CRM Core] -> [Notification Service] -> { Email Provider, SMS Provider }
```
- **Notification Service** (Node.js/Express or Python/FastAPI) receives events via a message queue (e.g., RabbitMQ or built‑in PostgreSQL NOTIFY/LISTEN).
- Service formats payload using stored templates and dispatches to external providers.

### Data Model (SQL)
```sql
CREATE TABLE notification_templates (
    id SERIAL PRIMARY KEY,
    channel VARCHAR(10) NOT NULL,   -- 'email' or 'sms'
    name VARCHAR(50) NOT NULL,
    subject VARCHAR(150),            -- only for email
    body TEXT NOT NULL,
    is_active BOOLEAN DEFAULT TRUE,
    created_at TIMESTAMP DEFAULT NOW()
);

CREATE TABLE user_notification_preferences (
    user_id BIGINT REFERENCES users(id),
    channel VARCHAR(10),
    enabled BOOLEAN DEFAULT TRUE,
    PRIMARY KEY (user_id, channel)
);

CREATE TABLE notification_audit (
    id BIGINT PRIMARY KEY,
    event_type VARCHAR(50),
    recipient VARCHAR(255),
    channel VARCHAR(10),
    status VARCHAR(20),   -- 'queued', 'sent', 'delivered', 'failed'
    provider_message_id VARCHAR(255),
    created_at TIMESTAMP DEFAULT NOW()
);
```

### Provider Integration
- **Email** – Use a transactional service like SendGrid, Mailgun, or SES. Store API key in environment variables.
- **SMS** – Use Twilio, Vonage, or local carrier gateway. Again, keep credentials secret.

### Workflow Example (lead created)
1. Lead creation endpoint publishes `lead.created` event to the queue.
2. Notification Service consumes the event, checks user preferences, loads the **email** and **SMS** templates.
3. Renders templates with merge fields (e.g., `{{lead.name}}`).
4. Sends request to provider APIs.
5. Persists each attempt in `notification_audit`.
6. Retries on transient failures.

## Implementation Steps
1. **Create Database Tables** – Run migration scripts.
2. **Build Notification Service**
   - Set up a small micro‑service project.
   - Implement queue listener and provider wrappers.
3. **Add Preference UI** – Extend the existing settings page with toggles and a template editor (rich‑text for email, plain‑text for SMS).
4. **Define Templates** – Provide default templates for each trigger.
5. **Instrument CRM Core** – Emit events for the defined trigger points.
6. **Testing**
   - Unit tests for template rendering.
   - Integration tests with mock provider endpoints.
   - End‑to‑end manual verification (send test email/SMS).
7. **Deployment** – Deploy the service alongside the CRM backend, configure environment variables.
8. **Monitoring** – Add dashboard widgets showing recent notification counts and failure rates.

## Security & Privacy
- Store API keys in `.env` (never commit).
- Mask personal data in logs.
- Provide a compliance page summarising data‑processing agreements.

## UI/UX Mockup (Optional)
If needed, we can generate a quick design mockup showing the **Notification Settings** panel with toggle switches and a **Template Editor** modal.

---
*This document serves as a blueprint for adding robust email and SMS notification capabilities to Grey Oak CRM.*
