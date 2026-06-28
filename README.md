# Vertex Code (Sitio Web)

Proyecto web **estático** para la marca **Vertex Code | Desarrollo de Software e IA**.

Incluye una landing page con:
- Navbar fija con navegación por secciones.
- Sección hero (texto + imagen).
- Bloques informativos (“Nosotros” y “Servicios”).
- Footer con datos de contacto.
- Estilos principales y responsivos.

---

## Estructura del proyecto

- `index.html`
  - Estructura base del sitio.
  - Carga los estilos y recursos del proyecto.
  - Carga Bootstrap e iconos desde CDN.
  - Incluye Bootstrap JS (bundle) y `app.js`.

- `css/`
  - `style.css`: estilos principales (tipografía, layout, hero, cards, footer, etc.).
  - `responsive.css`: ajustes para diferentes tamaños de pantalla.

- `assets/`
  - `logo.png`, `image.png`, `image-baner.png` (imágenes usadas en la landing).

- `app.js`
  - Lógica del front (por ejemplo, interacciones y/o helpers del sitio).

---

## Verificación de URLs de estilos (CSS)

Objetivo: asegurar que las referencias a hojas de estilo en `index.html` **no apunten a rutas inexistentes**.

En `index.html` se cargan los siguientes CSS:
- `css/style.css`
- `css/responsive.css`

✅ Ambas rutas existen físicamente dentro del proyecto (`css/`).

---

## Cómo ejecutar / ver el sitio

Como el proyecto es estático, tienes dos opciones:

1) **Abrir directamente**
- Abre `index.html` con tu navegador.

2) **Recomendado: servidor local** (evita problemas de rutas y cache)
- Usa una herramienta como **VSCode Live Server**.
- Esto levanta un servidor local para que las rutas (`css/...`, `assets/...`) funcionen de forma consistente.

---

## Dependencias externas

El HTML usa componentes desde CDN:
- **Bootstrap CSS**: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/...`
- **Bootstrap Icons**: `https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/...`
- **Bootstrap Bundle (JS)**: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/...`

No se requieren instaladores/compilaciones adicionales porque los recursos se consumen vía CDN.

---

## Notas de mantenimiento

- Si agregas nuevas secciones al HTML, respeta la convención de IDs y clases para mantener el estilo.
- Si agregas nuevos estilos, por lo general:
  - coloca estilos globales en `css/style.css`.
  - coloca ajustes para breakpoints en `css/responsive.css`.
- Si cambias nombres de archivos CSS o imágenes, actualiza siempre las rutas en `index.html`.


