---
title: Home
has_map: true
---

Dedicated and practical IT Professional with direct experience as an IT Endpoint Technician within critical healthcare infrastructure. Proven track record in hardware deployment, component-level repairs, and first-line support in high-pressure medical environments. Technically proficient in Windows administration and Active Directory, with a strong commitment to maintaining system availability for essential healthcare services. 

<p>
  <span style="display: inline-flex; align-items: center; gap: 0.4em;">
<svg xmlns="http://www.w3.org/2000/svg" shape-rendering="geometricPrecision" text-rendering="geometricPrecision" image-rendering="optimizeQuality" fill-rule="evenodd" clip-rule="evenodd" viewBox="0 0 512 512"><path fill="#0085FF" d="M105 0h302c57.928.155 104.845 47.072 105 104.996V407c-.155 57.926-47.072 104.844-104.996 104.998L105 512C47.074 511.844.156 464.926.002 407.003L0 105C.156 47.072 47.074.155 104.997 0H105z"/><path fill="#fff" fill-rule="nonzero" d="M173.234 144.311c33.5 25.237 69.538 76.397 82.765 103.853 13.228-27.456 49.267-78.616 82.767-103.853 24.177-18.205 63.343-32.294 63.343 12.534 0 8.949-5.115 75.209-8.117 85.969-10.429 37.393-48.441 46.931-82.251 41.159 59.1 10.091 74.133 43.513 41.664 76.936-61.663 63.479-88.629-15.927-95.533-36.273-1.991-5.857-1.708-5.991-3.745 0-6.905 20.346-33.869 99.752-95.531 36.273-32.47-33.423-17.437-66.845 41.663-76.936-33.81 5.772-71.822-3.766-82.251-41.159-3.002-10.76-8.117-77.02-8.117-85.969 0-44.828 39.172-30.739 63.343-12.534z"/></svg>
    <a href="https://www.linkedin.com/in/antonglushkov/" style="font-family:system-ui;">/antonglushkov</a>
  </span>
</p>
<p>
  <span style="display: inline-flex; align-items: center; gap: 0.4em;">
<svg width="20px" height="18px" version="1.1" xmlns="http://www.w3.org/2000/svg">
 <path d="m135.72 44.03c66.496 49.921 138.02 151.14 164.28 205.46 26.262-54.316 97.782-155.54 164.28-205.46 47.98-36.021 125.72-63.892 125.72 24.795 0 17.712-10.155 148.79-16.111 170.07-20.703 73.984-96.144 92.854-163.25 81.433 117.3 19.964 147.14 86.092 82.697 152.22-122.39 125.59-175.91-31.511-189.63-71.766-2.514-7.3797-3.6904-10.832-3.7077-7.8964-0.0174-2.9357-1.1937 0.51669-3.7077 7.8964-13.714 40.255-67.233 197.36-189.63 71.766-64.444-66.128-34.605-132.26 82.697-152.22-67.108 11.421-142.55-7.4491-163.25-81.433-5.9562-21.282-16.111-152.36-16.111-170.07 0-88.687 77.742-60.816 125.72-24.795z" fill="#1185fe"/>
</svg>
    <a href="https://bsky.app/profile/glushkov.pp.ua" style="font-family:system-ui;">/glushkov.pp.ua</a>
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

