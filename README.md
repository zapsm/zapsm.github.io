## Последние эпизоды

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.file }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
