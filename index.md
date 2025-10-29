---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
top_imge: https://upload.wikimedia.org/wikipedia/commons/9/94/Wide_brown_land_art-work.JPG
---
<div style="text-align:center;">
  <img src="{{ site.baseurl }}/assets/corfu.jpg" alt="" style="max-width:80%; height:auto;">
</div>

<h2>📚 Πρόσφατα άρθρα</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <br>
      <small>{{ post.date | date: "%d/%m/%Y" }}</small>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
