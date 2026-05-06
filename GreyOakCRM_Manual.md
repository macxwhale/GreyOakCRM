# Grey Oak Real Estate Management System (CRM) - Ultimate User Manual

## Table of Contents
1.  [Introduction](#1-introduction)
2.  [Getting Started & Navigation](#2-getting-started--navigation)
3.  [How to Create a Client](#3-how-to-create-a-client)
4.  [Lead Management Pipeline](#4-lead-management-pipeline)
5.  [The Sale Journey (Step-by-Step)](#5-the-sale-journey-step-by-step)
6.  [Financial Management (Account Module)](#6-financial-management-account-module)
7.  [Property & Inventory Control (Projects Module)](#7-property--inventory-control-projects-module)
8.  [Document & Title Deed Tracking](#8-document--title-deed-tracking)
9.  [Reporting & Analytics](#9-reporting--analytics)
10. [User Management (Staff Access)](#10-user-management-staff-access)
11. [Master Setup (Configuration)](#11-master-setup-configuration)
12. [Troubleshooting & Support](#12-troubleshooting--support)

---

## 1. Introduction
The **Grey Oak Real Estate Management System** is an all-in-one ERP/CRM solution designed to automate the complexities of land investment. This guide covers every feature, from the first contact in **Nanyuki** to the final Title Deed issuance in the **Nairobi CBD** office.

---

## 2. Getting Started & Navigation

### 2.1 Access & Security
*   **Portal URL:** `https://greyoakcrm.co.ke/admin/login`
*   **Authentication:** Use your corporate email and the provided password.
*   **Logout:** Click the profile icon in the top right corner of the header.

### 2.2 Navigation Menu (Sidebar)
The left sidebar is your primary navigation tool. The modules are:
1.  **Dashboard**: Business overview and summary statistics.
2.  **Clients**: Central database for all property buyers.
3.  **Leads**: Tracking for potential prospects.
4.  **Projects**: Management of land projects (e.g., *Arista Eminence 96*).
5.  **User Management**: Staff accounts and access control.
6.  **Account**: Financial modules (**Payments**, **Expenses**).
7.  **Reports**: Detailed business analytics and lead status reports.
8.  **Master**: Configuration settings (Currencies, Lead Sources, Property Sizes, etc.).

---

## 3. How to Create a Client

In the Grey Oak CRM, all buyers are managed under the **Clients** module. As the core dependency for all transactions, a client record must be created before any project, property, or payment can be linked.

### 3.1 Adding a Client Manually
1.  Navigate to **Clients** in the left sidebar.
2.  Click the green **+ Add Client** button located above the client list table.
3.  Complete the **Add Client Form** with the following details:
    *   **First Name** & **Last Name** (Required)
    *   **Nationality**
    *   **ID Number / PP Number**: Essential for legal documentation.
    *   **Gender**
    *   **Projects**: Link the client to a specific project (e.g., *Arista Eminence 96*).
    *   **Property**: Specify the plot/unit if known.
    *   **Assigned To**: Select the staff member responsible for this client (Required).
    *   **Email**: Primary communication address (Required).
    *   **Contact Number**: Primary mobile number (Required).
    *   **Address Details**: City, County, and Post Code.
4.  Click the **Add Client** button at the bottom of the form to save.

### 3.2 Converting a Lead to a Client
If the prospect is already in the system as a Lead:
1.  Go to **Leads** in the sidebar.
2.  Locate the prospect in the list and click their name.
3.  Click the **Convert to Customer** button (top right of the lead profile).
4.  Verify the pre-filled information and save.
    *   *Note: Converting a lead ensures all historical notes and site visit logs are preserved.*

### 3.3 Adding Multiple Contacts to a Client
For joint purchases (e.g., a couple or partners):
1.  Open the **Client Profile** from the list.
2.  Go to the **Contacts** tab.
3.  Click **New Contact** to add secondary buyer details.

---

## 4. Lead Management Pipeline
Leads are potential prospects still in the inquiry stage.

### 4.1 Capturing a New Lead
1.  Navigate to **Leads** in the sidebar.
2.  Click the **+ Add Lead** button.
3.  Fill in the inquiry source and contact details.
4.  **Status Tracking**: Update the lead status as they progress from *New* to *Site Visit Scheduled* to *Interested*.

---

## 5. The Sale Journey (Step-by-Step)

### Step 1: Reserving a Property
1.  Navigate to **Projects** in the sidebar.
2.  Select the specific project (e.g., *Arista Eminence 96*).
3.  Identify the **Property Number** and verify the **LR Number**.
4.  Change the **Property Status** to **Reserved** once the client confirms their choice.

### Step 2: Client Documentation
(See [Section 3: How to Create a Client](#3-how-to-create-a-client)). Ensure the client record is linked to the correct project and property.

### Step 3: Recording Payments & Installments
Navigate to **Account > Payments** to set up the billing plan.

---

## 6. Financial Management (Account Module)

The **Account** module is where all revenue and project-related costs are tracked.

### 6.1 Recording Payments
1.  Navigate to **Account > Payments**.
2.  Click the green **+ Add Payment** button.
3.  **Client & Property**: Select the Client, Project, and Property from the dropdowns.
4.  **Commission**: Assign the Sales Agent and their commission percentage.
5.  **Payment Schedule**: 
    *   Add rows for each installment.
    *   Enter **Expected Date** and **Expected Amount**.
    *   As the client pays, enter the **Actual Date** and **Actual Amount**.
6.  Click **Add Payment**.

### 6.2 Managing Expenses
Track operational and project-specific costs.
1.  Navigate to **Account > Expenses**.
2.  Click the **+ Add Expense** button.
3.  **Fields**: Title, Amount (KES), Date, and Payment Method.
4.  **Linking**: Link the expense to a specific **Sales Agent**, **Client**, and **Project** to track total project profitability.

---

## 7. Property & Inventory Control (Projects Module)

### 7.1 Adding a New Project
1.  Navigate to **Projects**.
2.  Click the **+ Add Project** button.
3.  **Project Details**: Name, Image (Marketing flyer), and Address.
4.  **Properties Sub-form**: Add individual plots/units by LR Number and Property Number. Specify Area (Acre/Sq Ft) and Price (KES/USD).

---

## 8. Document & Title Deed Tracking
Ensure all "Sold" properties have their corresponding legal documents uploaded in the **Client Files**:
- **ID/Passport Copy**
- **KRA PIN Certificate**
- **Signed Sale Agreement**
- **Title Deed Scan** (once processing is complete).

---

## 9. Reporting & Analytics

The **Reports** module provides real-time insights into your business.

### 9.1 Available Reports
*   **Sales Lead Report**: Track the status of every inquiry.
*   **Payment Status Report**: Identify clients with pending balances.
*   **Agent Performance Report**: Monitor sales targets and closures by staff.
*   **Expense Report**: Summary of all costs incurred.
*   **Customer Detail Report**: Full database of client contact information.

---

## 10. User Management (Staff Access)

### 10.1 Adding a New User
1.  Navigate to **User Management**.
2.  Click the **+ Add User** button.
3.  **Details**: Username, User Role, First/Last Name, Email, and Contact Number.
4.  **Security**: Set a temporary password and ensure the status is **Active**.

---

## 11. Master Setup (Configuration)

The **Master** module allows Administrators to configure the system backbone.

### 11.1 Setup Categories
*   **Currencies**: Define KES/USD rates.
*   **Property Sizes**: Define units (Acre, Sq Ft).
*   **Lead Sources**: Track where leads come from (Facebook, Referrals).
*   **Payment Methods**: M-Pesa, Bank Transfer, etc.
*   **Roles & Permissions**: Manage what different staff roles can see and do.

---

## 12. Troubleshooting & Support

| Symptom | Cause | Solution |
| :--- | :--- | :--- |
| **Plot Not Available** | Already Reserved | Check the status in the Projects module. |
| **Balance Inconsistency** | Payment not linked | Ensure actual payments are recorded in the Payment Schedule. |
| **Email Not Sent** | SMTP Error | Check the system settings or contact IT. |

### Support Contact
*   **Email**: info@greyoak.co.ke
*   **Physical Office**: Trust Mansion, Tubman Road, Nairobi CBD.

---

*Manual Version: 5.0 | Complete Verified Edition | © 2026 Grey Oak Limited*
