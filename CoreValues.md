---
layout: default
title: Core Values
comments: true
---


<!-- We reopen main-content and container -->

<div class="container-fluid">

    <div class="main-content">



        <section class="all-posts">

        <div class="section-title text-center">
            <h1>Core Values and Judging</h1>
        </div>

            <div class="row listfeaturedtag">

            {% for post in site.posts %}

                {% if post.tag == "CoreValues" %}
                    {% unless post.categories contains "draft" %}

                        {% include featuredbox.html %}
                    {% endunless %}
                {% endif %}

            {% endfor %}

            </div>

        </section>
