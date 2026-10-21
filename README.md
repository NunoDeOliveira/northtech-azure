# NorthTech Azure

## Table of Contents

1. [Context and Motivation](#1-context-and-motivation)
2. [Requirements](#2-requirements)
3. [Architecture Design](#3-architecture-design)
4. [Cost Estimation](#4-cost-estimation)
5. [Implementation](#5-implementation)
   - [5.1 Azure Administration and Testing](#51-azure-administration-and-testing)
   - [5.2 Automated Deployment and Operations](#52-automated-deployment-and-operations)
6. [Evaluation](#6-evaluation)
7. [Resources and References](#7-resources-and-references)

---

## 1. Project Overview

Design, implementation, and validation of an Azure infrastructure for a IT services company, with a focus on governance, identity, network security, scalability, monitoring, and cost management.

This project proposes an architecture comprising a customer-facing web application hosted on Microsoft Azure, whilst retaining certain internal systems on-premises. The design also takes into account the separation of responsibilities between the development and infrastructure teams, as well as the need to control operating costs.

**Main engineering goals:**
- Organize Azure resources and permissions using governance policies, Microsoft Entra ID, and RBAC.
- Segment network traffic and protect access to application and data services.
- Support changes in application demand through appropriate compute and traffic-distribution services.
- Monitor infrastructure behavior, verify recovery measures, and evaluate resource costs.
- Make deployments reproducible with Infrastructure as Code (IaC).

> Details of [Context](docs/context.md)
> Details of [Requirements](docs/requirements.md)

---

## 2. Architecture Design

1. **Governance and Identity Architecture**
Define subscriptions, resource groups, Entra ID and RBAC.

2. **Infrastructure Architecture**
Design VNets, subnets, compute, security and Azure services.

3. **Application Architecture**
Define frontend, backend, database and application traffic flows.

> Component selection and trust boundaries are explained in the [architecture documentation](docs/architecture.md).

---


## 3. Technical Scope

| Area | Technologies / capabilities addressed |
| --- | --- |
| Cloud administration | Microsoft Azure, resource governance, Microsoft Entra ID, RBAC |
| Networking & security | VNets, subnets, NSGs, private connectivity, Azure Bastion, Application Gateway / WAF |
| Compute & data | VMSS, PostgreSQL, Azure Storage |
| Operations | Azure Monitor, Log Analytics, alerts, Network Watcher |
| Automation | Infrastructure as Code, repeatable deployment and teardown |

---


## 4. Cost Estimation

Estimate the total Azure cost of the project, including administration, testing, temporary deployments and final validation.

1. **Administration and Testing Costs.**
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

2. **Deployment and Operational Costs**
Estimate the cost of deploying and operating the complete architecture during the final validation period.



---


## 5. Validation & Results

The following checklist tracks the validation of the project requirements.
Each completed requirement must be supported by test results and evidence
available in [Testing Documentation](docs/testing.md).

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

## 7. Resources and References used

- **Dignitae.** *AZ-104T00-A Microsoft Knowledge and Skills with Challenge Labs.* Training material. 

- **Microsoft.** *Course AZ-104T00-A: Microsoft Azure Administrator.* Microsoft Learn. 
https://learn.microsoft.com/en-us/training/courses/az-104t00



*This is a personal portfolio project based on a fictional business scenario. It is not an operational NorthTech company deployment.*
