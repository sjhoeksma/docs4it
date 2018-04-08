---
article: principle
title: Low-coupling interfaces
category: Platform principles
description: Interfaces have low coupling, are self--described, and offer low impact on the financial institution in case of changes.
rationale: 
 - Low-coupling interfaces are preferable, because when interfaces between independent applications are highly coupled, they are less generic and more susceptible to causing unwanted, secondary effects when they are changed.
implications:
- Low coupling means that the services (corporate APIs, for example) are conceived with no affinity to a certain service consumer.
- Therefore, the service is completely uncoupled to a service consumer. However, the service consumer is dependent of the service (that is, contains references for service interfaces).
- The service is also responsible for exception treatment. The result is a low-coupling architecture.
---

