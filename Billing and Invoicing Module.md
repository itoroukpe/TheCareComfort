 **Product Requirement Document (PRD)** for the **Billing & Invoicing Module**, now including **Insurance Claim Workflows** as **Phase 2**:

---

### 📌 **Feature Title:** Billing & Invoicing Module (with Insurance Claim Workflow – Phase 2)

---

### 🔍 **Objective:**

Deliver a comprehensive billing system within CareComfort to streamline invoicing, enable faster payments, support insurance/Medicaid claim workflows, and integrate with third-party accounting and payment platforms like QuickBooks and Celero.

---

### 🧩 **Key Requirements (Phase 1 – Core Billing)**

#### 1. **Automated Invoice Generation**

* Auto-generate invoices based on completed and verified shifts.
* Pull in relevant data from Scheduling and EVV, including:

  * Hours worked
  * Services rendered
  * Expenses/mileage
* Generate and export as PDF

#### 2. **Advanced Filtering & Search**

* Search invoices using:

  * Invoice number
  * Client name
  * Service date range
  * Status (open, overdue, paid)

#### 3. **Editable Invoices**

* Allow authorized users to:

  * Edit invoice items
  * Add discounts
  * Attach notes
  * Update status manually if needed

#### 4. **QuickBooks & PDF Export**

* Export invoices in QuickBooks-compatible format (CSV, IIF, or API integration)
* Enable batch export of invoices
* Allow branded PDFs for professional presentation

#### 5. **1-Click Credit Card Payments (Celero)**

* Allow clients to pay directly via:

  * Secure payment link
  * Credit card input through Celero
* Auto-match payments to invoices
* Confirm and log successful transactions

#### 6. **Alerts & Notifications**

* Automated email/SMS for:

  * Invoice delivery
  * Payment due reminders
  * Overdue alerts

#### 7. **Reconciliation & Reporting**

* Dashboard for:

  * Paid vs unpaid invoices
  * Aging reports
  * Monthly revenue reports
* View payment logs and reconciliation history

---

### 🧩 **Key Requirements (Phase 2 – Insurance Claim Workflow)**

#### 1. **Claim Data Capture**

* Collect Medicaid/insurance-required fields during:

  * Shift documentation
  * Invoice creation
* Fields include:

  * Client Medicaid ID
  * Provider NPI number
  * HCPCS service codes
  * Modifiers and units of service
  * Diagnosis codes (ICD-10)

#### 2. **Claim Form Generation**

* Auto-fill claim forms (CMS-1500 or UB-04)
* Export claim data in:

  * PDF (manual submission)
  * X12 EDI 837 format (for clearinghouse submission)

#### 3. **Claim Submission Integration (Optional)**

* Integrate with clearinghouses (e.g., Office Ally, Availity)
* Allow real-time submission and status tracking of claims

#### 4. **Claim Tracking**

* Track claim status: submitted, accepted, rejected, denied, paid
* Log denial codes and explanations
* Enable claim corrections and resubmissions

#### 5. **Reimbursement Reconciliation**

* Match payments from Medicaid/insurers with claims
* Auto-update claim and invoice status
* Allow manual override and notes for reconciliation exceptions

#### 6. **Reporting & Audits**

* Generate reports on:

  * Claims by status
  * Revenue by payer
  * Denial reasons
* Provide downloadable audit logs for compliance reviews

---

### 🛠️ **Backend Considerations**

* Strong data validation for claim submission compliance
* Role-based access to billing and claims data
* Integration-ready architecture for accounting and clearinghouse APIs
* Secure storage of PHI and financial data (HIPAA & PCI compliance)

---

### 🔐 **Permissions & Roles**

* **Billing Admins**: Full access to invoices and claims
* **Care Managers**: View client billing summary
* **Clients**: View/pay invoices (no access to insurance data)

---

### ✅ **Acceptance Criteria**

* Users can generate invoices and receive payments via Celero
* Invoices are searchable, editable, and exportable
* Insurance claims can be auto-generated, tracked, and submitted
* Status of claims is updated in real time
* Reimbursement records match claims/invoice entries accurately

---





