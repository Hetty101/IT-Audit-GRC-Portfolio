| Control Domain | Audit Objective (Control Goal) | Testing Procedure (Methodology) |
| :--- | :--- | :--- |
| **Identity & Access** | Validate MFA enforcement for privileged accounts to mitigate unauthorized access risk. | Review **Microsoft Entra ID** Conditional Access policies. Confirm MFA is mandatory for all Administrative roles. |
| **Data Security** | Confirm encryption-at-rest for cloud storage to ensure data confidentiality and compliance. | Inspect **Storage Account** encryption settings. Verify use of Microsoft-managed or Customer-managed keys. |
| **Network Security** | Identify and remediate open management ports (RDP/SSH) to reduce the external attack surface. | Analyze **Network Security Groups (NSG)** inbound rules. Ensure Ports 3389 and 22 are restricted from 'Any' source. |
| **Governance** | Verify resource tagging enforcement to ensure auditability and cost center accountability. | Evaluate **Azure Policy** assignments. Confirm 'Enforce Tagging' is active across the production environment. |
| **Monitoring** | Ensure high-severity security events are captured and alerted for timely incident response. | Validate **Azure Monitor** alert configurations for critical activities (e.g., Security Policy deletions). |
