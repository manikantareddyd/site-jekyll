---
layout: index
title: All Posts
excerpt: "A List of Posts"
comments: false
---
<div class="post-list">
    {% for post in site.posts %} 
        {% if post.project == null %}
            
        <div class="col-md-6 wow fadeIn" data-wow-duration="1.5s">
            <div class="image left fit captioned">
                    <img src="{{ site.url }}/assets/img/placeholder-big-b.jpg" alt="" />
                    <div class="caption">
                        <h5>{{ post.title }}</h5>
                        <p>{{ post.excerpt }}</p>
                        <a href="{{ site.url }}{{ post.url }}" class="btn zoombtn">Read More</a>
                    </div>
            </div>
        </div>
           
    </ul>
        {% endif %}
    {% endfor %}
</div>