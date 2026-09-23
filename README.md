# Proyecto VR — sitio del curso

## Ver en local
Abre `index.html` directamente en el navegador (doble clic) o, mejor aún,
sirve la carpeta con un servidor simple para que las rutas de imágenes/videos
carguen bien:

```
cd proyecto-vr
python3 -m http.server 8000
```

y entra a `http://localhost:8000`.

## Estructura
```
proyecto-vr/
├── index.html      → todo el contenido y las 3 secciones
├── css/style.css   → estilos
├── js/script.js    → menú móvil, sección activa, efecto de linterna
├── images/         → pon aquí tus fotos y capturas
└── videos/         → pon aquí los videos de las pruebas de usuario
```

## Cómo completar las secciones 2 y 3
- **Sección "Desarrollo"**: reemplaza `images/desarrollo-1.jpg`, `-2.jpg`, `-3.jpg`
  por tus capturas reales de Unity/modelos (mismo nombre, o cambia el `src`
  en `index.html`). Duplica el bloque `<article class="dev-item">...</article>`
  para agregar más avances, y edita el texto de introducción marcado con
  un comentario `<!-- -->`.
- **Sección "Pruebas de usuario"**: coloca tus videos en `videos/prueba-1.mp4`,
  etc. (formato `.mp4` recomendado por compatibilidad), y una miniatura
  opcional en `images/video-poster-1.jpg`. Duplica `<article class="test-item">`
  para cada usuario.
- Si una imagen aún no existe, la tarjeta muestra automáticamente el aviso
  "Añade una imagen en /images" en vez de romperse.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub y sube todo el contenido de esta carpeta
   (el `index.html` debe quedar en la raíz del repo, o en `/docs` si prefieres
   esa opción).
2. En el repo: **Settings → Pages → Source**, elige la rama (`main`) y la
   carpeta (`/root` o `/docs`).
3. Guarda; GitHub te dará una URL tipo
   `https://tu-usuario.github.io/tu-repo/` en un par de minutos.

## Videos pesados
Si los videos de las pruebas de usuario pesan mucho, GitHub Pages puede ir
lento. Alternativas: subirlos a YouTube (aunque sea "no listado") e incrustar
un `<iframe>` en vez de la etiqueta `<video>`, o comprimirlos antes de subirlos.
