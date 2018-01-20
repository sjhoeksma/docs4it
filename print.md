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
          <chapter>
          {% assign pages = site.mof | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
          </chapter><chapter>
          {% assign pages = site.framework | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
          </chapter><chapter>
          {% assign pages = site.principles | sort: 'url' %}
          {% for page in pages %}
            {% include article-{{ page.layout | default: 'framework'}}.html %}
          {% endfor %}
          </chapter><chapter>
          {% assign pages = site.roles %}
          {% for page in pages %}
            {% include article-role.html class='post-content' %}
          {% endfor %}
          </chapter><chapter>
          {% assign pages = site.posts | sort: 'url' %}
          {% for page in pages %}
            {% include article-framework.html %}
          {% endfor %}
          </chapter>

          {% include footer.html %}
        </section>
    </body>
</html>  