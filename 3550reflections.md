---
layout: page
title: "COMP3550 Learning Portfolio" 
---

This is the page for my COMP3100/COMP3500/COMP3550 TechLauncher Learning Portfolio at ANU.  These posts are in reverse-chronological order, since I haven't yet worked out a trick to change that in Jekyll.  Eventually I'll get them the right way round!

{% for post in site.posts %}
	{% if post.resource == true %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}
{% endfor %}
