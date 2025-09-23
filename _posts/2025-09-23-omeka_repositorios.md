---
layout: post
title: Omeka y otros repositorios | Jornadas HD
date: 2025-09-23
categories: [omeka, repositorio, humanidades-digitales]
---

# Comparación: Omeka, Islandora y Samvera/Hyrax

Sitio: https://www.omeka.net/

## Tabla comparativa

| Criterio            | Omeka (S/Classic) | Islandora (Drupal + Fedora) | Samvera/Hyrax | Licencia Software | Derechos/Acceso | Notas de Licencias de Contenido |
|---------------------|-------------------|-----------------------------|---------------|------------------|-----------------|---------------------------------|
| **Enfoque principal** | Publicación y exhibición de colecciones y narrativas (GLAM, HD). | Repositorio DAM/GLAM con fuerte integración Drupal y Fedora; escalable. | Framework de repositorios institucionales con flujos avanzados y alta configurabilidad. | GPLv3 | Roles básicos por sitio/contenido; menos granular que Islandora/Samvera. | Soporta CC y RightsStatements.org mediante plugins. |
| **Metadatos** | Dublin Core/Terms; plantillas y vocabularios sugeridos. | Esquemas flexibles vía Drupal + Fedora/Triplestore. | Modelos de 'Works/Files'; extensible. | GPL (hereda de Drupal/Fedora) | Control a nivel Drupal (roles, IP, etc.). | Derechos representados en campos Drupal; flexible para CC/RightsStatements.org. |
| **IIIF** | Soporta IIIF mediante módulos (IIIF Server/Presentation). | Soporte IIIF (zoom, pan, viewers). | Depende de configuración; no siempre 'core'. | GPL (Islandora) | Restricciones deben gestionarse vía Drupal, no automáticamente en Fedora/Solr. | Posibilidad de publicar metadatos de derechos junto a IIIF manifiestos. |
| **Control de acceso** | Roles básicos; limitado para flujos complejos. | Robusto a nivel Drupal; **ojo** con accesos directos a Fedora. | Visibilidad granular, embargos y leases. | Apache 2.0 (Samvera) | Visibilidad por obra/archivo; embargos temporales. | Permite publicar con restricciones de tiempo y acceso. |

---

## Derechos de autor y licencias en estas plataformas

No **pierdes** tus derechos de autor al subir materiales a **Omeka, Islandora o Samvera**.  
Estas plataformas son **software de código abierto**, no servicios comerciales con términos que exijan cesiones de derechos.

- **Autoría**: La autoría siempre sigue siendo tuya o de quien corresponda legalmente.  
- **Licencias**: Tú decides bajo qué licencia publicas el material (por ejemplo, **Copyright completo, Creative Commons, RightsStatements.org**).  
- **Control de acceso**:  
  - **Omeka**: puedes añadir campos de licencia y mostrar un aviso claro al público.  
  - **Islandora**: controlas tanto los metadatos como quién puede acceder (roles de Drupal).  
  - **Samvera**: permite visibilidad granular, embargos temporales y concesión de accesos específicos.  

👉 Lo importante es configurar de manera explícita los **metadatos de derechos** y, si lo requieres, las **políticas de acceso**.  
La plataforma no te quita derechos; solo los gestiona y muestra según lo que decidas.

---

# Ejemplos prácticos de declaración de derechos

### 🔹 Omeka (S/Classic)
En el **campo de metadatos “Rights”** (Dublin Core), podrías escribir:

```text
© 2025 Natalia Rocha Díaz. Todos los derechos reservados.
Licencia: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/)
