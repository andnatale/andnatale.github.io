---
layout: default
title: Publications
---


## Journal Articles and Preprints

<ol style="list-style: none; padding-left: 0; margin: 0;">
{% for pub in site.data.publications %}
  <li style="display: grid; grid-template-columns: auto 1fr; gap: 0.5em; margin-bottom: 1.2em; text-align: justify;">
    <span>[{{ forloop.index }}]</span>
    <span>
      {{ pub.authors }} ({{ pub.year }}), <strong>{{ pub.title }}</strong>{% if pub.journal %}, {{ pub.journal }}{% endif %}{% if pub.volume %}, vol. {{ pub.volume }}{% endif %}{% if pub.number %}({{ pub.number }}){% endif %}{% if pub.pages %}, pp. {{ pub.pages }}{% endif %}.{% if pub.publisher %} {{ pub.publisher }}.{% endif %}
      
      {% if pub.hal_id %}
        <a href="https://hal.archives-ouvertes.fr/{{ pub.hal_id }}">[HAL]</a>
      {% endif %}
      {% if pub.arxiv_id %}
        <a href="https://arxiv.org/abs/{{ pub.arxiv_id }}">[arXiv]</a>
      {% endif %}
      {% if pub.doi %}
        <a href="https://doi.org/{{ pub.doi }}">[DOI]</a>
      {% endif %}
    </span>
  </li>
{% endfor %}
</ol>



## Thesis

The full manuscript of my PhD thesis can be found <a href="https://spiral.imperial.ac.uk:8443/bitstream/10044/1/60687/1/Natale-A-2017-PhD-Thesis.pdf"> here</a>.
