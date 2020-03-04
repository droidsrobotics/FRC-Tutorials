---
layout: default
title: Coach's Corner
comments: true
---


<!-- We reopen main-content and container -->

<div class="container-fluid">

    <div class="main-content">

        <section class="all-posts">

            <div class="section-title">
                <h2><span>Tips from Coaches and Mentors</span></h2>
            </div>

            <div class="row listfeaturedtag">

            {% for post in site.posts %}

                {% if post.tag == "CoachCorner" %}
                    {% unless post.categories contains "draft" %}

                        {% include featuredbox.html %}
                    {% endunless %}
                {% endif %}

            {% endfor %}

            </div>

        </section>
