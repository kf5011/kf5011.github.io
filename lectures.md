---
title: Lectures
layout: default
---
## numbering convention
Lectures are numbered 01, 02,…  this is roughly aligned with the weeks in the semester, but it isn't a fixed mapping.

The .1, .2, sub-number indicates which of the two lectures the notes are for.

{% for lecture in site.lectures %}
## {{lecture.url|remove:'/lectures/'|remove:'.html'}} {{ lecture.title }}
<span class="file-link"><a href="https://github.com/kf5011/kf5011.github.io/blob/master/notes/{{lecture.file}}">TeX</a>&nbsp;source&nbsp;</span>
&nbsp;
<span class="file-link"><a href="notes/{{lecture.file|replace:".tex",".pdf"}}">PDF</a>&nbsp;slides&nbsp;</span>

{{ lecture.content }}

{% endfor %}
