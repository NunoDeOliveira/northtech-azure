## Infrastructure requirements asociated


### The following define the expected requirements of the infrasctructure:

**1. Governance and Identity Management**
R01 - Organize Azure resources using management groups, subscriptions, resource groups, naming conventions, tags, and Azure Policy.
R02 - Manage employee identities with Microsoft Entra ID and control permissions using RBAC.
R03 - Protect critical resources against accidental deletion and unauthorized changes.
**2. Networking and Security**
R04 - Establish secure Site-to-Site VPN connections between Bilbao, Madrid, and Azure.
R05 - Separate application, data, and management traffic using network segmentation.
R06 - Restrict administrative access to authorized users through secure connections.
R07 - Protect sensitive services from direct public Internet access.
R08 - Distribute application traffic across healthy instances.
**3. Compute and Storage**
R09 - Maintain application availability if an individual compute instance fails.
R10 - Automatically adjust compute capacity based on application demand.
R11 - Protect stored data using redundancy, encryption, and backups.
R12 - Ensure secure communication between frontend, backend, and data services.
**4. Monitoring and Operations**
R13 - Collect and analyze application, infrastructure, and network metrics.
R14 - Generate alerts for defined operational and security conditions.
R15 - Provide logs and diagnostic tools to investigate failures.
R16 - Restore services and data according to defined recovery objectives.
**5. Automation and Cost Management**
R17 - Deploy Azure resources using reusable and version-controlled IaC templates.
R18 - Automate infrastructure deployment, validation, and safe removal.
R19 - Estimate infrastructure costs and compare them with actual Azure expenditure.
R20 - Minimize unnecessary resource consumption during development and testing. 

---

[← Back to README](../README.md)

## Resouces

- Microsoft. *Azure Well-Architected Framework.* Microsoft Learn.<br>
https://learn.microsoft.com/en-us/azure/well-architected/

- Microsoft. *Course AZ-104T00-A: Microsoft Azure Administrator.* Microsoft Learn.<br> 
https://learn.microsoft.com/en-us/training/courses/az-104t00
