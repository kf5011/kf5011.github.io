---
title: Lectures
layout: default
---

{% for lecture in site.lectures %}
## {{lecture.url|remove:'/lectures/'|remove:'.html'}} {{ lecture.title }}
<span class="file-link"><a href="https://github.com/kf5011/kf5011.github.io/blob/master/notes/{{lecture.file}}">TeX</a>&nbsp;source&nbsp;</span>
&nbsp;
<span class="file-link"><a href="notes/{{lecture.file|replace:".tex",".pdf"}}">PDF</a>&nbsp;slides&nbsp;</span>

{{ lecture.excerpt }}

{% endfor %}
