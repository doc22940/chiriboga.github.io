---
layout: blog
title: Blog | Richard Chiriboga
description: "My blog about Web Development, Marketing and personal musings."
comments: false
permalink: /blog/
---
<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      <div class="entry">
        <p><strong>Published:</strong> {{ post.date | date: '%B %d, %Y'}} | <strong>Category:</strong> {{ post.categories }}</p>
      </div>
    </article>
    <hr/>
  {% endfor %}
</div>