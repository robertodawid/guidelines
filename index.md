---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% assign mydocs = site.docs | group_by: 'category' %}
{% for cat in mydocs %}
<h2>{{ cat.name | capitalize }}</h2>
    <ul>
      {% assign items = cat.items | sort: 'order' %}
      {% for item in items %}
        <li><a href="{{ item.url }}">{{ item.title }}</a></li>
      {% endfor %}
    </ul>
{% endfor %}