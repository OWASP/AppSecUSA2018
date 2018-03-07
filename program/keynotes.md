---
image: images-049.jpg
layout: multisection
title: Keynote speakers
---
<section class="image huge" style="background-image: url(/assets/images/simpleback.svg), url(/assets/images/images-049.jpg);">

</section>

<section class="inverse">
<h2>{{page.title}}</h2>
</section>

<section>
<div class="keynote-full">
	<ul>
	{% for member in site.data.keynotespeakers %}
		{% if member.name %}
		<li>
			<div class="image" style="background-image: url(/assets/images/keynotes/{{member.image | default: '../placeholder.svg'}});{{member.style}};"></div>
			<div>
				<h1>{{member.name}}</h1>
				{% if member.uri %}
					<h3><a href="{{member.uri}}">{{member.title}}</a></h3>
				{% else %}
					<h3>{{member.title}}</h3> 
				{% endif %}
				<p>
					{{member.description}}
				</p>
			</div>
		</li>
		{% endif %}
	{% endfor %}
	</ul>
</div>
</section>