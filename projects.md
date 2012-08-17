---
layout: page
title: Projects
tagline: 
---
{% include JB/setup %}

{% for page in site.pages %}
  	{% if page.project %}
<a class="well-project" href="{{ BASE_PATH }}{{ page.url }}">
	<div class="well">
			<div class="pull-left">
				<img class="well-project-icon" src='{{ ASSET_PATH }}{{ page.icon }}'/>
			</div>
			<div >
				<h2>{{ page.title }} <small>{{ page.tagline }}</small></h2>
				<p>{{ page.description }}</p>
			</div>
	</div>
</a>
	{% endif %}
{% endfor %}

<div class="page-header">
<h1>Contributions</h1>
</div>

{% for page in site.pages %}
  	{% if page.contribution %}
<div class="well-project well-contribution">
	<div class="well well-small">
		<div data-toggle="collapse" data-target="#{{ page.id }}">
			<h2>{{ page.title }} <small>{{ page.tagline }}</small></h2>
		</div>
		<div class="collapse out" id="{{ page.id }}">{{ page.content }}</div>
	</div>
</div>
	{% endif %}
{% endfor %}



