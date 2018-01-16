---
layout: compress
permalink: /print/
---

<html lang="en" itemscope itemtype="http://schema.org/BlogPosting">
    {% include head.html %}
    {% include svg-icons.html %}
    <body class="has-push-menu">
       <section class="post">
        {% include header.html sidemenu=site.usesidemenu %}
          {% assign pages = site.mof | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
         
          {% assign pages = site.framework | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
          
          {% assign pages = site.principles | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
          
          {% assign pages = site.data.roles %}
          {% for page in pages %}
            {% include article-role.html class='post-content' %}
          {% endfor %}
          
          {% assign pages = site.posts | sort: 'url' %}
          {% for page in pages %}
            {% include article-framework.html %}
          {% endfor %}
         

          {% include footer.html %}
        </section>
    </body>
</html>  