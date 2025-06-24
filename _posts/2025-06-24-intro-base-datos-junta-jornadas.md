---
layout: post
date: 2025-06-24
title: "Intro base datos, metadatos y elementos"
nav_order: 2
categories: [recursos, datos, metadatos, elementos]

---

## Índice de contenidos

- [¿Qué son los metadatos?](#qué-son-los-metadatos)
- [¿Qué es una estructura de datos de metadatos?](#qué-es-una-estructura-de-datos-de-metadatos)
- [¿Qué son los elementos en Omeka?](#qué-son-los-elementos-en-omeka)
- [¿Qué es Dublin Core?](#qué-es-dublin-core)
- [Ejemplo completo en Omeka con Dublin Core](#ejemplo-completo-en-omeka-con-dublin-core)
- [Beneficios de usar Dublin Core en Omeka](#beneficios-de-usar-dublin-core-en-omeka)
- [¿Cómo empezar en Omeka?](#cómo-empezar-en-omeka)




## ¿Qué son los metadatos?




## ¿Qué es una estructura de datos de metadatos?

¿Qué es una estructura de datos de metadatos?

Una **estructura de datos de metadatos** es un conjunto organizado de campos que definen:
- Qué tipo de información debe capturarse
- Cómo debe registrarse
- En qué formato debe almacenarse

Estas estructuras aseguran la consistencia y la interoperabilidad en la descripción de recursos digitales.

---


## ¿Qué son los elementos en Omeka?

¿Qué son los elementos en Omeka?

En Omeka, los **elementos** son los campos individuales que usamos para ingresar metadatos al describir un ítem digital (como un documento, imagen o video).

### ✍️ Ejemplo de uso en Omeka:

<table>
  <tr><th>Elemento</th><th>Valor</th></tr>
  <tr><td>Título</td><td>"Carta de Emiliano Zapata a Francisco Villa"</td></tr>
  <tr><td>Creador</td><td>Emiliano Zapata</td></tr>
  <tr><td>Fecha</td><td>18 de noviembre de 1914</td></tr>
  <tr><td>Descripción</td><td>Documento manuscrito dirigido a Francisco Villa</td></tr>
  <tr><td>Derechos</td><td>Reproducción autorizada por el AGN</td></tr>
</table>

---


## ¿Qué es Dublin Core?

¿Qué es Dublin Core?

**Dublin Core** es un estándar internacional para la descripción de recursos digitales. Define 15 elementos básicos que se utilizan en bibliotecas, archivos, museos y repositorios.

### 📚 Los 15 elementos Dublin Core:

<table>
  <tr><th>Elemento</th><th>¿Qué describe?</th></tr>
  <tr><td>Title</td><td>Título del recurso</td></tr>
  <tr><td>Creator</td><td>Autor o creador</td></tr>
  <tr><td>Subject</td><td>Tema o palabras clave</td></tr>
  <tr><td>Description</td><td>Resumen o sinopsis</td></tr>
  <tr><td>Publisher</td><td>Entidad que publica el recurso</td></tr>
  <tr><td>Contributor</td><td>Colaboradores</td></tr>
  <tr><td>Date</td><td>Fecha relevante</td></tr>
  <tr><td>Type</td><td>Tipo de recurso (texto, imagen, etc.)</td></tr>
  <tr><td>Format</td><td>Formato físico o digital</td></tr>
  <tr><td>Identifier</td><td>Identificador único (URL, ID)</td></tr>
  <tr><td>Source</td><td>Recurso del cual deriva</td></tr>
  <tr><td>Language</td><td>Idioma del contenido</td></tr>
  <tr><td>Relation</td><td>Relación con otros recursos</td></tr>
  <tr><td>Coverage</td><td>Cobertura geográfica o temporal</td></tr>
  <tr><td>Rights</td><td>Derechos de uso y licencia</td></tr>
</table>

---


## Ejemplo completo en Omeka con Dublin Core

Ejemplo completo en Omeka con Dublin Core

**Título:** Carta de Emiliano Zapata a Francisco Villa  
**Creador:** Emiliano Zapata  
**Fecha:** 18 de noviembre de 1914  
**Descripción:** Carta manuscrita que reafirma alianza militar  
**Formato:** PDF escaneado, 300 dpi  
**Tipo:** Documento histórico  
**Idioma:** Español  
**Cobertura:** México, Revolución Mexicana  
**Derechos:** AGN, reproducción autorizada

---


## Beneficios de usar Dublin Core en Omeka

Beneficios de usar Dublin Core en Omeka

- ✅ **Estandarización**: permite describir todos los objetos con la misma lógica.
- 🔍 **Facilidad de búsqueda**: mejora la indexación y el acceso.
- 🔗 **Interoperabilidad**: permite intercambiar metadatos entre plataformas.
- 📚 **Simplicidad**: fácil de aprender y aplicar en diferentes contextos culturales.

---


## ¿Cómo empezar en Omeka?

¿Cómo empezar en Omeka?

1. Accede a tu instalación de Omeka o crea una en [omeka.net](https://www.omeka.net).
2. Crea un nuevo ítem.
3. Llena los campos del formulario con los elementos Dublin Core.
4. Adjunta el archivo o enlace del recurso digital.
5. Guarda y publica.

> Puedes extender los metadatos con plugins como **Dublin Core Extended**, **Simple Vocab** o definir conjuntos de elementos personalizados.
