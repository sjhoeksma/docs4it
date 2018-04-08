---
title:  Service Demand
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
introduction: Provides guidance to stakeholders who support business processes with technology, and who are responsible for managing and measuring the resulting business outcomes. Helps stakeholders understand how to update staff skills and organizational processes necessary to ensure business governance in the cloud.
references: 
- {title: 'What is Agile' , url: 'https://www.agilealliance.org/agile101/'}
---
{{ page.introduction }} 

**Common Roles:** CIO; Program Managers; Project Managers; Enterprise Architects; Business Analysts; Portfolio Managers.

The Governance Perspective focuses on the skills and processes that are needed to align IT strategy and goals with your organisation business strategy and goals, to ensure your organization maximizes the business value of its IT investment and minimizes the business risks.
This Perspective includes Program Management and Project Management capabilities that support governance processes for service adoption and ongoing operations. 

## Service Life Cycle
The overall service life cycle can be divided into 4 clear steps; 
* **Demand**: ensure that the service requests of the business have an owner, are clearly defined, prioritized and approved
* **Deliver**: creates the services defined by the business, according to delivery method 
* **Operate**: ensures that the services are operated within the agreed service level
* **Retire**: ensures the correct disposal of the services which are no longer required.

![portfolio](/assets/framework/portfolio.png)

The Service Life Cycle start with the creation of a Service Plan by the Business Owner. When the business demands on the  service are clear, a product request can be created. This request is validate and approved **(G-0)** by the CTO responsible for the business function. During the incubation phase a high level solution direction and cost estimation is made. This information is added to the product request. This request is again validated and approved **(G-1)** by the responsible CTO. After this approval the delivery is planned according to the selected delivery lane. When the requested service needs goods or external services then CTO is approval **(G-2)** is required before building of the services can start. During the certification phase, the mandatory tests are evaluate and only when successful or after exception sign-off of the CTO **(G-3)** the service will be deployed. After the last deployment for this service, the product request will be closed **(G-4)**

### Service Demand

![portfolio](/assets/framework/infunnel.png)

For every function group there will be regular portfolio meeting, where business and the alignment manager meet together defining which services are required by the business. For each service the CTO decides if IT should invert time creating a high level solution direction. During this incubation phase also all external, risk and compliancy task will be performed. When services has impact on more then one function group the proposal needs to evaluated by the Business IT council. If the cost of the services is above the mandate of the Business IT council it will be forwarded to the CIO for approval. After the product request has been updated with the required approval the CTO has to give his final approval.  

![portfolio](/assets/framework/riskassesment.png)

When goods or external services are required an additional Risk and compliancy check needs to be done. Any purchasing activity needs to be completed (step 7) before **(G-2)**

### Service Delivery

![portfolio](/assets/framework/inpipeline-waterfall.png)

When for a services an traditional delivery model is chosen then during the preparation phase we will focus on requirements gathering and detail design. During the Build phase we will build one or more features and combine them later into on release.  

![portfolio](/assets/framework/inpipeline-agile.png)

**User Stories**: In consultation with the customer or product owner, the team divides up the work to be done into functional increments called "user stories." Each user story is expected to yield a contribution to the value of the overall product.

**Daily Meeting**: Each day at the same time, the team meets so as to bring everyone up to date on the information that is vital for coordination: each team members briefly describes any "completed" contributions and any obstacles that stand in their way.

**Incremental Development**:  Nearly all Agile teams favor an incremental development strategy; in an Agile context, this means that each successive version of the product is usable, and each builds upon the previous version by adding user-visible functionality.

**Iterative Development**:  Agile projects are iterative insofar as they intentionally allow for "repeating" software development activities, and for potentially "revisiting" the same work products.

**Team**: A "team" in the Agile sense is a small group of people, assigned to the same project or effort, nearly all of them on a full-time basis. A small minority of team members may be part-time contributors, or may have competing responsibilities.

**Milestone Retrospective**:  Once a project has been underway for some time, or at the end of the project, all of the team's permanent members (not just the developers) invests from one to three days in a detailed analysis of the project's significant events.

**Personas**:  When the project calls for it - for instance when user experience is a major factor in project outcomes - the team crafts detailed, synthetic biographies of fictitious users of the future product: these are called "personas".

![portfolio](/assets/framework/changemanagement.png)

Within the change process we focus on developing standard (preferred automated) service release process. We validate if all required documentation and test are provided. In case of a failure you should perform a root cause analysis and adopt require changes to the standard release process. The task of the changes manager will become more a facilitator of the process and auditor after the changes is completed.[(more..)](/framework/06-04-change-release)

![portfolio](/assets/framework/certify.png)

During certify we check if all required certifications steps are performed and completed successful. When not successful and it is required to continue an exception has to be provided by the CTO. 

### Service Operation

![portfolio](/assets/framework/inproduction.png)

During the deploy phase the provides is preferable automatically deployed on the required infrastructure. The information to support the new/update services is communicated or trained to all impacted resources.  

### Service Retirement

![portfolio](/assets/framework/retire.png)

When a service needs to be retired, all data should be archived or destroyed, people should be transferred to other jobs or let go. The services and assets should unregistered. 