---
layout: blog
title: Blog | Richard Chiriboga
description: "My blog about Web Development, Marketing and personal musings."
comments: false
permalink: /blog/
---
<div class="overlap-container">
  <div class="container pt-4">
      <div class="row">
        {% for post in site.posts %}
        <div class="col-lg-6">
              <a href="{{ site.baseurl }}{{ post.url }}" class="card blog_card mb-4">
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