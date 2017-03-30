---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

test
{% for post in paginator.posts %}
  {% if post.toc %}
    {{ post.content | toc }}
  {% else %}
    {{ post.content }}
  {% endif %}
{% endfor %}
test