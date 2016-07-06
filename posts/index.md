---
layout: index
title: All Posts
excerpt: "A List of Posts"
comments: false
---
<div class="post-list">
    {% for post in site.posts %} 
        {% if post.project == null %}
    <ul>
        <li class="wow fadeInLeft" data-wow-duration="1.5s">
            <a class="zoombtn" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
            <p>{{ post.excerpt }}</p>
            <a href="{{ site.url }}{{ post.url }}" class="btn zoombtn">Read More</a>
        </li>
    </ul>
        {% endif %}
    {% endfor %}
</div>