---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Blog | Richard Chiriboga
description: "My blog about Web Development, Marketing and personal musings."
---
<section id="blog">
  <div class="container">
    <div class="row">
      <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1 col-sm-12 col-xs-12">
        <div class="posts">
          {% for post in site.posts %}
            <article class="post">
              <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
              <div class="entry">
                {{ post.excerpt }}
              </div>
              <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
            </article>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</section>
