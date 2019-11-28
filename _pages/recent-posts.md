---
title: "Recent Posts"
layout: archive
author_profile: true
permalink: /recent/
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/MuizenbergSA_ZH-CN9407386955_1920x1080.jpg
  overlay_filter: 0.1 # same as adding an opacity of 0.5 to a black background
  actions:
    - label: "<i class='fas fa-download'></i> Install now"
      url: "/docs/quick-start-guide/"
excerpt: >
  A flexible two-column Jekyll theme. Perfect for building personal sites, blogs, and portfolios.<br />
  <small><a href="https://github.com/mmistakes/minimal-mistakes/releases/tag/4.17.2">Latest 
---
<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>
{% for post in site.posts limit:10 %}  
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}