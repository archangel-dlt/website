---
layout: page
title: People
permalink: /people/
---

{% for group in site.data.people %}
  <section>
    <h3><u>{{group.name}}</u></h3>
    {% for person in group.people %}
    <div class="profile">
      <img src="{{ site.baseurl }}/assets/images/people/{{person.image}}" />
      <div>
        <h4>{{person.name}}</h4>
        <p>{{person.position}}</p>
      </div>
    </div>
    {% endfor %}
  </section>
{% endfor %}
