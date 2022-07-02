---
layout: mainpage
title: /blog
url: /blog
---
## Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

## Experimental Section
<div>
  {% for post in site.posts %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <!-- <p><span>{{ post.date | date: "%Y-%m-%d"}}</span></p> -->
      <p><i>{{ post.date | date: "%Y-%m-%d"}}</i></p>
      <div>
      {{ post.content }}
      </div>
  {% endfor %}
</div>
<!-- <ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul> -->

<!-- <hr>
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %} -->