---
layout: page
title: Gallery
permalink: /gallery/
published: true
---

I am fond of photography; this site records some of the beautiful places I have been as well as the adorable animals I have petted.

<div class="gallery-cards">
{% for photo in site.data.gallery %}<figure class="gallery-card">
<a href="{{ photo.image }}" title="{{ photo.caption | escape }}"><img src="{{ photo.image }}" alt="{{ photo.alt | escape }}" loading="lazy"></a>
<figcaption><span class="gallery-card__caption">{{ photo.caption }}</span><span class="gallery-card__place">{{ photo.place }}</span></figcaption>
</figure>
{% endfor %}</div>
