---
title: Home
has_map: true
---

Dedicated and practical IT Professional with direct experience as an IT Endpoint Technician within critical healthcare infrastructure. Proven track record in hardware deployment, component-level repairs, and first-line support in high-pressure medical environments. Technically proficient in Windows administration and Active Directory, with a strong commitment to maintaining system availability for essential healthcare services. 

[LinkedIn: /antonglushkov](https://www.linkedin.com/in/antonglushkov/)


<div style="margin: 20px 0; font-size: 18px;">
  <a href="https://www.linkedin.com/in/antonglushkov/" target="_blank" rel="noopener noreferrer" style="text-decoration: none; color: #0077b5; display: inline-flex; align-items: center; gap: 8px;">
    <svg width="20" height="20" viewBox="0 0 72 72" xmlns="http://www.w3.org/2000/svg">
      <g fill="none" fill-rule="evenodd">
        <path d="M8,72 L64,72 C68.418278,72 72,68.418278 72,64 L72,8 C72,3.581722 68.418278,0 64,0 L8,0 C3.581722,0 0,3.581722 0,8 L0,64 C0,68.418278 3.581722,72 8,72 Z" fill="#007EBB"/>
        <path d="M62,62 L51.315625,62 L51.315625,43.8021149 C51.315625,38.8127542 49.4197917,36.0245323 45.4707031,36.0245323 C41.1746094,36.0245323 38.9300781,38.9261103 38.9300781,43.8021149 L38.9300781,62 L28.6333333,62 L28.6333333,27.3333333 L38.9300781,27.3333333 L38.9300781,32.0029283 C38.9300781,32.0029283 42.0260417,26.2742151 49.3825521,26.2742151 C56.7356771,26.2742151 62,30.7644705 62,40.051212 L62,62 Z M16.349349,22.7940133 C12.8420573,22.7940133 10,19.9296567 10,16.3970067 C10,12.8643566 12.8420573,10 16.349349,10 C19.8566406,10 22.6970052,12.8643566 22.6970052,16.3970067 C22.6970052,19.9296567 19.8566406,22.7940133 16.349349,22.7940133 Z M11.0325521,62 L21.769401,62 L21.769401,27.3333333 L11.0325521,27.3333333 L11.0325521,62 Z" fill="#FFF"/>
      </g>
    </svg>
    LinkedIn: /antonglushkov
  </a>
</div>

Key Skills:
{% include nodes.html %}

Located in:
{% include map.html %}

Actively seeking any IT or IT-related role where strong technical fundamentals, reliability, and willingness to learn are valued.

## Posts

<ul class="posts">
  {% for post in site.posts limit:10 %}
<li class="posts">
  <svg class="post-icon" viewBox="0 0 24 24" aria-hidden="true"
       xmlns="http://www.w3.org/2000/svg">
    <g>
      <path d="M20.5,22H4c-0.2,0-0.3,0-0.5,0C1.6,22,0,20.4,0,18.5V6h5V2h19v16.5C24,20.4,22.4,22,20.5,22z M6.7,20h13.8
        c0.8,0,1.5-0.7,1.5-1.5V4H7v14.5C7,19,6.9,19.5,6.7,20z M2,8v10.5C2,19.3,2.7,20,3.5,20S5,19.3,5,18.5V8H2z"/>
      <rect x="15" y="6" width="5" height="6"/>
      <rect x="9" y="6" width="4" height="2"/>
      <rect x="9" y="10" width="4" height="2"/>
      <rect x="9" y="14" width="11" height="2"/>
    </g>
  </svg>

  <strong>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </strong>
  <span style="color: #666;"> — {{ post.date | date: "%B %d, %Y" }}</span>
</li>
  {% endfor %}
</ul>

{% if site.posts.size > 10 %}
  <p><a href="/posts/">View all posts →</a></p>
{% endif %}

<footer>
    <p>© 2026 Anton Glushkov</p>
  <p>This page is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">Creative
Commons Attribution-NoDerivatives 4.0 International License</a></p>
</footer>

<script>
document.addEventListener('DOMContentLoaded', function() {
    // London center
    var myLat = 51.5074;
    var myLon = -0.1278;
    var zoomLevel = 14;

    var map = L.map('map', {
      zoomControl: false,
      attributionControl: false
    }).setView([myLat, myLon], zoomLevel);

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
      attribution: ''
    }).addTo(map);

  });
</script>