---
title: News
area: news
layout: default
section: news illustrated
---

## News History

{% for post in site.posts %}
<article>
    <h3 id="latest-news"><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <div class="date">{{ post.date | date: "%B %-d, %Y" }}</div>
    {{ post.content }}
</article>
{% endfor %}
