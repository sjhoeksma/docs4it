---
title: References
permlink: /references
---

Below you find a list of references to original material used within this site.

{% assign refs="" | split:"" %}

{% for ref in site.references %} {% assign refs = refs | push: ref %}{% endfor %}
{% for post in site.posts %} {% include reference.html page=post output=false %}{% endfor %}
{% for post in site.framework %}{% include reference.html page=post output=false %}{% endfor %}
{% for post in site.mof %}{% include reference.html page=post output=false %}{% endfor %}
{% for post in site.data.roles %}{% include reference.html page=post output=false %}{% endfor %}
{% for post in site.principles %}{% include reference.html page=post output=false %}{% endfor %}
{% assign refs=refs | sort:"title" %}
<footer><p>     
{% for ref in refs %}
<a class="feed" href="{{ ref.url }}" title="Reference">
  <svg class="love"><use xlink:href="#icon-heart"></use></svg>
  {{ ref.title }}
</a>
{% endfor %}
</p></footer>