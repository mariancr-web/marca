# mariancr-marca-web

Hoja de estilos común y logos de la marca, para publicar una sola vez (proyecto Vercel `mariancr-marca`) y enlazar desde todas las webs.

## Publicar
1. Sube esta carpeta a un repositorio de GitHub (por ejemplo, `mariancr-marca`).
2. En Vercel: *Add New → Project*, elige el repositorio y pulsa *Deploy* (sitio estático, sin configuración).
3. Quedará en `https://mariancr-marca.vercel.app` (`index.html` es una página de muestra).

## Usar en cada web
```html
<link rel="stylesheet" href="https://mariancr-marca.vercel.app/mariancr.css">
<link rel="icon" href="https://mariancr-marca.vercel.app/logo/simbolo/mcr_general.svg">
<body class="mcr mcr-app curso-general">
```
- Cambia `curso-*` en `body` al elegir grupo (`curso-general|1eso|2eso|4eso|1bach|2bach`; los grupos A/B comparten clase).
- Componentes: `mcr-barra`, `mcr-trama-banda` + `mcr-hero`, `mcr-filtros/mcr-filtro`, `mcr-btn(--prim|--peq|--peligro|--ancho)`, `mcr-seccion`, `mcr-lista/mcr-tarjeta(--vivo|--fin)`, `mcr-vivo`, `mcr-grupos/mcr-grupo` (details), `mcr-vacio`, `mcr-acceso`, `mcr-pie-app`. Los materiales usan `mcr-caja--*`, `mcr-ejercicio`, `mcr-portada`, etc.
- Modo oscuro: `data-theme="oscuro"` en `<html>`.
- Al cambiar la marca, se edita solo `mariancr.css` aquí y se actualizan todas las webs. Las reglas están en guia-de-marca.md y guia-web-herramientas.md.
