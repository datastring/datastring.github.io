## Latest Posts

<div>
  {% for post in site.posts %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <!-- <p><span>{{ post.date | date: "%Y-%m-%d"}}</span></p> -->
      <!-- <p><i>Posted on {{ post.date | date: "%Y-%m-%d"}}</i></p> -->
	  <p><span><i>Posted on {{ post.date | date: "%Y-%m-%d"}}</i></span></p>
      <div>
      {{ post.content | truncatewords: 100 }}
      </div>
  {% endfor %}
</div>

<!-- <ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul> -->
