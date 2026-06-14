---
layout:  page
title: ""
---


I am a post-doc researcher at UCL. My research focus on understanding how people integrate information during social decision making, and the neural mechanisms underlying these processes. In particular, I am interested in how individuals perceive the sense of self and navigate group dynamics in complex social contexts, as well as how these processes may be altered in mental health conditions.

To address these questions, I combine computational modelling of behaviour with neuroimaging and neuromodulation approaches, including M/EEG, fMRI, and brain stimulation techniques.


This website is currently under construction — more information about my research and work will be coming soon. 



{% if site.show_excerpts %}
  {% for post in site.posts %}
    <article>
      {% include meta.html post=post %}
      {{ post.excerpt }}
      <footer class="button"><a href="{{ post.url | relative_url }}">read more</a></footer>
    </article>
  {% endfor %}
{% else %}
  {% capture source %}{% include_relative archive.html title="Posts" %}{% endcapture %}
  {{ source | split: "---" | last }}
{% endif %}
