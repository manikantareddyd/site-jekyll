---
layout: index
title: All Posts
excerpt: "A List of Posts"
comments: false
---
Here is a list of all the posts I've ever made...
<div class="post-list">
    {% for post in site.posts %}
        {% if post.project == null %}
            {% cycle 'add row' : '<div class="row">', nil %}
                <div class="col-md-6  animated fadeIn">
                    <div class="image">
                        <img src="{{ site.url }}/assets/img/placeholder-big.jpg" alt="" />
                        <div class="caption">
                            <h3>{{ post.title }}</h3>
                            <p>{{ post.excerpt }}</p>
                            <a href="{{ site.url }}{{ post.url }}" class="btn zoombtn">Read More</a>
                        </div>
                    </div> 
                </div>
            {% cycle 'end row' : nil, '</div>' %}
        {% endif %}
    {% endfor %}
    {% cycle 'end row' : nil, '</div>' %}
</div>