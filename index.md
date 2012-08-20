---
layout: default
title: Blog
tagline:
---
{% include JB/setup %}

<div class="row-fluid">
		
	<div class="span8">
		{% for post in site.posts %}
			<blockquote>
				<h1><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h1>
				<h6 class="date">{{ post.date | date_to_string}}</h6>
				<p>{{ post.content }}</p>
			</blockquote>
		{% endfor %}
	  
	</div><!--/span-->
	<div class="span4">
		<h1 class="muted">Projects</h1>
			{% for page in site.pages %}
			  	{% if page.project %}
			  	<a class="project {{ page.class }}" href="{{ BASE_PATH }}{{ page.url }}">
					<img class='project-icon' src='{{ ASSET_PATH }}{{ page.icon }}'/>
					<div class='project-text' >
						{{ page.title}}
					</div>
				</a>  
				{% endif %}
			{% endfor %}
			
    </div><!--/span-->
</div><!--/row-->

<!--This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

	$ rm -rf _posts/core-samples

Here's a sample "posts list".-->

