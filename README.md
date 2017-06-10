## Последние эпизоды

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.file }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

<table>
  <thead>
    <tr>
      <th style="text-align: left">Дата</th>
      <th style="text-align: left">Название</th>
      <th style="text-align: left">Описание</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts %}
    <tr>
      <td style="text-align: left">{{ post.date }}</td>
      <td style="text-align: left"><a href="{{ post.file }}">{{ post.title }}</a></td>
       <td style="text-align: left">{{ post.excerpt }}</td> 
    </tr>
  {% endfor %}
  </tbody>
</table>
