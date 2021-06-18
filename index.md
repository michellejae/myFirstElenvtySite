---
title: Welcome to da blog
layout: layout.liquid
pagination: 
    data: collections.blog
    size: 2
    alias: blogs

---
[//]: # "the blog comes from the name of the tag we created in 11tydata.js and the data.title is cause we are grabbing front matter"

{% for blog in blogs %}
- [{{blog.data.title}}]({{blog.url}})
{% endfor %}

You should read it!

{% if pagination.href.previous %}
<a href="{{pagination.href.previous}}">Previous Page</a>
{% endif %}

{% if pagination.href.next %}
<a href="{{pagination.href.next}}">Next Page</a>
{% endif %}
