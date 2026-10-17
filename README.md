# Portafolio - John Esteban Sepúlveda Vargas

## Estructura
```
portafolio/
├── index.html
├── css/
│   ├── variables.css   (tokens de diseño)
│   ├── base.css        (reset, tipografía, layout)
│   ├── components.css  (botones, cards, modal, marcos)
│   └── animations.css
├── js/
│   └── main.js
├── assets/
│   └── cv/CV-John-Esteban-Sepulveda-Vargas.pdf   (placeholder; reemplazar por CV real)
└── README.md
```

## Cómo editar contenido
- **Datos personales**: editar en `index.html` secciones Hero (nombre), Sobre mí, Contacto.
- **Proyectos**: modificar tarjetas en sección `#projects` (título, meta, descripción, tags, enlace a GitHub).
- **Experiencia/Educación**: editar `.timeline__item` en sección `#history` (fechas, cargo, organización, lista).
- **Habilidades**: ajustar `--value` en cada `.skill__fill` (ej. `style="--value: 90%;"`).
- **Colores/tipografías**: cambiar en `css/variables.css`.
- **Animaciones**: desactiva partículas/animaciones pesadas vía `prefers-reduced-motion` (soportado). También puedes ajustar en `css/animations.css`.

## Reemplazar el CV
1. Reemplaza `assets/cv/CV-John-Esteban-Sepulveda-Vargas.pdf` por tu CV con el mismo nombre de archivo.
2. O actualiza los enlaces `href` y `src` en `index.html` (botones Descargar CV, enlace alternativo del modal, `iframe`).

## Cómo publicar (GitHub Pages, ejemplo)
1. Sube este repositorio a GitHub.
2. Ve a Settings → Pages → Build and deployment: Deploy from branch → main (o master).
3. Selecciona carpeta `/ (root)`. Se generará la URL `https://<usuario>.github.io/<repo>/`.

## Notas
- Abre `index.html` directamente (file://) sin servidor. El modal usa `<iframe>` y muestra enlace alternativo si no se visualiza el PDF.
- Sin logos, imágenes ni arte oficial de Riot Games. Todo con CSS, SVG inline y gradientes.
- Código comentado en español, clases en inglés con metodología BEM.
- Respeta `prefers-reduced-motion` (desactiva partículas). No hay scroll horizontal.
- Sin librerías externas. Solo HTML5, CSS3, JS vanilla.
