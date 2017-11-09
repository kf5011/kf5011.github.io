---
title: seminars
layout: default
---
{% for item in site.seminars %}
## {{ item.title }} 
[{{ item.url }}]({{ item.url }})
{{ item.excerpt }}
<hr />
{% endfor %}
