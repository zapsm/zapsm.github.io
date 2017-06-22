## Последние эпизоды

<table>
  <thead>
    <tr>
      <th style="text-align: left">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts %}
    <tr>
      <td style="text-align: left">{{ post.date | date: "%d.%m.%Y" }}</td>
      <td style="text-align: left"><a href="{{ site.storage }}/{{ post.file }}">{{ post.title }}</a></td>
       <td style="text-align: left">{{ post.excerpt }}</td> 
    </tr>
  {% endfor %}
  </tbody>
</table>
