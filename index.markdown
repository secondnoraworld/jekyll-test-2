---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{% assign articles = site.articles | sort: 'order' | reverse %}
{% for article in articles %}
  <h3><a href="{{ article.url }}">{{ article.title }}</a></h3>
{% endfor %}
