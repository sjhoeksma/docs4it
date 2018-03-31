---
title: IT as a Service
overviewmap:
 - {name: 'Business' , coord: '4,5,232,79', href: '/framework/01-00-cloud-business' }
 - {name: 'People' , coord: '4,171,232,242', href: '/framework/02-00-cloud-people' }
mainpage: false 
nobackmenu: true
references: 
- {title: 'IT as a Service', url: 'https://www.emc.com/collateral/software/white-papers/h10801-stepstoitaas-wp.pdf'}
---

<div id="textgrid" class="row flex-grid float-right">
<div class="box-item">
{% include image.html image="assets/framework/overview.png" imagemap=page.overviewmap class="width-default" %}
</div>  
<div class="box-item">
**Introduction-** There is a lot of information available on internet about the Digital Transformation of IT. But what I found out in the many years i worked as a business alignment manager between the Business and IT that is is important to tell the whole story. On this site i have bundeld all information i collected in the year into one (for me) consistant story. 
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


**Final Thanks-** to all everbody how has contributed to this site by editing the content through [GitHub](https://github.com/sjhoeksma/sjhoeksma.github.io). For all people and companies which are making create content avaiable trough sites and documents, links to these sources can always befound on the bottom of a page. 
