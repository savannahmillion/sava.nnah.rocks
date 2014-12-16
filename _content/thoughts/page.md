---
title: thoughts
_template: default
emoji: {{ homepage}}assets/img/thoughts.png
emoji-animation: flex
div-class: center
circle-style: purple-circle-outline
---

This is the blog part of my website. Some of these articles will be rambly feelings, some of them will be useful tutorials, and some of them will be write ups on projects. 

<div class="project center">
	{{ entries:listing folder="thoughts" }}
		<div class="blog-feed-divider center"></div>
		<h2><a href="{{ url }}">{{ title }}</a></h2>
		<p class="blog-data">{{ date }}</p>
	{{ /entries:listing }}
</div>