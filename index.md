---
title: Page d'accueil
description: Index du site statique
---

# Découvrir les GSS avec Paris Web 2017

GSS = Générateur de sites statiques

{{ site.title }}


<h1>{{page.title}}</h1>

## menu
<ul>
	{% for page in site.pages %}
	 <li><a href="{{ page.name }}">{{ page.title }}</a></li>
	{% endfor %}
</ul>

## Articles
<ul>
	{% for post in site.posts %}
		<li><a href="{{ post.title }}">{{ post.title }}</a></li>
	{% endfor %}
</ul>