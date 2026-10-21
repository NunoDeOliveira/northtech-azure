## Requirements asociated to the project

The following define the expected capabilities of the infrasctructure and web application:

1. Governance and Identity Management
- R01 — Resource Governance: Organize Azure resources using resource groups, naming conventions, tags, and Azure Policies.
- R02 — Identity and Access Management: Manage identities using Microsoft Entra ID and enforce role-based access control (RBAC).
- R03 — Resource Protection: Protect critical resources against accidental deletion or unauthorized modifications.
2. Networking and Security
- R04 — Hybrid Connectivity: Establish secure site-to-site VPN connections between Bilbao, Madrid, and Microsoft Azure.
- R05 — Network Segmentation: Separate application, database, and management networks using VNets, subnets, and NSGs.
- R06 — Secure Administration: Restrict administrative access to authorized users through secure management channels.
- R07 — Private Connectivity: Ensure sensitive services, including databases, are not directly accessible from the public Internet.
- R08 — Traffic Distribution: Distribute incoming application traffic across healthy backend instances.
3. Compute and Storage
- R09 — High Availability: Maintain application availability during the failure of an individual compute instance.
- R10 — Automatic Scaling: Automatically adjust compute capacity according to predefined workload thresholds.
- R11 — Data Protection: Configure appropriate storage redundancy, encryption, and backup mechanisms.
- R12 — Application Integration: Ensure secure communication between frontend, backend, and database components.
4. Monitoring and Operations
- R13 — Infrastructure Monitoring: Collect and analyze infrastructure, application, and network metrics.
- R14 — Incident Detection: Generate alerts when predefined operational or security thresholds are exceeded.
- R15 — Troubleshooting: Provide sufficient logs and diagnostic information to investigate connectivity and application failures.
- R16 — Recovery: Restore application services or data following a controlled failure scenario.
5. Automation and Cost Management
- R17 — Infrastructure as Code: Deploy Azure infrastructure using reusable and version-controlled IaC templates.
- R18 — Automated Deployment: Validate the automated creation, configuration, and removal of cloud resources.
- R19 — Cost Management: Monitor resource consumption and compare estimated costs against actual expenditure.
- R20 — Cost Optimization: Minimize unnecessary resource consumption during implementation, testing, and validation.-
