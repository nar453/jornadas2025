---
layout: post
date: 2025-06-24
title: "Plantilla de Metadatos para Mapa Sonoro"
categories: [recursos, datos, metadatos, mapa, sonoro]
---


## 🧭 Metadatos para Mapa Sonoro

Esta plantilla está basada en el estándar Dublin Core, con campos adaptados para la descripción y publicación de grabaciones georreferenciadas en proyectos de mapa sonoro.

### 📋 Campos de metadatos recomendados:

<style>
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1rem;
  font-size: 16px;
}
th, td {
  border: 1px dotted #666;
  padding: 10px;
  text-align: left;
}
th {
  background-color: #f0f0f0;
  font-weight: bold;
}
</style>

<table>
  <thead>
    <tr>
      <th>Elemento</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><strong>Título</strong></td><td>Nombre descriptivo del sonido</td></tr>
    <tr><td><strong>Fecha</strong></td><td>Fecha de grabación (formato ISO: YYYY-MM-DD)</td></tr>
    <tr><td><strong>Lugar</strong></td><td>Ubicación descriptiva (ciudad, sitio, referencia geográfica)</td></tr>
    <tr><td><strong>Coordenadas</strong></td><td>Latitud y longitud en formato decimal (ej. 25.6866, -100.3161)</td></tr>
    <tr><td><strong>Duración</strong></td><td>Duración del archivo en minutos/segundos</td></tr>
    <tr><td><strong>Grabado por</strong></td><td>Persona o institución que realizó la grabación</td></tr>
    <tr><td><strong>Descripción</strong></td><td>Contexto del sonido, ambiente, características auditivas</td></tr>
    <tr><td><strong>Tipo</strong></td><td>Clasificación del sonido (paisaje sonoro, entrevista, naturaleza, etc.)</td></tr>
    <tr><td><strong>Formato</strong></td><td>Formato de archivo (ej. MP3, WAV)</td></tr>
    <tr><td><strong>Idioma</strong></td><td>Idioma, si contiene habla (ej. español, mixteco)</td></tr>
    <tr><td><strong>Licencia</strong></td><td>Tipo de licencia (ej. CC BY 4.0, Dominio público)</td></tr>
    <tr><td><strong>Identificador</strong></td><td>Enlace al archivo o ID único para catalogación interna</td></tr>
    <tr><td><strong>Palabras clave</strong></td><td>Términos asociados (ej. río, mercado, tráfico, ritual)</td></tr>
  </tbody>
</table>

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
