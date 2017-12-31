---
layout: framework
title:  "Explaining Cloud!"
date:   2017-01-01 08:30:56
category: Framework
description: We try to explain cloud.
image: '/assets/framework.png'
imagemap:
 - {name: 'Finance' , coord: '233,5,460,170', href: '#Finance' }
 - {name: 'Strategy', coord: '461,5,690,170', href: '#Strategy'}
 - {name: 'Benefits', coord: '461,5,690,170', href: '#Benefits'}
tags:
- app
- mobile
- ios
introduction: Explaining side
---

Cloud Links
* [http://glasshouse.io/addressing_cloud_migration_complexity_88](http://glasshouse.io/addressing_cloud_migration_complexity_88)
* [http://michaelcorey.com/blog/cloud-application-migration-strategies-the-6-rs/](http://michaelcorey.com/blog/cloud-application-migration-strategies-the-6-rs/)
* https://medium.com/@BotmetricHQ/the-5-pillars-of-aws-well-architected-framework-84345ca54a30
* https://blogs.endjin.com/2016/08/aws-vs-azure-vs-google-cloud-platform-analytics-big-data/

<a class="anchor" id="Business"></a>
# Business
<a class="anchor" id="Finance"></a>
## Cloud Finance

<a class="anchor" id="Strategy"></a>
## Cloud Stratergy

<a class="anchor" id="Benefits"></a>
## Benefits Realisation

<a class="anchor" id="Risks"></a>
## Business Risk Management

<a class="anchor" id="People"></a>
# People

<a class="anchor" id="Resource"></a>
## Resource Management

<a class="anchor" id="Training"></a>
## Training Management

<a class="anchor" id="Change"></a>
## Organisational Change Management

<a class="anchor" id="Governance"></a>
# Governance
<a class="anchor" id="Portfolio"></a>
## Portfolio Management
{% mermaid %}
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
{% endmermaid %}

<a class="anchor" id="Project"></a>
## Project Management

<a class="anchor" id="Performance"></a>
## Business Performance Management

<a class="anchor" id="Project"></a>
## Project Management








{% mermaid %}
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
{% endmermaid %}

{% mermaid %}
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
{% endmermaid %}

{% mermaid %}
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
{% endmermaid %}

