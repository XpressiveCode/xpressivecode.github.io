---
layout: page
title: writing expressive code
tagline: one line at a time
---
{% include JB/setup %}
<div class="blog-index">
    {% for post in site.posts limit: 5 %}
        <article class="post">
          <h2 class="post-title well">
              <a href="{{ post.url }}" title="{{ post.title }}">
                  {{ post.title }}
              </a>

              <small class="date">
                <span><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%B %d, %Y' }}</time></span>
              </small>
          </h2>
          <section class="post">
            {{ post.excerpt }}
          </section>
          <a class="btn-link" href="{{ post.url }}" title="{{ post.title }}">Read More</a>
        </article>
    {% endfor %}
</div>
