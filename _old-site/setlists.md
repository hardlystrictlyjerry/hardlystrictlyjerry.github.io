---
layout: page
permalink: /setlists
---


<h1><img class="ui avatar image" src="/images/jerryavatar.jpg">HSJ Setlists</h1>

As of December 2019: 28 Jams, 112 songs, 347 attempts

The column label is a link to the page associated with that setlist.

<table>
  <thead>
    <tr>
      <th></th>
      {% for header in site.data.setlists.headers %}
      <th> <a href="{{ header.url }}">{{ header.label }}</a> </th>
      {% endfor %}
    </tr>
  </thead>
  <tbody>
    {% for songdata in site.data.setlists.songs %}
      <tr>
        {% for data in songdata %}
          <td>{{ data }}</td>
        {% endfor %}
      </tr>
    {% endfor %}
  </tbody>
</table>





