---
layout: post
title:  "My first Jekyll post!"
date:   2020-12-29 015:59:10 +0100
categories: jekyll update
tags: goodbye cruel world
---

I've spent the last few weeks at my in-laws' place. They've had some more time to bond with their new granddaughter, we've had a little more free time as a result - Everybody wins.

I will leave the default Jekyll post untouched until I am a little more familiar with all of this.

Getting this site up before the end of the year would be great, looks like that's a realistic goal.

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}