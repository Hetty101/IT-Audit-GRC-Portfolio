# Audit Program: Odoo ERP Application Controls
**Objective:** To evaluate the configuration of Odoo modules (Accounting, Inventory, Sales) to ensure data integrity and prevent unauthorized financial transactions.

| Control Area | Audit Objective | Testing Procedure (Odoo Specific) |
| :--- | :--- | :--- |
| **Automated Workflows** | Ensure 'Purchase Orders' over $5,000 require multi-level approval. | Review **Settings > Purchase**. Validate 'Purchase Order Approval' threshold and authorized 'Approver' groups. |
| **Journal Entry Integrity** | Prevent back-dating of financial transactions in closed periods. | Inspect **Accounting > Configuration > Settings**. Verify 'Lock Dates' are set for non-advisers to prevent prior-period edits. |
| **Inventory Valuation** | Ensure the 'Automated Inventory Valuation' matches the General Ledger. | Validate 'Product Category' settings. Confirm 'Inventory Valuation' is set to 'Automated' and 'Costing Method' is AVCO/FIFO as per policy. |
| **Access Rights (SoD)** | Ensure a 'Sales User' cannot also validate their own 'Invoices'. | Analyze **Settings > Users & Companies**. Compare 'Sales' group permissions against 'Accounting' validation rights. |
| **Bank Account Security** | Mitigate risk of fraudulent redirection of outbound payments. | Verify 'Two-Factor Authentication' is mandatory for users with 'Bank' edit permissions in the Accounting module. |
