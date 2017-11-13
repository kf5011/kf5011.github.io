---
title: seminars
layout: default
---

The seminar sessions form the core of the practical work in this module.  We will be using the FRDM-K64F ARM based platform.  The practical work will have two themes, one based on the MBED libraries and abstractions, the other based on a pure C clean room implementation.
<!--more-->

The MBED libraries are written in C++ and are a generic set of functions that abstract out the behaviour of supported devices.  The device vendor provides an implementation of the routines on their device.

## numbering convention
The seminar sessions are numbered 01, 02,…  this is roughly aligned with the weeks in the semester, but it isn't a fixed mapping.

Within each seminar exercises are numbered 1, 1,… the associated Githib repository is called s1.1 etc.   Question parts an solutions are tagged as releases,


# Getting started
You should study the [Getting started](/getting-started.html) notes to see the workflow that is recommended for the practical work.

<hr />

{::options parse_block_html="true" /}
{% for item in site.seminars %}
<article class="summary">
## {{ item.title }}
[{{ item.url }}]({{ item.url }})
{{ item.excerpt }} [more…]({{item.url}})
</article>
<hr />
{% endfor %}
