---
title: Introduction
overviewmap:
 - {name: 'Strategy' , coord: '11,6,270,62', href: '/framework/01-02-strategy' }
 - {name: 'Delivery' , coord: '11,63,270,581', href: '/framework/03-01-portfolio' }
 - {name: 'Governance' , coord: '11,582,270,633', href: '/framework/' }
mainpage: false 
nobackmenu: true
references: 
#- {title: 'IT as a Service', url: 'https://www.emc.com/collateral/software/white-papers/h10801-stepstoitaas-wp.pdf'}
---

<div id="textgrid" class="row flex-grid">
<div class="box-item box-item-grow-20" markdown="1">
There is a lot of information available on internet about the Digital Transformation of IT. What I found out during the many years I worked as a business alignment manager is, that it is important to tell a consistent story. So I bundled all the collected information, into one (for me) consistent story. 

The last years IT has become a commodity, fulling the **Digital Transformation Strategy** and blurring the boundaries between business and IT. Because of the complexity and cost involved with IT is still of great value to have strong and clear **Governance**. Your strategy and governance will always include aspects around **IT Service Delivery**, which starts with defining you service needs (in funnel) and retiring the services when they are no longer required (retired). 

The site has been made interactive, resulting that most image like the overview picture are clickable and in this way giving direct access to a specific topics. You can also use the search icon on the left side to find any topic.

</div>  
<div class="box-item">
{% include image.html image="assets/framework/overview.png" imagemap=page.overviewmap class="width-default" hideclickable=false %}
</div>
</div>	

## Quick Access
The links below give you access to the most common used items
<main class="home" >
    <div id="grid" class="row flex-grid float-right">
    {% for post in site.data.topics %}
        <article id="{{ post.title | remove: ' ' }}" class="box-item hover" itemscope="itemscope" itemtype="http://schema.org/BlogPosting" itemprop="blogPost">
            <span class="category">
                <a href="{{ post.url | prepend: site.baseurl }}">
                    <span class="float-left">{{ post.title }}</span>
                </a>
            </span>
            <div class="box-body">
                {% if post.image %}
                    <div class="cover">
                        <a href="{{ post.url | prepend: site.baseurl }}" {%if isnewpost %}class="new-post"{% endif %}>
                            <img src="/img/placeholder.png" data-url="{{ post.image }}" class="preload">
                        </a>
                    </div>
                {% endif %}
                <div class="box-info">
                    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
                        <p class="description">{{ post.introduction }}</p>
                    </a>
                </div>
            </div>
        </article>
    {% endfor %}
    </div>	
</main>


**Final Thanks** to all everybody how has contributed to this site by editing the content through [GitHub](https://github.com/sjhoeksma/sjhoeksma.github.io). For all people and companies which are making create content available trough sites and documents, links to these sources can always be found on the bottom of a page. 
