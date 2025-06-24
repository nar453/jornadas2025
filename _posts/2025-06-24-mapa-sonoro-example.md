---
layout: post
title: Ejemplo de Mapa Sonoro Básico
date: 2025-06-24
categories: [mapa, sonido, datos]

---
<link
  rel="stylesheet"
  href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
/>

<h2>🌍 Mapa Sonoro</h2>
<div id="map" style="height: 80vh; width: 100%; min-height: 400px;"></div>


<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
const map = L.map('map').setView([23.6345, -102.5528], 5);

L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
  attribution: '&copy; OpenStreetMap contributors'
}).addTo(map);

fetch('/sounds.json')
  .then(res => res.json())
  .then(data => {
    data.forEach(sound => {
      const marker = L.marker([sound.lat, sound.lon]).addTo(map);
      const popupContent = `
        <div style="max-width:250px">
          <strong>${sound.titulo}</strong><br/>
          <em>${sound.lugar}</em><br/>
          <p>${sound.descripcion}</p>
          <audio controls src="/assets/audios/${sound.audio}"></audio>
        </div>
      `;
      marker.bindPopup(popupContent);
    });
  });
</script>
