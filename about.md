---
layout: default
title: About
tagline: 
---

<div class="row">

<div class="span8">
	<div class="page-header">
	  <h1>{{ page.title }} {% if page.tagline %} <small>{{ page.tagline }}</small>{% endif %}</h1>
	</div>

	<p>
		Hey, my name is Will Honey, and I'm a developer!<br/><br/> 
		I started coding with Palm's webOS and have been involved with many projects for that platform. Lately, I've been branching out to other mobile platforms and the web.<br/><br/>
		I'm also a student at Brigham Young University studying Computer Science.<br/><br/>
		If you have any project ideas or jobs, I'd love to hear them.<br/><br/>
		<h4>About the Site</h4>
		This site was built using <a href="https://github.com/mojombo/jekyll">Jekyll</a>, <a href="http://jekyllbootstrap.com/">Jekyll Bootstrap</a>, and <a href="http://twitter.github.com/bootstrap/">Bootstrap</a>. Analytics are provided by <a href="http://getclicky.com">GetClicky.com</a>. The site is hosted by <a href="http://pages.github.com">Github Pages</a>.
	</p>
</div>

<div class="span4">
	<h1 class="muted">More</h1>
	<ul class="nav">
		<li>
			<a class="block" href="mailto:{{ site.author.email }}" target="_blank">
				<div class="well well-small">
					<img class="social-icon" src="{{ site.ASSET_PATH }}images/email.png" /><span class="more-label"><strong>Email</strong> <span class="muted">at will@tibfib.com</span></span>
				</div>
			</a>
		</li>
		<li>
			<a class="block" href="http://github.com/{{ site.author.github }}" target="_blank">
				<div class="well well-small">
					<img class="social-icon" src="{{ site.ASSET_PATH }}images/github.png" /><span class="more-label"><strong>Github</strong> <span class="muted">as Tibfib</span></span>
				</div>
			</a>
		</li>
		<li>
			<a class="block" href="http://twitter.com/{{ site.author.twitter }}" target="_blank" title="@{{ site.author.twitter }}">
				<div class="well well-small">
					<img class="social-icon" src="{{ site.ASSET_PATH }}images/twitter.png" /><span class="more-label"><strong>Twitter</strong> <span class="muted">as @Tibfib</span></span>
				</div>
			</a>
		</li>
		<li>
			<a class="block" href="{{ BASE_PATH }}atom.xml" target="_blank">
				<div class="well well-small">
					<img class="social-icon" src="{{ site.ASSET_PATH }}images/rss.png" /><span class="more-label"><strong>RSS</strong> <span class="muted">for tibfib.com</span></span>
				</div>
			</a>
		</li>
	</ul>	
</div>

</div>