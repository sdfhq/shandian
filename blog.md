---
layout: blog-list
title: 新闻动态
permalink: /blog/

header: 2013-2015，见证闪孵的成长
cover: shandian-blog.jpg
---

<div class="cbox title-box">
	<div class="box-title">
		<h2>
			文章列表
		</h2>
	</div>
	
	<ul class="">
	  	{% for post in site.posts %}
			<li class="">
				<span class="publish-date">{{ post.date | date: "%Y-%m-%d" }}</span>
				<a href="{{ post.url }}">{{ post.title }}</a>
			</li>
	  	{% endfor %}
	</ul>
</div>