# NorthTech Azure

## Table of Contents

1. [Project Context](#1-project-context)
2. [Requirements](#2-requirements)
3. [Architecture Design](#3-architecture-design)
4. [Cost Estimation](#4-cost-estimation)
5. [Implementation](#5-implementation)
   - [5.1 Azure Administration and Testing](#51-azure-administration-and-testing)
   - [5.2 Automated Deployment and Operations](#52-automated-deployment-and-operations)
6. [Evaluation](#6-evaluation)
7. [Resources and References](#7-resources-and-references)

---

## 1. Project Context

Describe NorthTech's scenario, current infrastructure, problem and project objectives.

---

## 2. Requirements

Define functional, technical, security and availability requirements.

---

## 3. Architecture Design

1. **Governance and Identity Architecture**
Define subscriptions, resource groups, Entra ID and RBAC.

2. **Infrastructure Architecture**
Design VNets, subnets, compute, security and Azure services.

3. **Application Architecture**
Define frontend, backend, database and application traffic flows.

---

## 4. Cost Estimation

Estimate the total Azure cost of the project, including administration, testing, temporary deployments and final validation.

1. **Administration and Testing Costs.**
Estimate the cost generated while configuring, testing and validating Azure resources before the final deployment.

2. **Deployment and Operational Costs**
Estimate the cost of deploying and operating the complete architecture during the final validation period.

---

## 5. Implementation

### 5.1 Azure Administration and Testing

1. **Governance and Identity Configuration**
Configure Entra ID, RBAC, policies, tags and locks.

2. **Network and Compute Deployment**
Deploy VNets, peering, NSGs, Bastion, Application Gateway and VMSS.

3. **Data Services Configuration**
Configure PostgreSQL, Storage and private connectivity.

4. **Web Application Deployment and Integration**
Deploy and connect frontend, backend and database.

5. **Monitoring and Observability Configuration**
Configure Monitor, Log Analytics, alerts and Network Watcher.

### 5.2 Automated Deployment and Operations

1. **Infrastructure as Code**
Create reusable infrastructure deployment templates.

2. **Infrastructure Deployment Testing**
Validate automated creation and removal of resources.

3. **Application Deployment**
Automate application deployment.

4. **Post-Deployment Validation**
Verify the complete environment after deployment.

---

## 6. Evaluation

- **Networking**
Validate connectivity, routing and network isolation.
- **Security**
Verify access controls and exposed services.
- **Scalability**
Test VMSS autoscaling under generated workload.
- **Cost Evaluation**
Compare estimated and actual Azure costs using deployment start and end times.

---

## 7. Resources and References

List Microsoft documentation


