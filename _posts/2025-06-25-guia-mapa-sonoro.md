---
layout: post
title: Guía para crear un Mapa Sonoro
date: 2025-06-25
categories: [mapa, sonido, humanidades-digitales]
---

# 🎧 Guía para crear un Mapa Sonoro interactivo

Este instructivo explica paso a paso cómo crear un mapa sonoro con metadatos accesibles y visualización interactiva en un sitio web construido con Jekyll y GitHub Pages.

---

## 🗂️ 1. Organiza tus audios

Crea una carpeta llamada `assets/audios/` y guarda ahí tus archivos de sonido en formato `.mp3`.

- Usa nombres simples y sin espacios (ej: `rio-zapopan.mp3`, `mercado-cdmx.mp3`)
- Si tus archivos están en `.wav`, conviene convertirlos a `.mp3` para mayor compatibilidad

---

## 📝 2. Crea el archivo `sounds.json`

Este archivo es la base de datos que contiene los metadatos de cada audio. Guárdalo en la raíz de tu repositorio.

Ejemplo de estructura:

```json
[
  {
    "titulo": "Café en campus",
    "fecha": "2025-06-20",
    "lugar": "Jalisco, Zapopan",
    "descripcion": "Vivencia café ubicado en campus",
    "lat": 20.7366,
    "lon": -103.4552,
    "audio": "coffee-pour-and-stir.mp3"
  },
  {
    "titulo": "Río al amanecer",
    "fecha": "2025-05-12",
    "lugar": "Oaxaca, San José del Pacífico",
    "descripcion": "Flujo de agua entre piedras",
    "lat": 16.2901,
    "lon": -96.4265,
    "audio": "rio-san-jose.mp3"
  }
]
```

> Puedes crear este archivo en VS Code, Google Colab o directamente desde GitHub.

---

## 🗺️ 3. Publica un post con el mapa

Crea un archivo en `_posts/` llamado, por ejemplo:

```
2025-06-25-mapa-sonoro.md
```

Y agrega el siguiente contenido:

```markdown
---
layout: post
title: Mapa Sonoro
date: 2025-06-25
categories: [mapa, sonido, datos]
---

<h2>🌍 Mapa Sonoro</h2>
<div id="map" style="height: 80vh; width: 100%; margin-top: 1rem;"></div>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
const map = L.map('map').setView([23.6345, -102.5528], 5);

L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
  attribution: '&copy; OpenStreetMap contributors'
}).addTo(map);

// Detecta subdirectorio del sitio (ej. jornadas2025)
const basePath = window.location.pathname.split('/')[1];

fetch('/' + basePath + '/sounds.json')
  .then(res => res.json())
  .then(data => {
    data.forEach(sound => {
      const marker = L.marker([sound.lat, sound.lon]).addTo(map);
      const popupContent = `
        <div style="max-width:250px">
          <strong>${sound.titulo}</strong><br/>
          <em>${sound.lugar}</em><br/>
          <p>${sound.descripcion}</p>
          <audio controls src="/${basePath}/assets/audios/${sound.audio}"></audio>
        </div>
      `;
      marker.bindPopup(popupContent);
    });
  });
</script>
```

---

## ✅ 4. Verifica la publicación

1. Asegúrate de que:
   - El post esté en la carpeta `_posts/`
   - `sounds.json` esté en la raíz del proyecto
   - Tus archivos de audio estén en `assets/audios/`
2. Haz `git add`, `git commit` y `git push`
3. Espera ~1-2 minutos a que GitHub Pages actualice

Tu mapa estará visible en:
```
https://USUARIO.github.io/NOMBRE-REPO/año/mes/día/título-del-post
```

---

## 🧩 Recursos y mejoras posibles

- Usar filtros por etiquetas o regiones
- Incorporar visualización de ondas o espectrogramas
- Agregar botones de descarga y licencias
- Construir el JSON dinámicamente desde formularios

---

¿Tienes dudas o quieres colaborar en esta iniciativa? [Escríbenos](mailto:tu@correo.edu)
