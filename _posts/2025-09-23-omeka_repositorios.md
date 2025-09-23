---
layout: post
title: Omeka y otros repositorios | Jornadas HD
date: 2025-09-23
categories: [omeka, repositorio, humanidades-digitales]
---

# Comparación: Omeka, Wikicommons y otros repositorios

[Omeka](https://www.omeka.net/)


[Wikicommons](https://commons.wikimedia.org/wiki/Portada)


## Comparación: Omeka vs Wikimedia Commons

### Tabla comparativa

| Criterio | **Omeka (S/Classic)** | **Wikimedia Commons** |
|----------|------------------------|------------------------|
| **Naturaleza** | Software de **código abierto** para crear repositorios/exposiciones propias (se instala en tu servidor). | Plataforma global de la **Fundación Wikimedia**, repositorio abierto centralizado. |
| **Licencia del software/plataforma** | GPLv3 (Omeka Classic y S). | El software base es **MediaWiki (GPL)**; el contenido está sujeto a las licencias elegidas por los usuarios, típicamente **Creative Commons Atribución/CompartirIgual**. |
| **Control sobre el servidor** | Total: tú administras el hosting, base de datos, diseño y políticas de acceso. | Ninguno: todo el contenido está alojado en los servidores de Wikimedia. |
| **Tipos de contenido** | Colecciones digitales variadas (imágenes, audio, video, textos, metadatos). | Imágenes, audio, video y algunos documentos, pero siempre bajo licencias libres o dominio público. |
| **Metadatos** | Dublin Core, Dublin Core Terms, vocabularios personalizados; admite IIIF y extensiones. | Plantillas MediaWiki con campos básicos (autor, fuente, fecha, licencia, categorías, Wikidata). |
| **Control de acceso** | Roles de usuario dentro de tu instalación (administrador, editor, público); puedes restringir colecciones o ítems. | Todo lo subido es **público** (salvo excepciones legales mínimas). No existe acceso restringido. |
| **Licencias de contenido** | Tú decides: Copyright, Creative Commons, RightsStatements.org, etc. | Solo se aceptan **licencias libres** (ej. CC BY, CC BY-SA, dominio público). Contenido con Copyright cerrado es rechazado. |
| **Derechos de autor** | Los autores **mantienen sus derechos**; la plataforma no reclama cesión. | Los autores **mantienen sus derechos**, pero deben **ceder a una licencia libre irrevocable** (ej. CC BY-SA). |
| **Visibilidad** | Local/global según tu infraestructura; puedes tener un sitio pequeño o un portal internacional. | Global: millones de usuarios, indexación en Google y conexión con Wikipedia/Wikidata. |
| **Orientación** | Museos, archivos, bibliotecas, proyectos académicos y de investigación que quieren **gestionar y exhibir** colecciones. | Repositorio masivo de **medios reutilizables** para Wikipedia y proyectos libres. |

---

### Derechos de autor y licencias

**Omeka**
- El **autor conserva siempre sus derechos**.  
- Se pueden subir materiales bajo **cualquier régimen de derechos** (Copyright cerrado, acceso restringido, o licencias abiertas).  
- Es posible usar **Creative Commons**, **RightsStatements.org** o un aviso legal propio.  
- Control granular: puedes mostrar materiales solo a ciertos roles (ej. estudiantes o investigadores).

**Wikimedia Commons**
- El **autor conserva sus derechos**, pero para subir debe **aceptar una licencia libre e irrevocable** (como CC BY o CC BY-SA).  
- No se permite material con copyright cerrado ni “uso justo” (excepto casos mínimos muy regulados).  
- El contenido subido puede ser reutilizado por cualquier persona, incluso con fines comerciales, siempre que se respeten las condiciones de la licencia.  
- La publicación es **global y abierta**: lo que subes se integra al ecosistema Wikimedia (Wikipedia, Wikidata, etc.).

---

### ¿Cuándo elegir cada uno?

- **Omeka**:  
  - Cuando necesitas **control total** sobre el repositorio.  
  - Si quieres publicar materiales con derechos reservados, acceso restringido o licencias específicas.  
  - Ideal para proyectos académicos, exposiciones curatoriales, colecciones patrimoniales.

- **Wikimedia Commons**:  
  - Cuando quieres **difusión global** y contribuir al conocimiento abierto.  
  - Si tu contenido puede y debe estar bajo **licencia libre**.  
  - Ideal para visibilidad, uso en Wikipedia y proyectos de cultura libre.



### Flujo práctico: subir la misma foto en Omeka vs Wikimedia Commons

Imaginemos que tienes una **fotografía histórica** tomada por ti en 2025 y quieres publicarla en ambas plataformas.

---

### Caso 1: Subir la foto en **Omeka**

**Flujo**
1. Ingresas a tu instalación de Omeka.
2. Creas un nuevo **Item** (Classic) o **Resource** (S).
3. En los metadatos (Dublin Core):
   - **Title**: "Fotografía de archivo — Plaza Central"
   - **Creator**: Natalia Rocha Díaz
   - **Date**: 2025
   - **Rights (dc:rights)**:  
     ```
     © 2025 Natalia Rocha Díaz.
     Todos los derechos reservados.
     Uso limitado a consulta académica.
     ```
4. (Opcional) Añades un plugin de **Creative Commons** si quieres licenciar bajo CC.

 **Resultado**
- La foto se muestra en tu portal de Omeka.  
- Solo las personas con permisos (ej. público general, estudiantes o investigadores) pueden acceder.  
- Tú decides si es **abierta, restringida o embargada**.  
- Los derechos los controlas totalmente: Copyright cerrado o abierto, CC, RightsStatements.org, etc.

---

### Caso 2: Subir la foto en **Wikimedia Commons**

**Flujo**
1. Entras a tu cuenta de Wikimedia Commons.
2. Subes el archivo y completas el formulario:
   - **Title**: "Plaza Central en 2025"
   - **Author**: Natalia Rocha Díaz
   - **Source**: Trabajo propio
   - **Date**: 2025
   - **License**: Debes elegir **una licencia libre**. Ejemplo:
     - CC BY-SA 4.0 (https://creativecommons.org/licenses/by-sa/4.0/)
3. Publicas el archivo.

**Resultado**
- La foto se publica **públicamente** en Commons.  
- Aparece disponible en **Wikipedia/Wikidata** y buscadores.  
- Cualquier persona puede **reutilizarla**, incluso con fines comerciales, siempre que se dé atribución y se comparta bajo la misma licencia.  
- La licencia es **irrevocable**: no puedes retractarte y cerrar el acceso después.  

---

### Diferencias clave en este ejemplo

| Aspecto | **Omeka** | **Wikimedia Commons** |
|---------|-----------|------------------------|
| **Licencia** | Tú eliges: Copyright cerrado, Creative Commons, RightsStatements.org, condiciones propias. | Obligatoriamente licencia libre (ej. CC BY, CC BY-SA, dominio público). |
| **Control de acceso** | Total: puedes restringir por rol, IP, o embargo temporal. | Ninguno: todo es abierto y global desde el inicio. |
| **Visibilidad** | Limitada a tu sitio (público o privado). | Global: inmediatamente visible y reutilizable en Wikipedia y más allá. |
| **Reversibilidad** | Puedes cambiar licencias o cerrar acceso en cualquier momento. | Irrevocable: no puedes retirar el permiso de reutilización libre una vez publicado. |
| **Objetivo** | Gestión y exhibición curatorial/académica. | Difusión global bajo principios de conocimiento libre. |

---

### Conclusión

- Si quieres **controlar la difusión y los derechos**, elige **Omeka**.  
- Si buscas **máxima visibilidad y libre reutilización**, elige **Wikimedia Commons**.  
- Una estrategia combinada puede ser: mantener en Omeka los materiales con restricciones, y subir a Commons aquellos que quieras liberar como bienes culturales abiertos.

---

---
## Otras opciones


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
