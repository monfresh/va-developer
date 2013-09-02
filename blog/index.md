---
layout: default
title: "PIF @ VA"
published: true
---

# PIF @ VA

{% for post in site.posts limit:5000 %}

## [{{ post.title }}](/veterans-affairs{{ post.url }})

{{ post.date | date:"%m-%d-%Y" }}

<img src="{{ post.image }}" width="100" align="right" style="padding: 20px;" />
{{ post.content | strip_html | truncatewords: 200     }}...[View Full Blog Post](/veterans-affairs{{ post.url }})    

- - -
{% endfor %}