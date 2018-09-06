---
title: Sponsoring the Career Fair
layout: multisection
---

<section markdown="1">
# Sponsoring the Career Fair

The AppSecUSA 2018 Career Fair is open to any company who is looking to hire new talent. The Career Fair will run for 2 hours during the first primary day of the session portion of the conference, Thursday, October 11th 2pm-4pm.

See the [Career sponsorship flyer](https://2018.appsecusa.org/docs/AppSecUSA_2018_CareerFair_Flyer_V01.pdf)
</section>

<section class="sponsors">
	<h3>Participants</h3>
  <div>
	{% for participant in site.data.careerfair.participants %}
    <a style="background-image: url(/assets/images/careerfair/{{participant.logo}});{% if participant.backgroundSize %}background-size: {{participant.backgroundSize}};{% endif %}" title="{{participant.name}}" href="{{participant.url}}"></a>
  {% endfor %}
  </div>
</section>