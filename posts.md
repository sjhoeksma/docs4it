---
layout: submain
---

<main class="home" id="post" role="main" itemprop="mainContentOfPage" itemscope="itemscope" itemtype="http://schema.org/Blog">
   <div class="">
    {% if site.usenavigation %}
		  {% include navigation.html %}
    {% endif %}
    <div id="grid" class="row flex-grid float-right">
    {% for post in site.posts %}
        <article class="box-item" itemscope="itemscope" itemtype="http://schema.org/BlogPosting" itemprop="blogPost">
            <span class="category">
                <a href="{{ site.url }}{{ site.baseurl }}/categoria/{{ post.category }}">
                    <span class="float-left">{{ post.category }}</span>
									<span class="float-right">
                    <svg id="date" class="icon-calendar"><use xlink:href="#icon-calendar"></use></svg>
									<time itemprop="datePublished" datetime="{{ post.date | date_to_xmlschema }}" class="date">
                        {% include date.html date=post.date %}
                    </time>
									</span>	
                </a>
            </span>
            <div class="box-body">
                {% if post.image %}
                    <div class="cover">
                        {% include new-post-tag.html date=post.date %}
                        {% if post.imagemaps != blank %}
                          <img id="img-id-1" src="/img/placeholder.png" data-url="{{ post.image }}" class="preload" usemap="#todo" highlight="1" >
                          <map name="todo">
                          {% for s in post.imagemaps %}
                              <area shape="{{ s.shape | default: 'rect' }}" coords="{{ s.coord }}" 
                                    href="{{ site.baseurl }}{{ s.url }}" 
                                    alt="{{ s.name }}" title="{{ s.name }}"
                                    {{ s.option }}
                              />
                          {% endfor %}
                          </map>
                        {% else %}
                        <a href="{{ post.url | prepend: site.baseurl }}" {%if isnewpost %}class="new-post"{% endif %}>
                            <img src="/img/placeholder.png" data-url="{{ post.image }}" class="preload">
                        </a>
                        {% endif %}
                    </div>
                {% endif %}
                <div class="box-info">
                    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
                        <h2 class="post-title" itemprop="name">
                            {{ post.title }}
                        </h2>
                    </a>
                    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
                        <p class="description">{{ post.introduction }}</p>
                    </a>
                    <div class="tags">
                        {% for tag in post.tags %}
                            <a href="{{ site.baseurl}}/tags/#{{tag | slugify }}">{{ tag }}</a>
                        {% endfor %}
                    </div>
                </div>
            </div>
        </article>
    {% endfor %}
    </div>	
	</div>	 
</main>