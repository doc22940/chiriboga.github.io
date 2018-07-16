---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Richard Chiriboga
description: "Richard Chiriboga is a Technical Manager, Wordpress and Front-End Developer based out of New York City."
---
<div class="jumbotron">
  <div class="container text-center">
    <h1>Hi, my name is Rich and I am a <span>Technical Project Manager</span> &amp; <span>Front-End Developer</span> living in New York City.</h1>
  </div>
</div>




<section class="subtron resume">
  <div class="container">
    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12 col-xs-12 text-center">
        <p><a class="btn btn-info btn-lg btn-rc" href="/resume/Richard.Chiriboga.Resume.pdf" target="_blank"><strong>View my resume</strong></a></p>
      </div>
    </div>
  </div>
</section>
<section id="aboutme">
  <div class="container">
    <div class="row">
      <div class="col-lg-5 col-md-4 col-sm-3 col-xs-12">
        <img class="img-responsive img-circle center-block" src="img/richard-chiriboga-250.jpg" alt="Richard Chiriboga">
      </div>
      <div class="col-lg-7 col-md-8 col-sm-9 col-xs-12 bio">
          <h2>About Me</h2>
          <p>Web Project Manager and front-end developer with extensive experience working across global corporate, non-profit and boutique agency environments. Expertise in leading website restructuring, development projects, corporate intranet builds and content management plans through the complete lifecycle. Known for being a trusted partner across  global matrixed organizations and having the ability to communicate complex information to both technical and non-technical users,  including information pertaining to change management, stakeholder engagement and governance. Hispanic marketing and social media expertise: Created award-winning website CorrienteLatina.com. Fluent in English, with intermediate Spanish fluency.</p>
      </div>
    </div>
  </div>
</section>


{% include case-study-featured.html %}

<section class="bt">
  <div class="container">
    <div class="row">
      <div class="col-lg-12 col-md-12 col-sm-12 col-xs-12">
        <h2><a href="/blog/">Latest Blogs</a></h2>
      </div>
    </div>
    <div class="row">
      {% for post in site.posts limit:3 %}
        <div class="col-lg-4 col-md-4 col-sm-4 col-xs-12">
          <div class="blog-box">
            <a href="{{ site.baseurl }}{{ post.url }}" class="well well-sm {{ post.categories }}">
              <h4>{{ post.title }}</h4>
              <div class="entry">
                <p>Published: {{ post.date | date: '%B %d, %Y'}}<br/> Category: {{ post.categories }}</p>
              </div>
            </a>
          </div>
        </div>
      {% endfor %}
    </div>
  </div>
</section>


{% include repositories.html %}


{% include contactform.html %}