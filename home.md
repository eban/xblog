<ul>
  {% for post in site.posts limit:10 %}
  <li>
    <a href="{{ post.url | relative_url }}">
      <span> {{ post.date | date: "%F %T" }} </span> {{ post.title }}
    </a>
  </li>
  {% endfor %}
</ul>
