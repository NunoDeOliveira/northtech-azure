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

## 1. Context and Motivation

### 1.1 Context

NorthTech Operations is a company that offer IT services another companies. Currently, maintains an on-premise web portal where witch customers can access the service catalogue, make enquiries and access a private customer area. The platform manages information that requires protection against unauthorized access and data loss.

As the company adds new customers, the application load increases and traffic peaks occur during marketing campaigns, which may afffect service performance. 

On the other hand, the platform is managed by different teams. For example, the development team handles the code and its deployments, while the administrators manage the infrastructure.

Given this scenario, Northtech decides to migrate its application to Microsoft Azure, while keeping part of its infrastructure and internal systems on-premise. The new solution must keep the platform costs under control.



### 1.2 Challenges

In order to build this solution, NorthTech must address several challenges.

- How can NorthTech structure its resources hierarchically, apply rules to them, and keep costs within the defined budget?

- How can NorthTech manage its employees identities and control who can access different Azure resources and what actions they are allowed to perform?

- How can NorthTech design a network topology segmented by trust level, restrict access to sensitive resources, and distribute incoming traffic efficiently and resiliently?

- How can NorthTech define a data storage strategy that ensures redundancy and confidentiality while optimizing costs?

- How can NorthTech define its compute infrastructure to respond to changes in load and keep the service available during failures or updates?

- How can NorthTech gain visibility into application and network behavior to detect anomalies before they affect users, diagnose their cause, prioritize critical traffic, and ensure recovery after data loss or service disruption?



### 1.3 Objetives

The objective is not only to deploy a web application, but rather to apply all the AZ-104 areas in a single business scenario.

In addition, the infrastructure will be designed to be created and destroyed using Infrastructure as Code (IaC), reducing costs during the development, testing, and validation phases.


---

## 2. Technical Requirements

R1. 
R2.
R3.
R4. 
R5. 

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


