---

title:  Alignment of ITIL and MOF
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
- cloud
- mof
introduction: In terms of the approach, both frameworks use a lifecycle structure at the highest level of design. Furthermore, both use processes and functions, although the emphasis differs significantly; ITIL describes many components in terms of processes and activities, with only a few functions, while MOF is almost entirely based on Service Management Functions.
---

{{ page.introduction }} This difference is not as severe as it looks at first hand, since ITIL uses the term “process” for many components that actually are functions.

ITIL follows a phased approach in the lifecycle, and most of the components described in one phase also apply, to a greater or lesser extent, to other phases. The control of the MOF lifecycle is much more discrete, using specific milestones that mark the progress through the various stages in the lifecycle. MOF components that apply to more than one of these three lifecycle phases are separated from the lifecycle phases and described in an underlying Management Layer.
Both frameworks are best characterized as “practice frameworks” and not “process frameworks.” The main difference is  that ITIL focuses more on the “what,” and MOF covers both the “what” and the “how.”

The modeling techniques of ITIL and MOF are not that much different at first sight: both frameworks use extensive text descriptions, supported by flowcharts and schemes. ITIL documents its best practices by presenting processes, activities, and functions per phase of its lifecycle. MOF components have a rigid structure: each SMF has key processes, each process has key activities, and documentation on SMFs and MRs is structured in a very concise format, covering inputs, outputs, key questions, and best practices for each component. This rigid structure supports consistency throughout the framework and supports the user in applying a selection of MOF components for the most urgent local problems. 
The activation and implementation of ITIL and MOF are not really part of the framework documentation. ITIL has been advocating the “Adopt and Adapt” approach. Supporting structures like organizational roles and skills are described for each phase, but implementation guidance is not documented. MOF, like ITIL, offers best practice guidance that can be followed in full but also in part, for addressing a subset of local problems. Both frameworks speak of “guidance,” leaving the actual decisions on how to apply it to the practitioner.

Support structures for ITIL are not really part of the core documents: although a huge range of products claim compatibility with ITIL, and several unofficial accreditation systems exist in the field, the core books stay far from commercial products and from product certification, due to a desire to remain vendor-neutral. MOF compatibility, on the other hand, is substantially established. Microsoft aligns a broad set of tools from its platform with the MOF framework. And although MOF is not exclusively applicable for these Microsoft management products, the documentation at Microsoft’s TechNet website provides detailed information on the use of specific products from the Microsoft platform.
 
## Differences
Although ITIL and MOF share many values, the two frameworks also show some significant differences.
* Cost: ITIL is available in 5 core books that are sold through various channels, but MOF is available on the internet for free. As a consequence, ITIL copyright is highly protected, where Microsoft made MOF content available under the Creative Commons Attribution License, which makes it freely available for commercial reuse.
* Development: in the latest versions, both ITIL and MOF spent considerable energy on documenting the development of new services and the adjustment of existing services. In addition, ITIL is constantly reviewed via the Change Control Log, where issues and improvements are suggested and then reviewed by a panel of experts who sit on the Change Advisory Board. The ITIL Service Design phase concentrates on service design principles, where the Deliver Phase in MOF concentrates on the actual development of services. The approach taken in MOF is heavily based on project management principles, emphasizing the project nature of this lifecycle phase.
* Reporting: ITIL has a specific entity that describes Reporting, in the Continual Service Improvement phase, where MOF has integrated reporting as a standard activity in SMFs.
* Call handling: ITIL V2 showed a combined handling of incidents and service requests in one process, but in ITIL V3 incident restoration and service request fulfillment were turned into two separately treated practices. MOF on the other hand stays much closer to the ITIL V2 practice, combining several customer requests in one activity flow, for incident restoration requests, information requests, service fulfillment requests, and new service requests. If the request involves a new or non-standard service, a separate change process can be triggered.
* Lifecycle construction: Most elements of ITIL are documented in one and only one of the five core books, but it is then explained they actually cover various phases of the ITIL lifecycle. ITIL uses five elements for its lifecycle: Strategy, Design, Transition, Operation, and Continual Improvement, which brings it close to the PDCA model. MOF’s lifecycle comprises only three phases: Plan, Deliver, Operate, with one underlying layer covering the components that apply to all lifecycle phases. As a consequence, a number of practices are applied all over the MOF lifecycle, but in ITIL these are mostly described in one or a few lifecycle phases. As an example, risk management is part of the Manage layer in MOF, but in ITIL it is mainly restricted to Strategy and Continual Improvement. The same goes for change and configuration management: throughout the MOF lifecycle but in ITIL these are concentrated in the Transition phase.
* Organization: ITIL describes roles and organizational structures in each lifecycle phase. MOF supports best practices for organizational structures by applying the Microsoft Solutions Framework (MSF) approach: throughout the MOF lifecycle responsibilities are documented and accountability is made explicit, and general rules are allocated to the underlying Manage layer. 
* Governance: Both frameworks illustrate the difference between governance and management. ITIL describes governance theory and practice in the Strategy phase and in the CSI phase of its lifecycle, and refers to governance requirements in most other phases. MOF explicitly documents accountability and responsibility in all of its lifecycle phases and in the Manage layer, identifying decision makers and stakeholders, and addressing performance evaluation. MOF specifically addresses risk management and compliance in the Manage layer, supporting governance throughout the lifecycle. Explicit Management Reviews are used throughout the MOF framework as control mechanisms. 

## Positioning
This section will show how ITIL and MOF are positioned in the main paradigms, as discussed before. Appendix A shows the differences in more detail.
Lifecycle
On a high level, the lifecycles of ITIL and MOF appear to be rather similar, although the phases cannot be compared on a one-to-one basis. 
 
![LifeCycle](/assets/framework/lifecycle-mof-ittl.png)

There are some major differences between ITIL and MOF lifecycles:
* ITIL lifecycle phases contain processes, activities, and functions that also apply to other phases. In MOF, the SMFs that apply to more than one phase have been filtered out and grouped in the Manage layer, supporting the entire MOF lifecycle.
* MOF lifecycle phase transitions are managed through several Management Reviews (MRs). These MRs serve to determine the status of IT services and to establish readiness to move forward in the lifecycle. ITIL also uses a number of readiness tests for progress control in the lifecycle phases, but these are less explicit.


## People - Process - Technology (PPT)
80 percent of unplanned downtime is caused by people and process issues, including poor change management practices, while the remainder is caused by technology failures and disasters. 
(Donna Scott, Gartner, Inc., 2003)

Both ITIL and MOF have a strong focus on processes. Both frameworks document the activities that need to be performed to cope with everyday problems and tasks in service organizations. Both frameworks also use the same formal definition of “process,” based on widely accepted ISO standards. However, in both cases the framework documentation is largely presented in a mix of process, people, and some technology, and therefore in the format of procedures, work instructions, and functions. This is for good reasons, because it addresses the actual perception of what people experience in their daily practice. Readers looking for “pure process descriptions” or process “models” will not find these in ITIL nor in MOF. And although ITIL uses the term “process” for many of its components, most of these components are actually functions. MOF uses the term Service Management Function throughout the framework.

Organizational structures are documented quite differently in both frameworks. Individual ITIL roles and MOF roles show some overlap, but both frameworks contain a long list of unique roles. This is largely based on the difference in viewpoint: ITIL works from its practices towards a detailed roles spectrum, and MOF works from a number of basic accountabilities: Support, Operations, Service, Compliance, Architecture, Solutions, and Management. MOF applies the MSF framework as a reference system for these organizational structures, supporting the performance of the organization. In larger organizations the MOF roles can be refined into more detailed structures, but in most organizations the roles are sufficient. The Team SMF of MOF is explicitly focused on the management of IT staff.

Technology is only covered at an abstract level in ITIL: the framework stays far from commercial products and only describes some basic requirements. MOF on the other hand is deeply interwoven with technology solutions. Although MOF has been defined in such a way that it is not technology-specific, the Microsoft technology platform highly aligns with the practices documented in MOF. The MOF website is embedded in the rest of the TechNet documentation on Microsoft products.
STO and SoD, in SAME

Strategic levels are covered in both frameworks. ITIL documents its best practices on long-term decisions in the Strategy phase. MOF does the very same in the Plan phase, and supports this in the Manage layer. 
Tactical levels are covered in a similar way: ITIL concentrates these in the Service Design and CSI phase, and MOF describes its tactical guidance in the Deliver phase, in the Manage layer and in the Operate phase (Problem Management).
Operational levels are covered mainly in a single phase in both frameworks; ITIL has its Service Operation phase, and MOF has its Operate phase. 

The ITIL lifecycle phases are positioned mainly in the Technology Management domain, emphasizing that ITIL explicitly supports the organizations that deliver IT services. The activities that relate to the specification of the service requirements and the management of enterprise data architectures are typically found in the middle column of the 3x3 SAME matrix.
 
This also applies to MOF. The MOF Plan phase is largely positioned at the Strategy level, but also concentrates on the Technology Management domain. The Deliver phase is positioned similarly, but then on tactical and operational levels. The Operate phase clearly works at the operational level of the Technology Management domain, except for the very tactical practice of Problem Management.
The Manage layer in MOF relates to all three management levels, but also concentrates at the Technology Management domain.
 
As a consequence, both frameworks require that elements from additional frameworks like TOGAF, ISO27001, CobiT, M_o_R®, BiSL, FSM, and MSP™, are applied for managing the rest of the overarching Information Support domain. 
Plan-Do-Check-Act (PDCA)

ITIL explicitly follows Demings PDCA management improvement cycle, for implementing the CSI phase, for implementing the Information Security function in the Service Design phase and for the continual improvement of services, processes, and functions throughout the service lifecycle. 

MOF does not explicitly list PDCA as a mechanism, but it follows its principles throughout the lifecycle, in all SMFs. Plan-do-check is elementary to the implementation of all SMFs, and various check-act points can be found in the very explicit Management Reviews throughout the MOF framework. 

## Terminology and Definitions
The “ITSM language” is quite consistent between both frameworks, with only minor differences. For example, where ITIL uses the term Change Schedule, MOF uses Forward Schedule of Change. Such small differences shouldn’t be a problem in practice.
Of course both frameworks use some typical terminology that illustrates some of their unique characteristics:
•	The ITIL core terms utility and warranty, fit for purpose and fit for use, are not used in MOF, and neither are terms like service package – although MOF speaks of “packaged products” in general terms. 
•	Likewise, some explicit MOF terms, like customer service management, stabilize, and issue-tracking, are not used—or are used differently—in ITIL.

 
