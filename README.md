## Последние эпизоды

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
      <td style="text-align: left">{{ post.date | date_to_string}}</td>
      <td style="text-align: left"><a href="{{ post.file }}">{{ post.title }}</a></td>
       <td style="text-align: left">{{ post.excerpt }}</td> 
    </tr>
  {% endfor %}
  </tbody>
</table>
