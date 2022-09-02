---
layout: post
title:  "My First Draft"
date:   2022-09-01 11:54:01 -0700
categories: jekyll update
tag: Jekyll Doc
---




<p>Here are some of my posts</p>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
         {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

{% assign verb = "turned" %}
{% comment %}
{% assign verb = "converted" %}
{% endcomment %}
Anything you put between {% comment %} and {% endcomment %} tags
is {{ verb }} into a comment.