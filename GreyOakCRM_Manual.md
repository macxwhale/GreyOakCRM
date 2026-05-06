# Grey Oak Real Estate Management System (CRM) - Ultimate User Manual

## Table of Contents
1.  [Introduction](#1-introduction)
2.  [Getting Started](#2-getting-started)
3.  [Lead Management Pipeline](#3-lead-management-pipeline)
4.  [How to Create a Client (Customer)](#4-how-to-create-a-client-customer)
5.  [The Sale Journey (Step-by-Step)](#5-the-sale-journey-step-by-step)
6.  [Financial Management](#6-financial-management)
7.  [Property & Inventory Control](#7-property--inventory-control)
8.  [Document & Title Deed Tracking](#8-document--title-deed-tracking)
9.  [Reporting & Analytics](#9-reporting--analytics)
10. [Expense Tracking (Project Costs)](#10-expense-tracking-project-costs)
11. [Staff Performance & Tasks](#11-staff-performance--tasks)
12. [Communication Templates (Email/SMS)](#12-communication-templates-emailsms)
13. [Contract & Document Automation](#13-contract--document-automation)
14. [User Roles & Permissions](#14-user-roles--permissions)
15. [System Settings & Customization](#15-system-settings--customization)
16. [Troubleshooting & Support](#16-troubleshooting--support)

---

## 1. Introduction
The **Grey Oak Real Estate Management System** is an all-in-one ERP/CRM solution designed to automate the complexities of land investment. This guide covers every feature, from the first contact in **Nanyuki** to the final Title Deed issuance in the **Nairobi CBD** office.

---

## 2. Getting Started

### 2.1 Access & Security
*   **Portal URL:** `https://greyoakcrm.co.ke/admin/login`
*   **Credentials:** Managed by the IT Administrator. Ensure your password contains symbols and numbers for security.
*   **Session Timeout:** For security, sessions expire after 2 hours of inactivity.

> [!IMPORTANT]
> **Data Privacy:** All customer data must be handled in compliance with the Data Protection Act of Kenya.

---

## 3. Lead Management Pipeline

### 3.1 Capturing Leads
Leads can be entered manually or synced via Web-to-Lead forms.
1.  Navigate to `Leads > New Lead`.
2.  **Required Fields:** Name, Phone, Source, and Assigned Staff.
3.  **Pro Tip:** Always tag the specific project the lead is interested in (e.g., *#NaivashaBreeze*).

### 3.2 Kanban vs. List View
*   **Kanban:** Best for visual tracking of sales progress.
*   **List:** Best for bulk actions like sending mass emails or SMS updates about site visits.

---

## 4. How to Create a Client (Customer)

In the Grey Oak CRM, "Clients" are referred to as **Customers**. There are two primary ways to add a new customer to the system.

### 4.1 Method A: Converting a Lead (Recommended)
This method is used when a prospect has already been tracked in the system and is now ready to make a purchase.
1.  Go to `Leads` and select the specific prospect.
2.  In the top right corner, click the **"Convert to Customer"** button.
3.  A form will appear pre-filled with the lead's information.
4.  **Review the details**: Ensure the Phone Number and Email are correct.
5.  Click **Save**.
    *   *Note: All previous notes, tasks, and site visit history will automatically transfer to the new Customer profile.*

### 4.2 Method B: Manual Creation
Use this method if the buyer is a walk-in or referral who is purchasing immediately without a prior lead history.
1.  Navigate to `Customers > New Customer`.
2.  **Company/Name Field**: Enter the Full Name of the individual (or company name if applicable).
3.  **VAT Number/KRA PIN**: Enter the client's KRA PIN for tax compliance.
4.  **Contact Information**:
    *   **Phone Number**: Crucial for SMS updates.
    *   **Email Address**: Crucial for automated invoicing.
5.  **Billing & Shipping**: Enter the client's physical or postal address.
6.  **Groups**: Assign the client to a group like *"Platinum Buyer"* or *"Nanyuki Phase 2 Clients"* for better filtering.
7.  Click **Save**.

### 4.3 Adding Multiple Contacts
If a plot is being bought by two people (e.g., a couple), you can add additional contacts under the same Customer profile:
1.  Open the **Customer Profile**.
2.  Go to the **Contacts** tab.
3.  Click **New Contact**.
4.  Enter the second person's details. You can choose who receives the email notifications for invoices.

---

## 5. The Sale Journey (Step-by-Step)

### Step 1: Reserving a Plot
1.  Go to **Property/Plots**.
2.  Search by Location/Phase.
3.  Select an **Available** plot and click **Reserve**.
4.  **Time Limit:** Reservations typically expire in 48-72 hours if no deposit is recorded.

### Step 2: KYC & Document Uploads
Navigate to the **Customer > Files** tab to upload:
*   ID/Passport Copy
*   KRA PIN Certificate
*   Payment Slips (Initial Deposit)
*   Signed Letter of Offer / Sale Agreement

### Step 3: Billing
1.  `Sales > Invoices > Create`.
2.  Add the plot as a "Line Item".
3.  Apply any **Early Bird Discounts** or **Cash Bonuses**.
4.  Send to the customer directly via the **"Email PDF"** button.

---

## 5. Financial Management

### 5.1 Recording Payments
All payments (M-Pesa, Bank, Cheque) must be logged here to reflect in the customer's balance.
*   Link each payment to a specific **Invoice Number**.
*   **Partial Payments:** The system handles these automatically, updating the "Balance Due" in real-time.

### 5.2 Credit Notes & Refunds
In case of a plot swap or cancellation:
1.  Go to `Sales > Credit Notes`.
2.  Issue a note to balance the customer's ledger.

---

## 6. Property & Inventory Control
Manage plots across **Diani, Kisumu, Athi River, and Nanyuki**.
*   **Plots Map:** (If integrated) View a visual site plan showing sold vs. available plots.
*   **Pricing Engine:** Update per-acre or per-plot prices based on current market valuations.

---

## 7. Document & Title Deed Tracking
The system tracks the **30-day processing commitment**.
*   **Status Indicators:** `Pending Docs` -> `In Progress` -> `At Registry` -> `Ready` -> `Collected`.
*   **Registry Details:** Log the Title Number and LR Number for easy searching.

---

## 8. Reporting & Analytics
*   **Sales Report:** View revenue by month, staff member, or project.
*   **Lead Conversion Rate:** See which staff are most effective at closing deals.
*   **Aging Report:** Identify customers who are behind on their installment plans.

---

## 9. Expense Tracking (Project Costs)
Track the costs of developing your land projects.
1.  Navigate to `Expenses > Record Expense`.
2.  **Categories:** Surveyor Fees, Fencing, Title Processing Fees, Marketing, Site Visit Transport.
3.  **Profitability:** Compare Project Revenue vs. Project Expenses.

---

## 10. Staff Performance & Tasks
*   **Tasks:** Assign follow-ups or document collection to specific staff.
*   **Reminders:** Set browser or email notifications for upcoming site visits.
*   **Goals:** Track individual sales targets vs. actual closures.

---

## 11. Communication Templates (Email/SMS)
Save time by using pre-approved templates:
*   **Welcome Message:** Sent when a new lead is captured.
*   **Payment Acknowledgment:** Automated thank-you note when a payment is logged.
*   **Site Visit Reminder:** Sent 24 hours before a scheduled viewing.
*   **Title Ready Alert:** Notification to the client that their deed is ready for collection.

---

## 12. Contract & Document Automation
Generate professional documents in seconds.
*   **Letter of Offer:** Auto-fills customer name, plot number, and price.
*   **Sale Agreement:** Generates the legal contract based on the agreed terms.
*   **Receipts:** High-resolution PDFs with the Grey Oak logo and watermark.

---

## 13. User Roles & Permissions
*   **Super Admin:** Full system control.
*   **Sales Manager:** Approves discounts and views all staff leads.
*   **Sales Agent:** Manages own pipeline only.
*   **Accountant:** Financial data entry and reporting only.
*   **Legal:** Access to Title Deed and KYC modules only.

---

## 14. System Settings & Customization
(Admin Only)
*   **Project Locations:** Add new phases (e.g., *Nanyuki Phase 5*).
*   **Custom Fields:** Add fields like "Next of Kin" or "Preferred Site Visit Day".
*   **Email Branding:** Update the logo and footer on system-generated emails.

---

## 15. Troubleshooting & Support

| Symptom | Cause | Solution |
| :--- | :--- | :--- |
| **Login Loop** | Cache/Cookie issue | Clear browser cache or use Incognito mode. |
| **PDF Not Generating** | Pop-up blocker | Allow pop-ups from `greyoakcrm.co.ke`. |
| **SMS Not Received** | Low Credit / Wrong Format | Ensure phone numbers start with `254...`. |

### Contact Support
*   **Helpdesk:** info@greyoak.co.ke
*   **Head Office:** Trust Mansion, Tubman Road, Nairobi.

---

*Manual Version: 4.0 | Ultimate Edition | © 2026 Grey Oak Limited*
