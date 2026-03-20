# ITGC: Change Management Audit Program
**Objective:** To ensure that all changes to the production environment are authorized, tested, and approved to mitigate the risk of system instability or unauthorized code execution.

| Control Activity | Audit Objective | Testing Procedure (Methodology) |
| :--- | :--- | :--- |
| **Request & Authorization** | Ensure all changes are initiated via a formal ticketing system. | Select a sample of changes. Verify a corresponding 'Service Desk' or 'Jira' ticket exists for each. |
| **Segregation of Duties (SoD)** | Prevent the person who wrote the code from moving it to production. | Inspect 'Commit' and 'Merge' logs. Verify that the 'Developer' and 'Deployer' are unique individuals. |
| **UAT (User Acceptance)** | Confirm that business owners have validated the change. | Review 'User Acceptance Testing' (UAT) sign-off documentation for the sampled changes. |
| **Rollback Planning** | Ensure a 'Plan B' exists if the change causes a system failure. | Verify that a documented 'Backout Plan' was included in the Change Request prior to approval. |
| **CAB Approval** | Validate that the Change Advisory Board (CAB) reviewed high-risk items. | Review CAB meeting minutes. Confirm approval was granted before the production deployment date. |
