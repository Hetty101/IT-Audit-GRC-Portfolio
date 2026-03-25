# Case Study: ERP Application Controls & Governance Review

| Control Area | Audit Objective | Technical Testing Procedure |
| :--- | :--- | :--- |
| **Delegation of Authority** | Ensure expenditures >$5,000 require multi-level approval. | **Configuration Review:** Validated hard-coded thresholds mapped to authorized 'Approver' security groups. |
| **Financial Integrity** | Prevent fraudulent back-dating of transactions in closed periods. | **Change Management:** Verified 'Lock Date' settings; restricted prior-period edits to 'Super-User' roles. |
| **Inventory Valuation** | Ensure sub-ledger reconciles with the GL (AVCO/FIFO). | **Substantive Testing:** Validated automated valuation logic against corporate accounting policy and GAAP. |
| **Segregation of Duties** | Prevent 'Sales' users from validating their own invoices. | **Access Matrix:** Compared 'Sales' group permissions against 'Accounting' validation rights to ensure SoD. |
| **Disbursement Security** | Protect against unauthorized bank master data changes. | **Security Audit:** Verified mandatory MFA and 'Dual-Control' for users with 'Bank' edit permissions. |
