---
layout: default
title: Pulications

---
# Publications

  {% for item in site.data.publications %}
     * {{item.authors}} : 
       {{item.title}}. {{item.proceedings}}
       [Published Version]({{item.conference_link}}) [Full Version]({{item.fullversion_link}}) [Video]({{item.video_link}}) 

  {% endfor %}
