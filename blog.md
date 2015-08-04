---
layout: blog-list
title: 新闻动态
permalink: /blog/

header: 2013-2015，见证闪孵的成长
---

<div class="row">
  <div class="col-md-8 post-list">
  	<div class="normal-box ">
  		<div class="box-title">
  			<h2><span>文章列表</span></h2>
  		</div>
  		<ul class="">
		  	{% for post in site.posts %}
				<li class="">
					<a href="{{ post.url }}">{{ post.title }}</a>
					<span class="publish-date">{{ post.date | date_to_string }}</span>
				</li>
		  	{% endfor %}
	  	</ul>
  	</div>

  	<!-- <ul class="post-list">
  		{% for post in site.posts %}
	  		<li class="normal-box">
	  			<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	  			<div class="post-meta">
	  				<span class="author">{{ post.author }}</span>
	  				<span class="date">· {{ post.date | date_to_string }}</span>
	  			</div>
	  			<div class="post-content">{{ post.summary }}</div>
	  		</li>
  		{% endfor %}
  	</ul> -->
  </div>
  <div class="col-md-4">
  	<div class="normal-box posts-category">
  		<div class="box-title">
  			<h2><span>分类</span></h2>
  		</div>
		<ul>
			{% for category in site.categories %}
				<li>
					<a href="{{ cat.url }}">{{ category | first }}</a>
				</li>
			{% endfor%}
		</ul>
  	</div>
  </div>
</div>