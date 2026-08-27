# code-art

Experimentos visuales de Artool.

## Ascenso — `burbujas.html`

Animación de fondo para web: burbujas que ascienden en un líquido viscoso semitransparente, sobre la paleta de marca (slates y púrpuras).

- **Física tipo Stokes**: velocidad terminal según radio y viscosidad, con relajación viscosa al cambiar el medio y vaivén lateral que se atenúa en medios densos.
- **Profundidad y parallax**: 4 bandas con distinta escala, velocidad, opacidad y desenfoque; las capas responden al puntero con inercia.
- **Iluminación cenital**: poza de luz radial con brillo especular y cáustica por burbuja.
- **Interacción**: clic sobre una burbuja la revienta y la divide en 2–3 hijas (conservando volumen), con onda expansiva.
- **Controles**: tono de luz, posición de la luz, viscosidad, cantidad de burbujas y rango de tamaño (slider doble mín–máx).
- Sin dependencias (Canvas 2D). Respeta `prefers-reduced-motion`.

### Uso

Abrir `burbujas.html` en el navegador, o copiar el `<canvas>`, sus estilos y el `<script>` a tu página. El canvas ya viene en `position: fixed; inset: 0`; dale `z-index: -1` para usarlo como fondo. El panel de sliders es opcional: elimínalo y fija los valores iniciales en el objeto `estado`.
