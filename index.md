---
layout: default
---

# MY OUTREACHY BLOG

Welcome! This is my personal outreachy blog.  
More posts coming soon!

## Recent Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

