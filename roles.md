---
mainpage: true
permalink: /roles/
references:
   - { title: 'Faces of cloud', url: 'https://blogs.vmware.com/accelerate/2013/02/is-your-organization-ready-for-the-software-defined-data-center.html' }
   - { title: 'Operating Transformation', url: 'https://infocus.emc.com/choong_kengleong/cloud-operating-model-transformation/' }
---

<main class="home" id="post" role="main" itemprop="mainContentOfPage" itemscope="itemscope" itemtype="http://schema.org/Blog">
   <div class="index">
    <div id="grid" class="row flex-grid float-right">
    {% for page in site.roles %}
       {% include article-role.html  class='box-item' preload=true %}
    {% endfor %}
    </div>	
	</div>	 
</main>