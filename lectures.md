---
title: Lectures
layout: default
---
 * toc
 {:toc}

## numbering convention
Lectures are numbered 01, 02,…  this is roughly aligned with the weeks in the semester, but it isn't a fixed mapping.

The .1, .2, sub-number indicates which of the two lectures the notes are for.

Roughly split into 2 interweaving streams,
 will try to keep step with labs (no promises)

{% for lecture in site.lectures %}
## {{lecture.url|remove:'/lectures/'|remove:'.html'}} {{ lecture.title }}
_{{lecture.lecturer}}_  
<span class="file-link"><a href="{{site.baseurl}}/lectures/{{lecture.file}}">TeX</a>&nbsp;source&nbsp;</span>
&nbsp;
<span class="file-link"><a href="{{site.baseurl}}/lectures/{{lecture.file|replace:".tex",".pdf"}}">PDF</a>&nbsp;slides&nbsp;</span>

{{ lecture.excerpt }}

{% endfor %}
