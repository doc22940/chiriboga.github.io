---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Richard Chiriboga
description: "Richard Chiriboga is a Web Project Manager, Wordpress and Front-End Developer based out of New York City."
---
{% include hp-jumbotron.html %}

{% include section-aboutme.html %}

{% include case-study-featured.html %}
<div class="overlap-container">
  <div class="container">
    <div class="row">
          <div class="col">
              <h3>Latest Blogs</h3>
          </div>
      </div>
      <div class="row row-eq-height">
        {% for post in site.posts limit:3 %}
        <div class="card blog_card m-1 p-0">
              <a href="{{ site.baseurl }}{{ post.url }}">
                  <div class="card-body">
                    {% if post.image %}
                    <img src="{{post.image}}" class="img-fluid rounded" />
                    {% endif %}
                      <h6 class="mt-2 font-weight-bold">{{ post.title }}</h6>
                      <!-- <p>Published: {{ post.date | date: '%B %d, %Y'}}<br/> Category: {{ post.categories }}</p> -->
                  </div>
              </a>
          </div>
        {% endfor %}
      </div>
  </div>
</div>

{% include repositories.html %}

{% include contactform.html %}
