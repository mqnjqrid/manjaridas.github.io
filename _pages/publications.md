---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications %}
  {% if post.paperurl <> "ongoing" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

Ongoing
======

{% include base_path %}

{% for post in site.ongoingresearch %}
  {% if post.paperurl == "ongoing" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
