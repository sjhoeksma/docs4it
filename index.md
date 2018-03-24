---
mainpage: true 
---

<main class="home" >
    <div id="grid" class="row flex-grid float-right">
    {% for post in site.data.topics %}
        <article id="{{ post.title | remove: ' ' }}" class="box-item" itemscope="itemscope" itemtype="http://schema.org/BlogPosting" itemprop="blogPost">
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