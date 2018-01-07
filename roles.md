---
layout: main

---

<main class="home" id="post" role="main" itemprop="mainContentOfPage" itemscope="itemscope" itemtype="http://schema.org/Blog">
   <div class="index">
    <div id="grid" class="row flex-grid float-right">
    {% for post in site.data.roles %}
        <article id="{{ post.role | remove: ' ' }}" class="box-item" itemscope="itemscope" itemtype="http://schema.org/BlogPosting" itemprop="blogPost">
                    <h2 class="color-white" >{{ post.role }}</h2>
            <div class="box-body">
                {% if post.image %}
                    <div class="cover">
                      <img src="/img/placeholder.png" data-url="{{ post.image }}" class="preload">
                    </div>
                {% endif %}
                <div class="box-info">
                  <p class="description"><b>Duties: </b>{{ post.duties }}</p>
                        <p class="description"><b>Education: </b>{{ post.education }}</p>
                        <p class="description"><b>Skills: </b>{{ post.skills }}</p>
                </div>
            </div>
        </article>
    {% endfor %}
    </div>	
	</div>	 
</main>