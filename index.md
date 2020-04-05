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
      <div class="row">
        {% for post in site.posts limit:2 %}
        <div class="col-lg-6">
              <a href="{{ site.baseurl }}{{ post.url }}" class="card blog_card">
                  <div class="card-body">
                      <img src="{{post.image}}" class="img-fluid rounded" />
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
