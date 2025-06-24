---
layout: post
date: 2025-06-24
title: "Plantilla de Metadatos para Mapa Sonoro"
categories: [recursos, datos, metadatos, mapa, sonoro]
---

## 🧭 Plantilla de Metadatos para Mapa Sonoro

Esta plantilla está basada en el estándar Dublin Core, con campos adaptados para la descripción y publicación de grabaciones georreferenciadas en proyectos de mapa sonoro.

### 📋 Campos de metadatos recomendados:

| Elemento       | Descripción                                                                 |
|----------------|------------------------------------------------------------------------------|
| **Título**      | Nombre descriptivo del sonido                                               |
| **Fecha**       | Fecha de grabación (formato ISO: YYYY-MM-DD)                               |
| **Lugar**       | Ubicación descriptiva (ciudad, sitio, referencia geográfica)               |
| **Coordenadas** | Latitud y longitud en formato decimal (ej. 25.6866, -100.3161)              |
| **Duración**    | Duración del archivo en minutos/segundos                                   |
| **Grabado por** | Persona o institución que realizó la grabación                             |
| **Descripción** | Contexto del sonido, ambiente, características auditivas                    |
| **Tipo**        | Clasificación del sonido (paisaje sonoro, entrevista, naturaleza, etc.)     |
| **Formato**     | Formato de archivo (ej. MP3, WAV)                                           |
| **Idioma**      | Idioma, si contiene habla (ej. español, mixteco)                           |
| **Licencia**    | Tipo de licencia (ej. CC BY 4.0, Dominio público)                           |
| **Identificador** | Enlace al archivo o ID único para catalogación interna                  |
| **Palabras clave** | Términos asociados (ej. río, mercado, tráfico, ritual)                |

---

## 📌 Recomendaciones

- Usar coordenadas exactas si se desea visualización en mapa.
- Documentar el consentimiento si hay personas identificables.
- Asegurar compatibilidad de metadatos con plataformas como Aporee, Omeka o Leaflet.js.

---

## 📎 Ejemplo de entrada en YAML

```yaml
titulo: "Sonido de las campanas de la Catedral"
fecha: "2023-04-16"
lugar: "Centro Histórico de Zacatecas"
coordenadas: "22.7743, -102.5722"
duracion: "1:32"
grabado_por: "Lydia R."
descripcion: "Registro sonoro de las campanas tocando al mediodía. Fondo con sonido urbano leve."
tipo: "Paisaje sonoro"
formato: "MP3"
idioma: "Sin habla"
licencia: "CC BY-NC 4.0"
identificador: "zac-campanas-2023"
palabras_clave: ["campanas", "ciudad", "Zacatecas", "religioso"]
```

---

