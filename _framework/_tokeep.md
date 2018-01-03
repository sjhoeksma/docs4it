---
layout: framework
title:  Cloud Framework
date:   2017-01-01 08:30:56
category: Strategy
#description: We try to explain cloud.
image: '/assets/framework.png'
imagemap:
 - {name: 'Finance' , coord: '233,5,460,170', href: '#finance' }
 - {name: 'Strategy', coord: '461,5,690,170', href: '#strategy'}
 - {name: 'Benefits', coord: '461,5,690,170', href: '#benefits'}
tags:
- strategy
- cloud
introduction: The Cloud Framework organizes guidance into six areas of focus, which span the entire organization. We describe these areas of focus as Perspectives. Perspectives each encompass distinct responsibilities owned or managed by functionally related stakeholders. 
mermaid: true
reference: https://aws.amazon.com/professional-services/CAF/perspectives/
---


```
---
layout: framework
title:  Cloud
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
- cloud
introduction: 
---

{{ page.introduction }}
```

{{ page.introduction }} There are three perspectives addressing Business Stakeholders and three perspectives addressing Technology Stakeholders
Each of the six Perspectives that make up the Cloud Framework as is described below.

# Business
Helps stakeholders understand how to update staff skills and organizational processes involved in business support capabilities, to optimize business value with cloud adoption.

**Common Roles:** Human Resources; Staffing; People Managers.
<a class="anchor" id="People"></a>
# People
Provides guidance for stakeholders responsible for people development, training, and communications. Helps stakeholders understand how to update staff skills and organizational processes with cloud based competencies.

**Common Roles:** Business Managers; Finance Managers; Budget Owners; Strategy Stakeholders.

<a class="anchor" id="Governance"></a>
# Governance
Provides guidance for stakeholders who support business processes with technology, and who are responsible for managing and measuring the resulting business outcomes. Helps stakeholders understand how to update staff skills and organizational processes necessary to ensure business governance in the cloud.

**Common Roles:** CIO; Program Managers; Project Managers; Enterprise Architects; Business Analysts; Portfolio Managers.

<a class="anchor" id="Platform"></a>
# Platform
Helps stakeholders understand how to update staff skills and organizational processes necessary to deliver, maintain, and optimize cloud solutions and services.

**Common Roles:** CTO; IT Managers; Solution Architects.

<a class="anchor" id="Security"></a>
# Security
Provides guidance for stakeholders responsible for staff skills and organizational processes necessary to ensure that the workloads deployed or developed in the cloud align to the organization’s security control, resiliency, and compliance requirements.

**Common Roles:** CISO; IT Security Managers; IT Security Analysts; Head of Audit and Compliance.


<a class="anchor" id="Operations"></a>
# Operations
Helps stakeholders understand how to update staff skills and organizational processes necessary to ensure system health and reliability through the move to the cloud, and as an agile, ongoing, cloud computing best practice.

**Common Roles:** IT Operations Managers; IT Support Managers.

<a class="anchor" id="Finance"></a>
## Cloud Finance

<a class="anchor" id="Strategy"></a>
## Cloud Stratergy

<a class="anchor" id="Benefits"></a>
## Benefits Realisation

<a class="anchor" id="Risks"></a>
## Business Risk Management


<a class="anchor" id="Resource"></a>
## Resource Management

<a class="anchor" id="Training"></a>
## Training Management

<a class="anchor" id="Change"></a>
## Organisational Change Management


<a class="anchor" id="Portfolio"></a>
## Portfolio Management
<div class="mermaid">
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section A section
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d
        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d
</div>

<a class="anchor" id="Project"></a>
## Project Management

<a class="anchor" id="Performance"></a>
## Business Performance Management

<a class="anchor" id="Project"></a>
## Project Management







<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
</div>

<div class="mermaid">
sequenceDiagram
    participant Alice
    participant Bob
    Alice->John: Hello John, how are you?
    loop Healthcheck
        John->John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->Alice: Great!
    John->Bob: How about you?
    Bob-->John: Jolly good!
</div>

<div class="mermaid">
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section A section
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d
        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d
</div>


Cloud Links
* [http://glasshouse.io/addressing_cloud_migration_complexity_88](http://glasshouse.io/addressing_cloud_migration_complexity_88)
* [http://michaelcorey.com/blog/cloud-application-migration-strategies-the-6-rs/](http://michaelcorey.com/blog/cloud-application-migration-strategies-the-6-rs/)
* https://medium.com/@BotmetricHQ/the-5-pillars-of-aws-well-architected-framework-84345ca54a30
* https://blogs.endjin.com/2016/08/aws-vs-azure-vs-google-cloud-platform-analytics-big-data/
