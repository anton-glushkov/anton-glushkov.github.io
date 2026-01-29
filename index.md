---
title: Home
has_map: true
---

Dedicated and practical IT Professional with direct experience as an IT Endpoint Technician within critical healthcare infrastructure. Proven track record in hardware deployment, component-level repairs, and first-line support in high-pressure medical environments. Technically proficient in Windows administration and Active Directory, with a strong commitment to maintaining system availability for essential healthcare services. 

<p>
  <span style="display: inline-flex; align-items: center; gap: 0.4em;">
    <svg height="1.2em" width="1.2em" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true" style="color: #0a66c2;">
      <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"/>
    </svg>
    <a href="https://www.linkedin.com/in/antonglushkov/" style="color: #0a66c2; text-decoration: none;">LinkedIn: /antonglushkov</a>
  </span>
</p>

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