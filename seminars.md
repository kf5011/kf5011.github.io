---
title: seminars
layout: default
---
{::options parse_block_html="true" /}
{% for item in site.seminars %}
<article class="summary">
## {{ item.title }}
[{{ item.url }}]({{ item.url }})
{{ item.excerpt }} [more…]({{item.url}})
</article>
<hr />
{% endfor %}
