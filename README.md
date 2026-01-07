# GRC-Implementation-Portfolio
ServiceNow GRC &amp; ISO 27001 Automation Projects
graph TD
    A[ISO 27001 Requirement] --> B[Control Objective: A.12.6.1]
    B --> C[Entity Type: Critical Servers]
    C --> D[Generated Control: SRV-001]
    D --> E{Scripted Indicator}
    E -->|Queries CMDB/Vuln Table| F[Evidence Collection]
    F -->|Record Found| G[Compliant - Auto-Close Audit Task]
    F -->|No Record| H[Non-Compliant - Trigger Issue/Remediation]
