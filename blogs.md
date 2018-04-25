---
layout: page
title: Blogs
permalink: /blogs/
---

<div class="home">
    {% if site.posts.size > 0 %}
        <h2 class="post-list-heading">{{ page.list_title | default: "Posts" }}</h2>
        {% for post in site.posts %}
        <div class="row yk-post">
            <div class="col">
                <div class="row">
                    <div class="col-md-9">
                        <h4>
                            <a class="post-link" href="{{ post.url | relative_url }}">
                            {{ post.title | escape }}
                            </a>
                        </h4>
                    </div>
                    <div class="col-md-3">
                        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
                        <span class="post-meta float-right">{{ post.date | date: date_format }}</span>
                    </div>
                </div>
                <div class="row">
                    <div class="col-12 mb-2">
                        {% if site.show_excerpts %}
                            {{ post.excerpt | strip_newlines | remove: '<p>' | remove: '</p>' }}
                        {% endif %}
                    </div>
                    <div class="col-12">
                        <a class="post-link" href="{{ post.url | relative_url }}">
                            <button class="btn btn-primary float-right">
                                <strong>Read More...</strong>
                            </button>
                        </a>
                    </div>
                </div>
            </div>
        </div>
        <hr class="yk-post-divider" />
        {% endfor %}
    {% endif %}
</div>