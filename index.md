---
layout: page
title: writing expressive code
tagline: one line at a time
---
{% include JB/setup %}
<div class="blog-index">
    {% for post in site.posts limit: 5 %}
        <h2>
            <a href="{{ post.url }}" title="{{ post.title }}">
                {{ post.title }}
            </a>
            <small>{{ post.date | date_to_string }}</small>
        </h2>
        {{ post.excerpt }}
    {% endfor %}
</div>
