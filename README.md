## Последние эпизоды

<table>
  <thead>
    <tr>
      <th style="text-align: center">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
      <th style="text-align: left">&nbsp;</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts %}
    <tr>
      <td style="text-align: сenter">
	{{ post.date | date: "%d.%m.%Y" }}
      </td>
      <td style="text-align: left">
      	<strong>{{ post.title }}</strong>
	{{ post.excerpt }}
      </td>
      <td style="text-align: left"><i class="material-icons"><a href="{{ site.storage }}/{{ post.file | append: '.mp3'}}">audiotrack</a></i></td>
      {% if post.youtube %}
      <td style="text-align: left"><i class="material-icons"><a href="{{ site.storage }}/{{ post.file | append: '.360.mp4'}}">ondemand_video</a></i></td> 
      <td style="text-align: left"><i class="material-icons"><a href="{{ site.storage }}/{{ post.file | append: '.720.mp4'}}">hd</a></i></td>
      {% else %}
      <td style="text-align: сenter">&nbsp;</td>
      <td style="text-align: сenter">&nbsp;</td>
      {% endif %}
    </tr>
  {% endfor %}
  </tbody>
</table>
