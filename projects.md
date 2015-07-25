---
layout: default
title: Projects
permalink: /projects/
navbar: true
---

<div class="page-header">
	<h1>Websites</h1>
</div>

<div class="projects">
	<div class="row">
		<div class="col-md-12">
			{% for project in site.data.projects %}
				{% if project.type == "website" %}
					<a class="block {{project.class}}" target="_blank" href="{{project.url}}">
						<div class="well well-sm">
							<div class="block-icon pull-left"></div>
							<div class="block-content">
								<h2>{{ project.title }} <small>{{ project.tagline }}</small></h2>
								<p>{{ project.description }}</p>
							</div>
						</div>
					</a>
				{% endif %}
			{% endfor %}
		</div>
	</div>


	<h1>Applications</h1>
	<hr/>

	<div class="row">
		<div class="col-md-12">
			{% for project in site.data.projects %}
				{% if project.type == "application" %}
					<a class="block {{project.class}}" href="{{ project.url }}">
						<div class="well well-sm">
							<div class="block-icon pull-left"></div>
							<div class="block-content">
								<h2>{{ project.title }} <small>{{ project.tagline }}</small></h2>
								<p>{{ project.description }}</p>
							</div>
						</div>
					</a>
				{% endif %}
			{% endfor %}
		</div>
	</div>


	<h1>Contributions</h1>
	<hr/>

	<div class="row">
		<div class="col-md-12">
			{% for project in site.data.projects %}
				{% if project.type == "contribution" %}
					<div class="block {{project.class}}">
						<div class="well well-sm">
							<div class="block-icon pull-left"></div>
							<div class="block-content">
								<h2>{{ project.title }} <small>{{ project.tagline }}</small></h2>
								<p>{{project.description}}</p>
							</div>
						</div>
					</div>
				{% endif %}
			{% endfor %}
		</div>
	</div>
</div>
