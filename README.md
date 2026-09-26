# Bloombela.co

Sitio web de Bloombela.co — rosas y bolsos de perlas, con envíos exclusivos en Rionegro, Antioquia. Página autocontenida en un solo archivo HTML (React + Tailwind vía CDN, sin build ni dependencias que instalar).

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (público para Pages gratis).
2. Sube el archivo `index.html` a la raíz del repositorio.
3. Ve a **Settings → Pages**.
4. En "Build and deployment", selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. En unos minutos tu sitio quedará disponible en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Notas

- Todo el sitio vive en `index.html`: no hay que instalar nada ni correr `npm install`.
- El carrito y las reseñas se guardan en el navegador de cada visitante (`localStorage`).
- Los pedidos se envían por WhatsApp al número configurado dentro del archivo (`CONFIG.WHATSAPP_NUMBER`).
- Para usar un dominio propio, configúralo en **Settings → Pages → Custom domain**.
- El sitio es mobile-first y funciona correctamente en iOS (incluye `env(safe-area-inset-*)`) y Android.

## Correcciones aplicadas (v2 responsive)

- SVG con `width`/`height` intrínsecos para evitar iconos gigantes si Tailwind CDN tarda en cargar.
- Botón flotante de WhatsApp con CSS puro (no depende de Tailwind) y adaptado a notch/isla dinámica.
- Eliminado `overflow-x` accidental en drawers y modales.
- Imágenes con `max-width: 100%`, `loading="lazy"` y `decoding="async"`.
- Uso de `100dvh` en lugar de `100vh`.
- Corrección de clase inexistente `h-88` → `h-96`.
