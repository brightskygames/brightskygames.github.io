<p>
{% if page.ios_link %}
<a href="{{ page.ios_link }}" onclick="ga('send', 'event', 'Link', 'click', '{{ page.ref }}_i');">
  <img src="{{ site.url }}/assets/img/dl_app_store_badge_135x40.png" alt="Download on the AppStore">
</a>
{% endif %}
{% if page.and_link %}
<a href="{{ page.and_link }}" onclick="ga('send', 'event', 'Link', 'click', '{{ page.ref }}_a');">
  <img src="{{ site.url }}/assets/img/google_play_badge.png" alt="Get it on Google Play">
</a>
{% endif %}
</p>
