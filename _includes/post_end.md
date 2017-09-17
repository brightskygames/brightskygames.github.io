<p>
{% assign arApps = site.mobile_app | where: "ref", page.ref %}
{% if arApps.size > 0 %}{% assign app = arApps[0] %}
	{% if app.ios_link %}
	<a href="{{ app.ios_link }}" onclick="ga('send', 'event', 'Link', 'click', '{{ page.ref }}_i');">
	  <img src="{{ site.url }}/assets/img/dl_app_store_badge_135x40.png" alt="Download on the AppStore">
	</a>
	{% endif %}
	{% if app.and_link %}
	<a href="{{ app.and_link }}" onclick="ga('send', 'event', 'Link', 'click', '{{ page.ref }}_a');">
	  <img src="{{ site.url }}/assets/img/google_play_badge.png" alt="Get it on Google Play">
	</a>
	{% endif %}
{% endif %}
</p>
