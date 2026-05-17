# Dr. Gerardo Félix Ramos · Landing

Sitio web personal del Dr. Gerardo Félix Ramos · Pediatra · Medicina Crítica Pediátrica · Hermosillo, Sonora.

## Contenido del paquete

```
deploy/
├── index.html          ← Página principal (renombrar al subir si se desea)
├── images/             ← Fotos del doctor, consultorio e Instagram
└── README.md           ← Este archivo
```

## Cómo publicarlo

### Opción A — Hosting estático (recomendado)

Cualquiera de estos funciona sin configuración:

- **Vercel** — `vercel deploy` desde la carpeta `deploy/`
- **Netlify** — arrastra la carpeta `deploy/` a [app.netlify.com/drop](https://app.netlify.com/drop)
- **GitHub Pages** — sube la carpeta a un repositorio, activa Pages en Settings
- **Cloudflare Pages** — conecta el repo o sube como ZIP

### Opción B — Hosting tradicional (cPanel / hosting compartido)

Sube el contenido de `deploy/` por FTP a la raíz del dominio (`public_html/` o `www/`).

## Dominio

El sitio está preparado para `drgerardofelix.com`. Si usas otro dominio, actualiza:

- `<link rel="canonical">` en el `<head>`
- `<meta property="og:url">`
- Las URLs en el bloque JSON-LD (`@id`, `url`, `image`)

## Fotos pendientes

El landing ya referencia las siguientes imágenes — las que estén en la carpeta `images/` se muestran solas, las que falten se verán como placeholder:

| Archivo                       | Uso                                  |
|-------------------------------|--------------------------------------|
| `dr-gerardo-portrait.png`     | Retrato principal (hero)             |
| `dr-gerardo-consulta.png`     | Foto secundaria (sección sobre)      |
| `consultorio-1.png` … `-4.png`| Galería del consultorio              |
| `ig-1.png` … `ig-6.png`       | Grid de publicaciones de Instagram   |
| `og-cover.png`                | Vista previa al compartir en redes   |

**Para reemplazar/agregar fotos:** solo coloca el archivo con el nombre correspondiente dentro de `images/`. No necesitas tocar el HTML.

## Datos y links

Toda la info está editada directo en `index.html`. Si cambia algo (teléfono, dirección, email, horarios, publicaciones), edita el HTML — está organizado por secciones con comentarios claros.

- **WhatsApp:** `+52 644 146 0765`
- **Correo:** `contacto@drgerardofelix.com`
- **Consultorio:** Hospital San José · Hermosillo, Sonora

## Notas técnicas

- Sin dependencias de build — es HTML/CSS/JS plano
- Fuentes Google (Fraunces + Inter) cargan desde CDN
- Mapa embebido de Google Maps
- Sin tracking ni cookies (puedes agregarlos si los necesitas)

—

Última actualización: mayo 2026
