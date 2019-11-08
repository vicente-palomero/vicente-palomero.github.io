<h1>En qué ando ahora</h1>
<ul>
  {% for item in site.data.interests %}
    <li>{% if item.link %}<a href="{{ item.link }}">{% endif %}{{ item.name | downcase }}{% if item.link %}</a>{% endif %}: {{ item.desc }}</li>
  {% endfor %}
</ul>
