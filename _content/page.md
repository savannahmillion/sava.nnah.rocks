---
title: Hey
_template: default
emoji: {{ homepage}}assets/img/home.png
emoji-animation: wave
div-class: center
circle-style: purple-circle-outline
---

Hello, my name is Savannah Million and I'm an interaction designer living and working in Chicago. Some of my work is featured below.

<div class="project center">
	{{ entries:listing folder="projects" }}
		<a href="{{ url }}"><img class="project-feed-thumb" src="{{ feed-thumbnail }}"></a>
		<h2><a href="{{ url }}">{{ title }}</a></h2>
		<p>{{ project-description }}</p>
	{{ /entries:listing }}

	<br/>I will be posting more projects soon. &hearts;
</div>