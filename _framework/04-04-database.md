---

title:  Cloud Database Provisioning
date:   2018-01-01 08:30:56
category: Strategy
tags:
- strategy
- cloud
- provisioning
introduction: Addresses the organization’s capability to providedatabase and database management systems in support of enterprise applications.
references:
- {title: 'SQL Server Database Provisioning', url: 'https://www.red-gate.com/simple-talk/sql/database-delivery/sql-server-database-provisioning/'}
---

{{ page.introduction }}
The skills and processes supporting this capability change significantly from
managing hardware-bound and cost-bound databases to provisioning standard
relational database management systems (RDMS) in the cloud and leveraging
cloud-native databases.

Database provisioning for development work isn't always easy. The better that development teams meet business demands for rapid delivery and high quality, the more complex become the requirements for the work of development and testing. More databases are required for testing and development, and they need to be more rapidly kept current. Data and loading needs to match more closely what is in production. 

When more than one developer is working on a development database, it is wise to ensure that developers can easily set up, or provision, their own versions of the current build of the database as a part of having an isolated development environment. By providing a separate copy of the current version of the database, it is easier to ensure that any one person working on code doesn’t break the work being done by others. This goes some way to support a DevOps approach to database development. It doesn’t remove the need for integration and integration testing, but it improves the individual developer’s ability to get work done unhindered by the overhead of team-based database development.

Provisioning any type of server environment for this type of isolated development is tricky, whether it involves web servers, active domains or email servers, but when we add databases to the provisioning story, as with just about everything with databases, the situation becomes more challenging.

## Challenges of Provisioning Database
As soon as you start to automate the process of creating databases for developers you’re going to hit a number of issues. Each of these makes it more difficult to create an automated, hopefully self-service, method of provisioning a database. Ideally, you’d like the developers to manage this themselves via an automated system but there are plenty of roadblocks on the route to that Eldorado.

### Size of Database
It is quick and easy to automate the simple process of creating an empty database. However, the production environment will never involve just an empty database, and the developer will have to be certain that the database will work with a volume of data with the same characteristics, distribution and size as the production data. Basically, you’re going to need that sort of data for at least part of the development process. That data is going to have to be at least representative of your production data, though you’d be unlikely to be able to use a copy of it (see more on Production Data in the section below). This means you’re moving more than a few rows. Most databases these days are at least hundreds of gigabytes in size and may run into many terabytes or more.

The size of the data presents two immediate challenges to provisioning. First, you need to have the space available to provide this for each of the developers. For relatively small databases of 20-50gb, this is no big deal nowadays, but the more production-like the volume of data gets to be, the larger the size of disk-space required. Second, as the sizes increase, it makes provisioning slower and slower in an almost linear fashion. Restoring or migrating more data simply takes more time.

### Timing of Provisioning Refresh
When you have several developers working on a single development database, but working with different parts of that database in varying degrees of completion for any given piece of functionality, one developer may want to check in his work and get a fresh build of the database, while the others haven’t completed their code or even set up adequate unit testing for the new functionality yet and need to remain on the current version increment of the database. Add in a testing team or even multiple development teams and this problem multiplies. You could just hope that they are all happy with the same set of data, but what if someone needs an extreme version for scalability tests, or run integration tests on a process, using a known input set of data?

As long as the individual is responsible for their own database, they can largely ignore the current status of other databases, however, as soon as integration has to occur, multiple versions of test data, structures or code could cause severe difficulty.

### Production Data
In theory, the very best data for testing aspects of the functionality to ensure that it will work when the code gets to production is the data from production. However, data is becoming more and more tightly regulated, up to and including the actual threat of prison time for intentionally sharing data with unauthorized people.

Even if there were no need for regulatory compliance, it would be crazy to allow your developers to have production data on their development laptops. These are likely to leave the building regularly and could be, and often are, lost or stolen. The information managed within these databases defines many modern businesses, so losing something like a database of customers to the competition could be crippling.

You could easily imagine that you just need to mask the data, to render it compliant. The problem with this is that you would need to mask the data without affecting its distribution. The reason for wanting to use production data in the first place is because of its size and distribution. If you change the way it is distributed as well as the actual values then what is its’ value? It may not respond to queries in the same way.

## Necessary Provisioning Requirements for Databases
On top of the problems with data, there are requirements that must be met within a standard development and deployment process in support of more accurate and faster development.

### Clean Data
The data that gets distributed through the provisioning process must be clean. Not just for reasons of legal compliance, although, of course, that also applies. Instead, we’re cleaning the data in order to be sure that our tests will work smoothly and accurately. For example, if you’re testing email from the application, you want the email information stored within the database to be an email address that can be checked as part of the testing process in order to validate that things are working end-to-end. This means that the data within the provisioned database will have to be modified to reflect the needs of the testing.

### Accurate Distribution
Although you may want to use masked or obfuscated production data in order to meet clean data requirements or answer regulatory limits, that doesn’t mean that you can simply update all the information to a single string. This will ruin any special types of data distribution that occurs in production. In order to provide meaningful testing data, the replacement process should provide a means of ensuring that the replacement data is similar to that which is being replaced. Without this you could have indexes with a single value or statistics that are radically skewed differently to your production servers.

## Methods for Meeting Challenges and Requirements
Although it is difficult to meet the challenges and requirements for database provisioning, it’s not impossible. Virtualization and containerization technologies can help. For example, a new Redgate tool, SQL Clone, builds on standard disk virtualization technologies in Windows to allow us to create a database ‘clone’ that behaves just like a normal database, but has a vastly smaller footprint. Generally though, you just have to approach this problem in the same way you do other problems within your database management system.

### Automation
The first and most important aspect of ensuring a fast, accurate, repeatable provisioning process, as well as possibly supplying a mechanism of self-service is to use automation. You must automate the database clean-up. From there you have to automate the mechanisms for refreshing the database to your development and test systems (probably taking advantage of some type of restore). By automating all these steps you can ensure that they will work the same way every time. If you build a script to cleanse data, you’ll be sure that the data is clean, every time. Just be sure that your data manipulation processes run in an atomic fashion, meaning, all or nothing on the commit so that you don’t accidently release production data to the development environment.

### Communication
Everyone should know what the process is, how it works, and, most importantly, how often you’re updating the root provisioning database. This is vital. Everyone needs to understand the process so that they know where to go to get the database and so that the business and the auditors know that you’re protecting the production system. Everyone must know how the process works in order to be able to help with adjusting process over time as needs and requirements change or additional checks, tests, data modifications and data masking are added. Finally, everyone needs to know how frequently the provisioning is set up in order to appropriately schedule their own activities.

## Conclusion
While provisioning for databases certainly has a large number of challenges, many of them can be overcome through careful communication and precise automation. Through these means you should be able to automate preparation of a provisioning database and, possibly, provide a means of self-service in order to support your DevOps processes within the database in as efficient a fashion as possible.