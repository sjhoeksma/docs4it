---

title:  Cloud Storage Provisioning
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
- cloud
- provisioning
introduction: Focuses on the organization’s capability to provide storage in support of enterprise applications.
references:
 - { title: 'The Cloud Storage Provisioning Roadblock', url: 'http://www.storage-switzerland.com/Articles/Entries/2013/1/22_The_Cloud_Storage_Provisioning_Roadblock.html' }
---

{{ page.introduction }}
Storage provisioning in the cloud is accomplished with cloud-based block and
file storage. The skills and processes required to provision these services are
significantly different from provisioning the physical storage area network
(SAN), network-attached storage (NAS), and disk drives.

## The Problem With Legacy Storage Provisioning

This need for better storage provisioning capabilities has lead the storage suppliers in the industry to add storage virtualization capabilities to their legacy storage systems. But this virtualization is often internal, meaning it is isolated to a single system and a single manufacturer. Internal storage virtualization has simplified, to a degree, the storage provisioning process by allowing an administrator to simply select the size of the partition and letting the storage system do more of the work. With internal virtualization the administrator will still receive every storage request, analyze the request and know where to provision that storage from. All of which becomes a bottleneck to service delivery.

It also leads to having multiple storage virtualization software instances running as each system from each manufacturer has its own software that needs to be learned and interacted with. The CSP/MSP typically has a wide collection of storage hardware. This would be similar to having a different brand hypervisor loaded on every server and having to manage each of those separately.  

Legacy provisioning as it is provided by internal storage virtualization also requires that the administrator know which type of storage and storage system from which the provisioning will occur. The administrator needs to make the physical connection between the performance needs of the application and the storage environment's available storage media types. They must know which media types and systems are best suited for each type of request. 


## Provisioning is More Than Capacity

The current internal storage virtualization capabilities found in legacy systems are limited to the provisioning of capacity. Storage, like servers, has more than just one resource and applications will use those resources differently depending on the situation. Storage resources include the storage CPU, storage controller memory, internal cache management and network bandwidth in addition to physical capacity required. The combination and control of these resources represent the amount of IOPS (input/output operations per second) or throughput and storage latency that a storage system can deliver. But as is the case with storage capacity not all servers or applications need the same amount of IOPS or storage latency. Legacy storage systems simply don't provide a granular way to allocate performance within a storage system. 

The lack of the ability to provision performance plagues even more modern storage systems as well as storage virtualization software that claims to be designed for the highly virtualized data center. Reality is that these systems may be appropriate for those situations but are not able to meet the provisioning needs of the CSP/MSP. 

## Provision Requirements of the CSP/MSP
The CSP/MSP is foreshadowing what the enterprise will become in the near future; a data center that is judged on its ability to respond rapidly to an ever growing and ever demanding user base. In the case of a CSP/MSP these "users" are accounts that pay a monthly fee and have specific service level agreements (SLA) requirements of the CSP/MSP. The speed at which provisioning can be performed and the ability for that provisioning rule to be maintained over time is the foundational component in meeting those SLAs.

## Self-Serviced Provisioning
For the CSP/MSP to be profitable they cannot afford to hire administrators every time a new account is brought on or even after 100 accounts are brought on. Instead they need to be able to safely delegate provisioning to the account while maintaining oversight. This means allocating a certain amount of capacity and IOPS/throughput/latency per account and then allowing the account to divide up those services based on need. 

Self monitoring also may be a need in many cases. The account wants to know how much he is using on which application at what time. This will help them to better manage their applications running at a CSP/MSP.


## Manages User’s Expectations

A key challenge with not being able to provision IOPS in legacy systems is that the performance experience can not be controlled. This creates an expectations problem because users that sign up for a bronze service level get the same performance experience that a gold service level gets. 

Even if different class systems are used to allocate the performance resources, the first set of users on a system will experience a higher than promised level of performance and then see their performance degrade as more accounts are added to a system. The CSP/MSP needs the ability to guarantee a certain level of performance, no more, no less, so that user’s expectations can be managed.  

This level of performance needs to remain constant, so the performance that the user sees from their assigned storage is the same today as it will be a year from now. Changes to the environment and even the storage system itself should not impact the user nor jeopardize the SLA. 


## Efficient Provisioning

The MSP/CSP needs to balance the cost advantages of maximizing storage resources with the customer satisfaction risks associated with extending a system too far. They need a storage system that will allow them to granularly assign capacity and performance resources so that these systems can be taken to their maximum capabilities without risking customer satisfaction. 

Essentially each available GB and IOPS needs to be bought and paid for prior to investing in an additional system. This allows the addition of new storage investment to be trended based on the rate that resources are being consumed on present systems. In short the storage environment needs to scale like the CSP/MSPs business scales. 

When a customer or account demands storage with varying levels of performance and capacity, they may need to be provisioned from different storage systems. The administrator needs to know which storage system has how much capacity and performance left out. When manually managed by the administrator, storage fragmentation occurs, usually. 

Storage fragmentation is a phenomenon in which large number of storage systems have the ability to provide a certain type of storage but none of the storage system is capable of providing one type of storage. For example, if there are 10 storage systems in the infrastructure and the CSP/MSP admin provisions 5TB/1000 IOPS volumes equally on all of them, when the system is 70% full, it may not be possible to provision 5TB/20000 IOPS, as this needs writing across large number of disks, but the disks are 70% full. Intelligent and automated provisioning guidelines will help avoid such a scenario. 


## Multi-Vendor, Multi-Tier Provisioning

CSP/MSP also need the storage system to provide this provisioning along with other storage services like thin provisioning, snapshots, cloning and replication, across multiple storage platforms, even those from different vendors. This allows the CSP/MSP to manage their entire storage environment from a single interface regardless of the manufacturer of the individual platform. Performance can then be allocated intelligently across platforms by finding the storage system with the storage resources that best match the IOPS requirement. It also saves the MSP/CSP from the vendor lock in associated with buying a single vendor’s system, giving them flexibility to select storage systems based on suitability to the task at hand.

## Introducing Elastic Provisioning

Elastic provisioning is the ability to provision both capacity and performance resources data center wide from a single interface. It models the server virtualization concept by deploying a series of off the shelf servers to act as physical storage controllers. The storage in the environment is then assigned to these storage controllers. Since these controllers are abstracted from the physical storage they can manage a mixed storage vendor environment. 

Elastic storage provides the ability to spawn virtual controllers similar to how a server host spawns virtual servers. Each of these virtual controllers is assigned to an account. Capacity and IOPS/Throughput/Latency, based on the needs of the account, are then assigned to the virtual controller. The account can then sub-divide the capacity and SLA parameters based on the needs of each of its applications. 

This virtual controller functionality ensures that a misbehaving application at one account won't impact the capacity or performance needs of another account. There is complete isolation. It also insures that data can be segregated between accounts, another common concern in the CSP/MSP. 

## From CSP to the Enterprise
It is easy to see how the enterprise could leverage these capabilities as well. Instead of accounts, different lines of business or application groups could be assigned virtual storage controllers. Those groups could then manage their own storage without risk to the other groups. As is the case with CSP/MSPs the enterprise also has a mix of storage systems and could benefit from a centralized controller cluster. 


## Summary
Provisioning of storage remains a key challenge in data centers of all types and sizes but it is especially problematic for the CSP/MSP. It becomes THE bottleneck in rapidly responding to customer requests and its limitations make it difficult to guarantee long term adherence to SLAs. Elastic provisioning is a viable solution to this problem. It provides for multi-vendor provisioning of both capacity and performance resources.