# Mímica de películas

Juego de mímica para reuniones: una tarjeta oculta muestra una película de animación y quien actúa debe hacerla entender sin hablar. Incluye películas de Disney, Pixar y DreamWorks, con filtro por estudio, baraja que se mezcla y atajos de teclado (`espacio` revela, `→` avanza).

## Cómo ejecutarlo

Es un único archivo estático, `index.html`, sin compilación. Ábrelo en un navegador o sirve la carpeta:

```bash
python3 -m http.server 8000
```

## Notas técnicas

- HTML, CSS y JavaScript sin frameworks.
- Los carteles se piden en tiempo de ejecución a la API pública de Wikipedia; si no hay conexión se muestra un emoji de respaldo.
- Las tipografías se cargan desde Google Fonts.
- Respeta `prefers-reduced-motion` y usa atributos ARIA en los controles principales.
