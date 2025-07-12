---
layout: single
title: "Wanderlust Map"
permalink: /wanderlust-map/
---

<p style="font-weight: 600; font-size: 1.1rem; margin-bottom: 0.5rem;">
  🌍 Places visited: <span id="placeCount">...</span>
</p>

<div id="map" style="height: 600px; margin-top: 2em;"></div>

<link
  rel="stylesheet"
  href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var map = L.map("map").setView([48.8566, 2.3522], 3);

  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    attribution:
      '&copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors',
  }).addTo(map);

  // --- Turkey (red)
  L.circleMarker([39.9208, 32.8541], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ankara</strong><br>Turkey");
  L.circleMarker([41.0082, 28.9784], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Istanbul</strong><br>Turkey");
  L.circleMarker([36.4018, 36.3498], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Hatay</strong><br>Turkey");
  L.circleMarker([37.5736, 36.9371], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kahramanmaraş</strong><br>Turkey");
  L.circleMarker([36.8969, 30.7133], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Antalya</strong><br>Turkey");
  L.circleMarker([38.4192, 27.1287], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Izmir</strong><br>Turkey");
  L.circleMarker([37.0344, 27.4303], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bodrum</strong><br>Turkey");
  L.circleMarker([36.8529, 28.2744], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Marmaris</strong><br>Turkey");
  L.circleMarker([36.2013, 29.6380], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kaş</strong><br>Turkey");
  L.circleMarker([37.1674, 38.7955], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Şanlıurfa</strong><br>Turkey");
  L.circleMarker([37.0662, 37.3833], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Gaziantep</strong><br>Turkey");
  L.circleMarker([39.9043, 41.2679], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Erzurum</strong><br>Turkey");
  L.circleMarker([40.8533, 29.8815], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kocaeli</strong><br>Turkey");

  // --- France (blue)
  L.circleMarker([48.8566, 2.3522], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Paris</strong><br>France");
  L.circleMarker([47.3220, 5.0415], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Dijon</strong><br>France");
  L.circleMarker([48.5734, 7.7521], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Strasbourg</strong><br>France");
  L.circleMarker([45.8992, 6.1294], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Annecy</strong><br>France");
  L.circleMarker([48.0796, 7.3585], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Colmar</strong><br>France");

  // --- Switzerland (green)
  L.circleMarker([46.5197, 6.6323], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lausanne</strong><br>Switzerland");
  L.circleMarker([46.9481, 7.4474], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bern</strong><br>Switzerland");
  L.circleMarker([46.2044, 6.1432], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Geneva</strong><br>Switzerland");
  L.circleMarker([47.3769, 8.5417], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Zurich</strong><br>Switzerland");
  L.circleMarker([46.6863, 7.8632], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Interlaken</strong><br>Switzerland");

  // --- Italy (orange)
  L.circleMarker([45.4642, 9.1900], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Milan</strong><br>Italy");
  L.circleMarker([45.4408, 12.3155], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Venice</strong><br>Italy");
  L.circleMarker([43.7696, 11.2558], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Florence</strong><br>Italy");
  L.circleMarker([41.9028, 12.4964], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Rome</strong><br>Italy");
  L.circleMarker([45.8081, 9.0852], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Como</strong><br>Italy");

  // --- Canada (purple)
  L.circleMarker([45.5019, -73.5674], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Montreal</strong><br>Canada");
  L.circleMarker([43.6532, -79.3832], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Toronto</strong><br>Canada");
  L.circleMarker([45.4215, -75.6996], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ottawa</strong><br>Canada");
  L.circleMarker([46.2382, -63.1311], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Prince Edward Island</strong><br>Canada");
  L.circleMarker([46.8139, -71.2082], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Quebec City</strong><br>Canada");
  L.circleMarker([48.4274, -123.3673], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Victoria</strong><br>Canada");
  L.circleMarker([45.9636, -66.6431], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Gaspésie</strong><br>Canada");
  L.circleMarker([46.1605, -60.8119], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Cap Breton</strong><br>Canada");
  L.circleMarker([48.4284, -71.0684], {radius: 6, color: "salmon", fillColor: "salmon", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Saguenay</strong><br>Canada");

  // --- Germany (darkred)
  L.circleMarker([51.2277, 6.7735], {radius: 6, color: "darkred", fillColor: "darkred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Düsseldorf</strong><br>Germany");
  
  // --- United Kingdom (cadetblue)
  L.circleMarker([51.5074, -0.1278], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>London</strong><br>UK");
  L.circleMarker([53.4084, -2.9916], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Liverpool</strong><br>UK");
  L.circleMarker([53.4808, -2.2426], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Manchester</strong><br>UK");
  L.circleMarker([51.4816, -3.1791], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Cardiff</strong><br>UK");
  L.circleMarker([55.9533, -3.1883], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Edinburgh</strong><br>UK");

  // --- United States (darkgreen)
  L.circleMarker([40.7128, -74.0060], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>New York</strong><br>USA");
  L.circleMarker([42.3601, -71.0589], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Boston</strong><br>USA");
  L.circleMarker([47.6062, -122.3321], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Seattle</strong><br>USA");
  L.circleMarker([39.7684, -86.1581], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Indianapolis</strong><br>USA");
  L.circleMarker([39.9526, -75.1652], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Philadelphia</strong><br>USA");
  L.circleMarker([44.5588, -72.5778], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Vermont</strong><br>USA");
  L.circleMarker([43.1939, -71.5724], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>New Hampshire</strong><br>USA");
  L.circleMarker([44.2795, -73.9843], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lake Placid</strong><br>USA");
  L.circleMarker([31.9686, -99.9018], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Texas</strong><br>USA");

  // --- Portugal (darkblue)
  L.circleMarker([41.1579, -8.6291], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Porto</strong><br>Portugal");
  L.circleMarker([38.7169, -9.1399], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lisbon</strong><br>Portugal");
  L.circleMarker([38.7974, -9.3904], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Sintra</strong><br>Portugal");

    // --- Ireland (darkpurple)
  L.circleMarker([53.3498, -6.2603], {radius: 6, color: "darkpurple", fillColor: "darkpurple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Dublin</strong><br>Ireland");
  L.circleMarker([54.5973, -5.9301], {radius: 6, color: "darkpurple", fillColor: "darkpurple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Belfast</strong><br>Ireland");

  // --- Belgium (lightred)
  L.circleMarker([50.8503, 4.3517], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Brussels</strong><br>Belgium");
  L.circleMarker([51.0543, 3.7174], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ghent</strong><br>Belgium");
  L.circleMarker([51.2194, 4.4025], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Antwerp</strong><br>Belgium");
  L.circleMarker([51.2093, 3.2247], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bruges</strong><br>Belgium");

  // --- Greece (lightblue)
  L.circleMarker([37.9838, 23.7275], {radius: 6, color: "lightblue", fillColor: "lightblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Athens</strong><br>Greece");
  L.circleMarker([41.1231, 25.4066], {radius: 6, color: "lightblue", fillColor: "lightblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Gumulcine</strong><br>Greece");

    // --- Mexico (gold)
  L.circleMarker([21.1619, -86.8515], {radius: 6, color: "gold", fillColor: "gold", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Cancún</strong><br>Mexico");
  L.circleMarker([20.7099, -89.0943], {radius: 6, color: "gold", fillColor: "gold", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Yucatán</strong><br>Mexico");

  // --- Romania (lightgreen)
  L.circleMarker([44.4268, 26.1025], {radius: 6, color: "lightgreen", fillColor: "lightgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bucharest</strong><br>Romania");

  // --- Netherlands (deeppink)
  L.circleMarker([52.3676, 4.9041], {radius: 6, color: "deeppink", fillColor: "deeppink", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Amsterdam</strong><br>Netherlands");

    // --- Slovenia (skyblue)
  L.circleMarker([46.0569, 14.5058], {radius: 6, color: "skyblue", fillColor: "skyblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ljubljana</strong><br>Slovenia");

  // --- Sweden (teal)
  L.circleMarker([59.3293, 18.0686], {radius: 6, color: "teal", fillColor: "teal", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Stockholm</strong><br>Sweden");

  // --- Finland (steelblue)
  L.circleMarker([60.1695, 24.9354], {radius: 6, color: "steelblue", fillColor: "steelblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Helsinki</strong><br>Finland");

  // --- Latvia (chocolate)
  L.circleMarker([56.9496, 24.1052], {radius: 6, color: "chocolate", fillColor: "chocolate", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Riga</strong><br>Latvia");

  // --- Lithuania (coral)
  L.circleMarker([54.6872, 25.2797], {radius: 6, color: "coral", fillColor: "coral", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Vilnius</strong><br>Lithuania");

  // --- Estonia (navy)
  L.circleMarker([59.4370, 24.7536], {radius: 6, color: "navy", fillColor: "navy", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Tallinn</strong><br>Estonia");

  // --- Norway (olive)
  L.circleMarker([59.9139, 10.7522], {radius: 6, color: "olive", fillColor: "olive", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Oslo</strong><br>Norway");

  // --- Denmark (indigo)
  L.circleMarker([55.6761, 12.5683], {radius: 6, color: "indigo", fillColor: "indigo", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Copenhagen</strong><br>Denmark");


});

  // Count the number of markers
  const markerCount = document.querySelectorAll(".leaflet-interactive").length;
  document.getElementById("placeCount").textContent = markerCount;

</script>

<p style="margin-top: 1em; font-style: italic; color: #666;">
  ...to be continued.
</p>