---
layout: page
title: Events

meetup_events: true
---

<ul>
  {% for event in site.data.event-types %}
    <li>
      <ul>
        <li>Type: {{ event.type }}</li>
        <li>Description: {{ event.description }}</li>
      </ul>
    </li>
  {% endfor %}
</ul>

<section id="meetup-events" class="container-fluid">
    <meetup-events
        id="events"
        max-events="5">
    </meetup-events>
</section>
