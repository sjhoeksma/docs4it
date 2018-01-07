---
layout: principle
title: Adherence to functional domains
category: Application principles
description: The business rules and functionality of a system are consistent with the mission of that system. There is complete adherence to the functional domain in which the system is located.
rationale: 
 - The purpose of this principle is to avoid functional redundancy between systems.
 - Functional redundancy can cause loss of data integrity and increase maintenance costs related to the redundant business rule.
implications:
 - Systems must be located in proper functional domains, with explicit definition of the manager in charge of the functional domain.
 - Each new functionality request must be submitted to the respective manager.
 - Applications that are already in production with functional redundancy should be replaced entirely or partially in a timely manner. The functional redundancy of such applications must not be promoted.
---
