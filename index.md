---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title:  KF5011 Computer Networks and Control Systems
---


 * [Reading list]({{site.baseurl}}{%link books.md%})
 * [Development Software]({{site.baseurl}}{%link platform.md%})
 * [Course structure and content]({{site.baseurl}}{%link structure.md%})
 * [Hardware]({{site.baseurl}}{%link hardware.md%})
 * [Assessment]({{site.baseurl}}{%link assessment.md%})

 * [Getting Started]({{site.baseurl}}{%link getting-started.md%})

The organisation [https://github.com/KF5011](https://github.com/KF5011) has several example projects that have been built for the system under consideration.

[Module descriptor]({{site.baseurl}}{%link KF5011.2016.pdf%})

If you're interested I've distilled the [results]({{site.baseurl}}{%link survey.md%}) of the module satisfaction survey for the last (2016/17) run of small embedded systems  

# Some initial notes that may become lectures.
{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }}) {{ repository.project_tagline }}
{% endfor %}
