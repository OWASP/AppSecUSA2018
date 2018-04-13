---
image: images-049.jpg
layout: multisection
title: Keynote speakers
---
<section class="image huge" style="background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI4MDAiIGhlaWdodD0iMTAwIiB2aWV3Qm94PSIwIDAgODAwIDEwMCIgdmVyc2lvbj0iMS4xIj4KICA8cmVjdCB3aWR0aD0iODAwIiBoZWlnaHQ9IjEwMCIgZmlsbD0iIzBlYjliMCIgc3R5bGU9Im9wYWNpdHk6IDAuNzciIC8+Cjwvc3ZnPg==), url(/assets/images/images-049.jpg), url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNTgyIDE3MjEiPjxmaWx0ZXIgaWQ9ImIiPjxmZUdhdXNzaWFuQmx1ciBzdGREZXZpYXRpb249IjEyIiAvPjwvZmlsdGVyPjxwYXRoIGZpbGw9IiM2NjYiIGQ9Ik0wIDBoMjU4MnYxNzE0SDB6Ii8+PGcgZmlsdGVyPSJ1cmwoI2IpIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSg1IDUpIHNjYWxlKDEwLjA4NTk0KSIgZmlsbC1vcGFjaXR5PSIuNSI+PGVsbGlwc2Ugcng9IjEiIHJ5PSIxIiB0cmFuc2Zvcm09InJvdGF0ZSgtMjAuOCA0NjQuMyAtMTgwKSBzY2FsZSgyNy42NjcwNyA5Mi40NTM2OSkiLz48ZWxsaXBzZSBjeD0iMjQzIiBjeT0iMTQxIiByeD0iMjkiIHJ5PSIzNiIvPjxwYXRoIGZpbGw9IiNiNGI0YjQiIGQ9Ik0yMzkgMTExTDg3IDEyMiAyNzEtMTZ6Ii8+PGVsbGlwc2UgZmlsbD0iI2Q4ZDhkOCIgcng9IjEiIHJ5PSIxIiB0cmFuc2Zvcm09Im1hdHJpeCgyLjQ5NTAyIC03MS40NDgxIDE0Ljk4Mzc3IC41MjMyNCAxMDMuOCAyNS4zKSIvPjxlbGxpcHNlIGZpbGw9IiNhZmFmYWYiIHJ4PSIxIiByeT0iMSIgdHJhbnNmb3JtPSJtYXRyaXgoMTMuOTc4OSAxMDYuMTgwMyAtMTQuODkxNDggMS45NjA1IDMyLjEgNDkuNCkiLz48ZWxsaXBzZSBmaWxsPSIjZmZmIiByeD0iMSIgcnk9IjEiIHRyYW5zZm9ybT0ibWF0cml4KC0uMjYzOTYgLTUuMzk3MSAzMy4wOTQxOCAtMS42MTg1OCAxNjMuNiAxNTcuOCkiLz48ZWxsaXBzZSBmaWxsPSIjMWMxYzFjIiBjeT0iNjUiIHJ4PSIyMCIgcnk9Ijc4Ii8+PHBhdGggZD0iTTExOC4zIDE0MC4ybC02MyA0OS4yLTIxLjYtMjcuNiA2My00OS4yeiIvPjwvZz48L3N2Zz4=);">

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
