---
layout: framework
title:  Cloud License Management
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
- cloud
- process
introduction: Defines your organization’s capability to procure,distribute, and manage the licenses needed for IT systems, services, and software. 
references:
 - { title: 'Software licensing in the cloud', url: 'https://www.computerworld.com/article/2496855/cloud-computing/software-licensing-in-the-cloud.html' }
---

{{ page.introduction }}
The cloud consumption model requires that teams develop new skills
for procurement and license management and new processes for evaluating
license needs.

The cloud delivery models that present the most software-licensing challenges are infrastructure as a service (IaaS) and platform as a service (PaaS). Software as a service (SaaS) is less likely to cause problems because, as the name suggests, the software is part of the cloud provider's services. With IaaS and PaaS, though, the customer has shared control over what is run in the cloud environment, including third-party software. In the case of IaaS, the customer does not manage or control the underlying cloud infrastructure but may have control over operating systems and deployed applications. With PaaS, while the customer typically doesn't have control over the operating system, it may have control over the deployed applications.

Where the complexity comes in is that software manufacturers are all over the map in how they address cloud use in their software licenses. Some base their licensing on the number of users, and those users in turn may be named or concurrent. Others charge per processor or core that the software runs on. Still others look at actual usage, a metric that is distinct from number of users. The one thing that these various licensing models have in common is that they are attempts to maximize revenue, and naturally, software makers view the use of their products in the cloud as an expansion of licensing rights that represents an opportunity for increased revenue.

Can the customer argue that the cloud does not represent an expansion of licensing rights? It would be difficult. If the customer acquired its software licenses from the vendor under a long-standing agreement, chances are good that the agreement pre-dates the inception of cloud computing. Of course, contracts generally do not address technology offerings that don't exist at the time of the contract's drafting, so a pre-cloud software-licensing contract is highly unlikely to contemplate the use of those licenses in a cloud environment. Legally, any rights that aren't explicitly stated as being granted to the customer in the license agreement are retained by the software manufacturer. In cases like this, customers do not have any pre-existing rights to use their software licenses in the cloud.

## Parsing the clauses
To better understand the challenges that the cloud brings to software licensing, it might be helpful to take a look at some clauses that one might see in a cloud vendor's contract. Below are four, followed by my explanation of what they mean and why they're pertinent.

> Customer authorizes [VENDOR] to copy, install and modify, when necessary and as required by this Agreement, all third-party software to be used in the Services.

*What this means:* As part of providing the service, the cloud vendor may need to access the software in order to create redundant systems, and potentially to replicate or restore the customer environment in the event of an unplanned outage or other disaster. The above language says that the customer gives the cloud vendor permission to do these things on its behalf.

> Customer warrants to [VENDOR] that it has obtained any licenses or approvals required to give [VENDOR] such rights or licenses to access, copy, distribute, use and/or modify or install any third-party software to be used in the Services.

*What this means:* This affirms that the customer's license agreement with the software manufacturer includes the rights for the cloud vendor to access the software in the manner described above.

> Some third-party software manufacturers' contract terms and conditions may become void if [VENDOR] provides services for or works on the software (such as providing maintenance services). [VENDOR] DOES NOT TAKE RESPONSIBILITY FOR THIRD-PARTY WARRANTIES OR FOR ANY EFFECT THAT THE [VENDOR'S] SERVICES MAY HAVE ON THOSE WARRANTIES.

*What this means:* The cloud vendor is saying that if its use of the software in providing the services causes any noncompliance with the terms of the software-license agreement, then the cloud vendor is not responsible for any adverse consequences.

> Third-party software shall be exclusively subject to the terms and conditions between the third-party software provider and Customer. [VENDOR] shall have no liability for third-party software.

*What this means:* The cloud vendor is saying that it has no responsibility regarding the effective functioning of the software, or any adverse impacts of any malfunctioning of the software.

All this adds up to the fact that you need to clearly identify your license rights and usage needs before deploying third-party software in the cloud, then effectively capture those in your contract with the cloud vendor.

