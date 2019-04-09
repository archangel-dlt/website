---
layout: page
title: Publications
permalink: /publications/
---

{% for pub in site.data.publications %}
  <section class="publication">
    <h3>{{pub.title}}</h3>
    <p>{{pub.authors}}</p>
    <a href="https://doi.org/{{pub.doi}}">{{pub.doi}}</a> | <a href="{{pub.url}}">{{pub.url}}</a>
    <hr/>
  </section>
{% endfor %}
