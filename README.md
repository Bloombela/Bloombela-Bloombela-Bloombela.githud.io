# Bloombela.co

Sitio web de Bloombela.co — rosas y bolsos de perlas, con envíos exclusivos en Rionegro, Antioquia. Página autocontenida en un solo archivo HTML (React + Tailwind vía CDN, sin build ni dependencias que instalar).

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser público o privado, pero para Pages gratis debe ser público).
2. Sube este archivo `index.html` a la raíz del repositorio (arrastra y suelta en la web de GitHub, o con `git push`).
3. Ve a **Settings → Pages** en el repositorio.
4. En "Build and deployment", selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. En unos minutos tu sitio quedará disponible en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Notas

- Todo el sitio vive en `index.html`: no hay que instalar nada ni correr `npm install`.
- El carrito y las reseñas se guardan en el navegador de cada visitante (`localStorage`), no en un servidor.
- Los pedidos se envían por WhatsApp al número configurado dentro del archivo (`CONFIG.WHATSAPP_NUMBER`).
- Para usar un dominio propio (como bloombela.co), configúralo en **Settings → Pages → Custom domain**.
