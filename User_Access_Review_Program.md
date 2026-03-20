# Audit Program: Identity & Access Management (IAM)
**Objective:** To verify that user access to core financial systems is granted based on the 'Principle of Least Privilege' and that terminated employees' access is revoked in a timely manner.

| Control Activity | Audit Objective | Testing Procedure |
| :--- | :--- | :--- |
| **New Hire Provisioning** | Ensure access is granted based on approved 'Role-Based Access Control' (RBAC). | Sample new hires from the HR system. Verify that their system permissions match their job description. |
| **Termination Revocation** | Mitigate the risk of 'Orphan Accounts' by ensuring access is removed within 24 hours of exit. | Compare the HR 'Leavers' list to Active Directory logs. Confirm account deactivation dates. |
| **Privileged Access Review** | Validate that 'Super User' access is restricted and reviewed quarterly. | Inspect the 'Global Administrator' group. Confirm that each user has a valid business justification. |
| **Segregation of Duties (SoD)** | Ensure no single user can both 'Initiate' and 'Approve' a financial transaction. | Analyze the 'Permissions Matrix' for the ERP system. Identify and report any conflicting roles. |
