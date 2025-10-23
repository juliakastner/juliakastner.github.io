---
layout: default
title: Pulications

---

 # Preprints and Unpublished Manuscripts

  {% for item in site.data.preprints %}
  * {{item.authors}} : 

    {{item.title}}. 

    {% if item.fullversion_link %}[PDF]({{item.fullversion_link}}){% endif %}

  {% endfor %}
# Peer-Reviewed Publications

  {% for item in site.data.publications %}
  * {{item.authors}} : 

    {{item.title}}. {{item.proceedings}}

    {% if item.conference_link %} [Published Version]({{item.conference_link}}) {% endif %}{% if item.fullversion_link %}[Full Version]({{item.fullversion_link}}){% endif %}{% if item.video_link %} [Video]({{item.video_link}}) {% endif %}

  {% endfor %}
