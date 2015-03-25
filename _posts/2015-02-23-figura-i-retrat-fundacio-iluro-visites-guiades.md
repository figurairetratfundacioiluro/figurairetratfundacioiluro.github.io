---
layout: post
og: true
og-type: article
title: "Visites guiades" 
share: true
class: event
categories:
  - visites
published: true
work: 3
email: "ateneu@fundacioiluro.cat"
---

{% assign work_data = site.data.visites.adults | where:"id", page.work %}
{% assign work = work_data | first %}
<figure class="no-margin margin-bottom-1">
    <div class="embed-container embed-container_{{ work.aspect_ratio }}">
      <core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image> 
    </div>
    <div class="padding-artwork-container" itemscope itemtype="http://schema.org/Event">
        <h3><span itemprop="name">{{ work.category }}</span></h3>
        <strong>Durada:</strong> {{ work.duration }}<br/>
        <meta itemprop="startDate" content="{{ work.startDate }}">
        <div itemprop="location" itemscope itemtype="http://schema.org/Place">
          <strong>Lloc:</strong> {{ work.place }}
          <div itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
            <strong>Adreça:</strong> <span itemprop="streetAddress">{{ work.streetAddress }}</span> <span itemprop="postalCode">{{ work.postalCode }}</span>, <span itemprop="addressLocality">{{ work.addressLocality }}</span>
          </div>
        </div>
        <strong>Dates:</strong><br/>
        <strong>Dissabte:</strong> {{ work.timetable.saturday }}<br/>
        <strong>Dijous:</strong> {{ work.timetable.thursday }}
        <hr/>
        {{ work.description }}
    </div>
</figure>