## Details of project context 


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
