---
layout: page
title: java 技术
titlebar: java
subtitle: <span class="mega-octicon octicon-organization"></span>&nbsp;&nbsp; java相关
menu: java
css: ['blog-page.css']
permalink: /java
---

<div class="row">

    <div class="col-md-12">

        <ul id="posts-list">
            {% for post in site.tags.java %}
					<li class="posts-list-item">
						<div class="posts-content">
							<span class="posts-list-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
							<a class="posts-list-name bubble-float-left" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
							<span class='circle'></span>
						</div>
					</li>
            {% endfor %}
        </ul> 

        <!-- Pagination -->
        {% include pagination.html %}

        <!-- Comments -->
       <div class="comment">
         {% include comments.html %}
       </div>
    </div>

</div>
<script>
    $(document).ready(function(){

        // Enable bootstrap tooltip
        $("body").tooltip({ selector: '[data-toggle=tooltip]' });

    });
</script>