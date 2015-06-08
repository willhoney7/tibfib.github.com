---
layout: page
title: Projects
tagline: 
---


<div>  	
	{% for page in site.pages %}
	  	{% if page.project %}
			<a class="block" href="{{ BASE_PATH }}{{ page.url }}">
				<div class="well">
					<div class="hidden-phone pull-left">
						<img class="block-icon" src='{{ site.ASSET_PATH }}{{ page.icon }}'/>
					</div>
					<div >
						<h2>{{ page.title }} <small>{{ page.tagline }}</small></h2>
						<p>{{ page.description }}</p>
					</div>
				</div>
			</a>
		{% endif %}
	{% endfor %}
</div>

<div class="page-header">
<h1>Contributions</h1>
</div>

{% for page in site.pages %}
  	{% if page.contribution %}
<div class="block block-small">
	<div class="well well-small">
		<h2>{{ page.title }} <small>{{ page.tagline }}</small></h2>
		<div>
			<img class="pull-left pad-right" src='{{ site.ASSET_PATH }}{{ page.icon }}'/>
			{{ page.content }}
		</div>
	</div>
</div>
	{% endif %}
{% endfor %}
