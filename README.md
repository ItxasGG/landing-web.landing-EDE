# Landing de diseño web · Estrategia Digital Estrella

Landing estática (HTML, CSS y JavaScript sin frameworks) para los servicios de diseño de landing pages y páginas web. No necesita paso de compilación.

## Estructura

```
index.html     Página
styles.css     Estilos (mobile first)
script.js      Mejoras ligeras (acordeón y animaciones)
_headers       Cabeceras de seguridad y caché para Cloudflare Pages
assets/        Imágenes
```

## Imágenes y dominio

- Imágenes en `assets/`: `logo-rojo.png` (cabecera), `logo-negro.png` (pie, versión blanca para fondo negro), `banner.png` (hero), `favicon.png` (512 × 512 px) y `og-image.png` (1200 × 630 px, para redes).
- Dominio configurado en `index.html`: `web.estrategiadigitalestrella.com`. Si cambia, busca y sustituye esa dirección.

## Publicar en Cloudflare Pages

1. Sube el proyecto a un repositorio de GitHub.
2. En el panel de Cloudflare, ve a **Workers y Pages › Crear › Pages › Conectar a Git** y elige el repositorio.
3. Configuración de compilación:
   - Framework: **Ninguno**
   - Comando de compilación: *(vacío)*
   - Directorio de salida: `/`
4. Pulsa **Guardar e implementar**. Cada `push` a `main` publicará la nueva versión automáticamente.
5. Para usar el dominio, entra en el proyecto › **Dominios personalizados** › **Configurar un dominio**, escribe `web.estrategiadigitalestrella.com` y sigue los pasos.

## Vista previa en local

```
python3 -m http.server 8000
```

Y abre http://localhost:8000
