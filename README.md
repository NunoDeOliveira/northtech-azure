# NorthTech Azure

## 1. Structure of project

northtech-azure
.
├── docs
│   ├── architecture.md
│   ├── context.md
│   ├── implementation.md
│   ├── infra-requirements.md
│   └── web-portal-requirements.md
├── infra
├── monitoring
├── README.md
├── screenshot 
└── web-app

---


## 2. Project Overview

**Context**
Design, implementation, and validation of an Azure infrastructure for a IT services company, with a focus on governance, identity, network security, scalability, monitoring, and cost management.

This project proposes an architecture comprising a customer-facing web application hosted on Microsoft Azure, whilst retaining certain internal systems on-premises. The design also takes into account the separation of responsibilities between the development and infrastructure teams, as well as the need to control operating costs.

**Main goals:**
- Organize Azure resources and permissions using governance policies, Microsoft Entra ID, and RBAC.
- Segment network traffic and protect access to application and data services.
- Support changes in application demand through appropriate compute and traffic-distribution services.
- Monitor infrastructure behavior, verify recovery measures, and evaluate resource costs.
- Make deployments reproducible with Infrastructure as Code (IaC).

> Details of [Context](docs/context.md)<br>
> Details of [Requirements](docs/requirements.md)

---


## 3. Architecture Design

1. **Web Portal design**<br>
Define frontend, backend, database and application traffic flows.

![Web Portal design](docs/diagrams/applicationWeb.png)


2. **Infrastructure design**<br>
Design VNets, subnets, compute, security and Azure services.

![Infrastructure design](docs/diagrams/infrastructure.png)


3. **Governance and Identity diagram**<br>
Define subscriptions, resource groups, Entra ID and RBAC.

![Governance diagram](docs/diagrams/infrastructure.png)


> Component selection of components is explained in the [architecture documentation](docs/architecture.md).

---


## 4. Technical Scope

| Area | Technologies / capabilities addressed |
| --- | --- |
| Cloud administration | Microsoft Azure, resource governance, Microsoft Entra ID, RBAC |
| Networking & security | VNets, subnets, NSGs, private connectivity, Azure Bastion, Application Gateway / WAF |
| Compute & data | VMSS, PostgreSQL, Azure Storage |
| Operations | Azure Monitor, Log Analytics, alerts, Network Watcher |
| Automation | Infrastructure as Code, repeatable deployment and teardown |

---


## 5. Cost Estimation

1. **Administration and Testing Costs.**<br>
Estimate the cost generated while configuring, testing and validating Azure resources before the final deployment.

| Azure Service | Estimated Cost (€/hour) | Hours | Total Cost (€) |
|---|---:|---:|---:|
| Virtual Machines | 0,08 € | 20 | 1,60 € |
| Azure Database for PostgreSQL | 0,04 € | 12 | 0,48 € |
| Azure Storage | 0,01 € | 40 | 0,40 € |
| VPN Gateway | 0,22 € | 6 | 1,32 € |
| Application Gateway | 0,30 € | 6 | 1,80 € |
| Azure Monitor | 0,03 € | 20 | 0,60 € |
| **TOTAL** | | | **6,20 €** |

2. **Deployment and Operational Costs**<br>
Estimate the cost of deploying and operating the complete architecture during the final validation period.

| Azure Service | Estimated Cost (€/hour) | Hours | Total Cost (€) |
|---|---:|---:|---:|
| Azure Monitor | 0,03 € | 20 | 0,60 € |

---


## 6. Quick start



---


## 7. Validation and Results

The following checklist follow the requirements.

**Governance and Identity Management**

- [ ] Verify resource groups, naming conventions, tags, and Azure Policy compliance.
- [ ] Verify Microsoft Entra ID identities and RBAC permissions.
- [ ] Verify protection against accidental deletion and unauthorized modifications.

**Networking and Security**

- [ ] Verify site-to-site VPN connectivity between Bilbao, Madrid, and Azure.
- [ ] Verify network isolation and NSG filtering between application, database, and management networks.
- [ ] Verify that administrative access is restricted to authorized users.
- [ ] Verify that sensitive services are not directly accessible from the public Internet.
- [ ] Verify that incoming traffic is distributed across healthy backend instances.

**Compute and Storage**

- [ ] Verify application availability during the failure of an individual compute instance.
- [ ] Verify automatic scaling under increasing and decreasing workloads.
- [ ] Verify storage redundancy, encryption, and backup configurations.
- [ ] Verify secure communication between frontend, backend, and database components.

**Monitoring and Operations**

- [ ] Verify collection of infrastructure, application, and network metrics.
- [ ] Verify alerts triggered by predefined operational or security conditions.
- [ ] Verify the availability of diagnostic logs and tools to investigate failures.
- [ ] Verify service or data recovery after a controlled failure.

**Automation and Cost Management**

- [ ] Verify infrastructure deployment using version-controlled IaC templates.
- [ ] Verify automated creation, configuration, and removal of Azure resources.
- [ ] Compare estimated costs with actual Azure expenditure.
- [ ] Verify that unnecessary resources are removed and consumption is minimized.

---


## 8. Resources used
- Dignitae. *AZ-104T00-A Microsoft Knowledge and Skills with Challenge Labs.* Training material. 
- Microsoft. *Course AZ-104T00-A: Microsoft Azure Administrator.* Microsoft Learn.<br> 
https://learn.microsoft.com/en-us/training/courses/az-104t00
- Microsoft. *Azure Pricing Calculator.* Microsoft Azure.<br> 
https://azure.microsoft.com/en-us/pricing/calculator/
- Microsoft. *Azure for Network Engineers.* Microsoft Learn.<br> 
https://learn.microsoft.com/en-us/azure/networking/azure-for-network-engineers?toc=/azure/networking/toc.json
- Microsoft. *Azure Networking Documentation.* Microsoft Learn.<br> 
https://learn.microsoft.com/en-us/azure/networking/
- Microsoft. *Azure Bastion Documentation.* Microsoft Learn.<br> 
https://learn.microsoft.com/en-us/azure/bastion/


*This is a personal portfolio project based on a fictional business scenario. It is not an operational NorthTech company deployment.*
