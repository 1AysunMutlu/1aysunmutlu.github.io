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
  let markerCount = 0;

  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    attribution:
      '&copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors',
  }).addTo(map);

  // --- Türkiye (red)
  L.circleMarker([39.9208, 32.8541], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ankara</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([41.0082, 28.9784], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Istanbul</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([36.4018, 36.3498], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Hatay</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([37.5736, 36.9371], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kahramanmaraş</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([36.8969, 30.7133], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Antalya</strong><br>Turkey");
  markerCount++;
  L.circleMarker([38.4192, 27.1287], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Izmir</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([37.0344, 27.4303], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bodrum</strong><br>Türkiye");
  L.circleMarker([36.8529, 28.2744], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Marmaris</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([36.2013, 29.6380], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kaş</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([37.1674, 38.7955], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Şanlıurfa</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([37.0662, 37.3833], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Gaziantep</strong><br>Turkey");
  markerCount++;
  L.circleMarker([39.9043, 41.2679], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Erzurum</strong><br>Türkiye");
  markerCount++;
  L.circleMarker([40.8533, 29.8815], {radius: 6, color: "red", fillColor: "red", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Kocaeli</strong><br>Türkiye");
  markerCount++;

  // --- France (blue)
  L.circleMarker([48.8566, 2.3522], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Paris</strong><br>France");
    markerCount++;
  L.circleMarker([47.3220, 5.0415], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Dijon</strong><br>France");
    markerCount++;
  L.circleMarker([48.5734, 7.7521], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Strasbourg</strong><br>France");
    markerCount++;
  L.circleMarker([45.8992, 6.1294], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Annecy</strong><br>France");
    markerCount++;
  L.circleMarker([48.0796, 7.3585], {radius: 6, color: "blue", fillColor: "blue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Colmar</strong><br>France");
    markerCount++;

  // --- Switzerland (green)
  L.circleMarker([46.5197, 6.6323], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lausanne</strong><br>Switzerland");
    markerCount++;
  L.circleMarker([46.9481, 7.4474], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bern</strong><br>Switzerland");
    markerCount++;
  L.circleMarker([46.2044, 6.1432], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Geneva</strong><br>Switzerland");
    markerCount++;
  L.circleMarker([47.3769, 8.5417], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Zurich</strong><br>Switzerland");
    markerCount++;
  L.circleMarker([46.6863, 7.8632], {radius: 6, color: "green", fillColor: "green", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Interlaken</strong><br>Switzerland");
    markerCount++;

  // --- Italy (orange)
  L.circleMarker([45.4642, 9.1900], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Milan</strong><br>Italy");
    markerCount++;
  L.circleMarker([45.4408, 12.3155], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Venice</strong><br>Italy");
    markerCount++;
  L.circleMarker([43.7696, 11.2558], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Florence</strong><br>Italy");
    markerCount++;
  L.circleMarker([41.9028, 12.4964], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Rome</strong><br>Italy");
    markerCount++;
  L.circleMarker([45.8081, 9.0852], {radius: 6, color: "orange", fillColor: "orange", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Como</strong><br>Italy");
    markerCount++;

    // --- Canada (purple)
  L.circleMarker([45.5019, -73.5674], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Montreal</strong><br>Canada"); markerCount++;

  L.circleMarker([43.6532, -79.3832], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Toronto</strong><br>Canada"); markerCount++;

  L.circleMarker([45.4215, -75.6996], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Ottawa</strong><br>Canada"); markerCount++;

  L.circleMarker([46.2382, -63.1311], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Prince Edward Island</strong><br>Canada"); markerCount++;

  L.circleMarker([46.8139, -71.2082], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Quebec City</strong><br>Canada"); markerCount++;

  L.circleMarker([48.8339, -64.4817], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Gaspé</strong><br>Canada"); markerCount++;

  L.circleMarker([48.5256, -64.2104], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Percé</strong><br>Canada"); markerCount++;

  L.circleMarker([44.6488, -63.5752], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Halifax</strong><br>Canada"); markerCount++;

  L.circleMarker([45.2733, -66.0633], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Saint John</strong><br>New Brunswick, Canada"); markerCount++;

  L.circleMarker([51.1784, -115.5708], {radius: 6, color: "purple", fillColor: "purple", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Banff</strong><br>Canada"); markerCount++;

  // --- Germany (darkred)
  L.circleMarker([51.2277, 6.7735], {radius: 6, color: "darkred", fillColor: "darkred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Düsseldorf</strong><br>Germany");
    markerCount++;
  
  // --- United Kingdom (cadetblue)
  L.circleMarker([51.5074, -0.1278], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>London</strong><br>UK");
    markerCount++;
  L.circleMarker([53.4084, -2.9916], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Liverpool</strong><br>UK");
    markerCount++;
  L.circleMarker([53.4808, -2.2426], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Manchester</strong><br>UK");
    markerCount++;
  L.circleMarker([51.4816, -3.1791], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Cardiff</strong><br>UK");
    markerCount++;
  L.circleMarker([55.9533, -3.1883], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Edinburgh</strong><br>UK");
    markerCount++;

  // --- United Kingdom (cadetblue)
  L.circleMarker([55.8642, -4.2518], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Glasgow</strong><br>UK"); markerCount++;

  L.circleMarker([51.6214, -3.9436], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Swansea</strong><br>UK"); markerCount++;

  L.circleMarker([50.8225, -0.1372], {radius: 6, color: "cadetblue", fillColor: "cadetblue", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Brighton</strong><br>UK"); markerCount++;

  // --- United States (darkgreen)
  L.circleMarker([40.7128, -74.0060], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>New York</strong><br>USA");
  markerCount++;
  L.circleMarker([42.3601, -71.0589], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Boston</strong><br>USA");
  markerCount++;
  L.circleMarker([47.6062, -122.3321], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Seattle</strong><br>USA");
  markerCount++;
  L.circleMarker([39.7684, -86.1581], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Indianapolis</strong><br>USA");
  markerCount++;
  L.circleMarker([39.9526, -75.1652], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Philadelphia</strong><br>USA");
  markerCount++;
  L.circleMarker([44.5588, -72.5778], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Vermont</strong><br>USA");
  markerCount++;
  L.circleMarker([43.1939, -71.5724], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>New Hampshire</strong><br>USA");
  markerCount++;
  L.circleMarker([44.2795, -73.9843], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lake Placid</strong><br>USA");
  markerCount++;
  L.circleMarker([31.9686, -99.9018], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Texas</strong><br>USA");
  markerCount++;
    // --- United States (darkgreen)
  L.circleMarker([39.9612, -82.9988], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Columbus (Ohio)</strong><br>USA"); markerCount++;
  L.circleMarker([33.4484, -112.0740], {radius: 6, color: "darkgreen", fillColor: "darkgreen", fillOpacity: 0.8})
    .addTo(map).bindPopup("<strong>Phoenix</strong><br>USA"); markerCount++;

  // --- Portugal (darkblue)
  L.circleMarker([41.1579, -8.6291], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Porto</strong><br>Portugal");
  markerCount++;
  L.circleMarker([38.7169, -9.1399], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Lisbon</strong><br>Portugal");
  markerCount++;
  L.circleMarker([38.7974, -9.3904], {radius: 6, color: "darkblue", fillColor: "darkblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Sintra</strong><br>Portugal");
  markerCount++;

    // --- Ireland (darkpurple)
  L.circleMarker([53.3498, -6.2603], {radius: 6, color: "darkpurple", fillColor: "darkpurple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Dublin</strong><br>Ireland");
  markerCount++;
  L.circleMarker([54.5973, -5.9301], {radius: 6, color: "darkpurple", fillColor: "darkpurple", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Belfast</strong><br>Ireland");
  markerCount++;

  // --- Belgium (lightred)
  L.circleMarker([50.8503, 4.3517], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Brussels</strong><br>Belgium");
  markerCount++;
  L.circleMarker([51.0543, 3.7174], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ghent</strong><br>Belgium");
  markerCount++;
  L.circleMarker([51.2194, 4.4025], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Antwerp</strong><br>Belgium");
  markerCount++;
  L.circleMarker([51.2093, 3.2247], {radius: 6, color: "lightred", fillColor: "lightred", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bruges</strong><br>Belgium");
  markerCount++;

  // --- Greece (lightblue)
  L.circleMarker([37.9838, 23.7275], {radius: 6, color: "lightblue", fillColor: "lightblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Athens</strong><br>Greece");
  markerCount++;
  L.circleMarker([41.1231, 25.4066], {radius: 6, color: "lightblue", fillColor: "lightblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Gumulcine</strong><br>Greece");
  markerCount++;

    // --- Mexico (gold)
  L.circleMarker([21.1619, -86.8515], {radius: 6, color: "gold", fillColor: "gold", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Cancún</strong><br>Mexico");
  markerCount++;
  L.circleMarker([20.7099, -89.0943], {radius: 6, color: "gold", fillColor: "gold", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Yucatán</strong><br>Mexico");
  markerCount++;

  // --- Romania (lightgreen)
  L.circleMarker([44.4268, 26.1025], {radius: 6, color: "lightgreen", fillColor: "lightgreen", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Bucharest</strong><br>Romania");
  markerCount++;

  // --- Netherlands (deeppink)
  L.circleMarker([52.3676, 4.9041], {radius: 6, color: "deeppink", fillColor: "deeppink", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Amsterdam</strong><br>Netherlands");
  markerCount++;

    // --- Slovenia (skyblue)
  L.circleMarker([46.0569, 14.5058], {radius: 6, color: "skyblue", fillColor: "skyblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Ljubljana</strong><br>Slovenia");
  markerCount++;

  // --- Sweden (teal)
  L.circleMarker([59.3293, 18.0686], {radius: 6, color: "teal", fillColor: "teal", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Stockholm</strong><br>Sweden");
  markerCount++;

  // --- Finland (steelblue)
  L.circleMarker([60.1695, 24.9354], {radius: 6, color: "steelblue", fillColor: "steelblue", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Helsinki</strong><br>Finland");
  markerCount++;

  // --- Latvia (chocolate)
  L.circleMarker([56.9496, 24.1052], {radius: 6, color: "chocolate", fillColor: "chocolate", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Riga</strong><br>Latvia");
  markerCount++;

  // --- Lithuania (coral)
  L.circleMarker([54.6872, 25.2797], {radius: 6, color: "coral", fillColor: "coral", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Vilnius</strong><br>Lithuania");
  markerCount++;

  // --- Estonia (navy)
  L.circleMarker([59.4370, 24.7536], {radius: 6, color: "navy", fillColor: "navy", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Tallinn</strong><br>Estonia");
  markerCount++;

  // --- Norway (olive)
  L.circleMarker([59.9139, 10.7522], {radius: 6, color: "olive", fillColor: "olive", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Oslo</strong><br>Norway");
  markerCount++;

  // --- Denmark (indigo)
  L.circleMarker([55.6761, 12.5683], {radius: 6, color: "indigo", fillColor: "indigo", fillOpacity: 0.8}).addTo(map).bindPopup("<strong>Copenhagen</strong><br>Denmark");
  markerCount++;


});

  // Count the number of markers
  const markerCount = document.querySelectorAll(".leaflet-interactive").length;
  document.getElementById("placeCount").textContent = markerCount;

</script>

<p style="margin-top: 1em; font-style: italic; color: #666;">
  ...to be continued.
</p>