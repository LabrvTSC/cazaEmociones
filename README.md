# Juegos de emociones

Dos minijuegos web para descubrir cómo se pueden representar, generar y "medir" las emociones con tecnología. Se crearon para la charla "Mi viaje al mundo virtual", del programa "Ciencia y Tecnología en Femenino" de Sevilla TechPark, dirigida a estudiantes de Educación Secundaria.

**Jugar:** https://labrvtsc.github.io/cazaEmociones/

No hace falta instalar nada: funcionan directamente en el navegador.

---

## Los juegos

### Caza de emociones (móvil · realidad aumentada)
`caza.html`

Las emociones aparecen flotando por la habitación, sobre la imagen de la cámara del móvil. Hay que girar el móvil para encontrarlas y tocarlas para cazarlas antes de que pasen 60 segundos.

- 7 emociones, cada una con su criatura: alegría, tristeza, miedo, ira, asco, sorpresa y calma.
- **Emoción dorada:** aparece de vez en cuando, es rápida y vale +5.
- **Artefactos rojos:** representan el "ruido" que estropea una señal. Si los tocas, pierdes 3 puntos.
- Combos, una misión aleatoria al empezar y un "frenesí" de puntos dobles en los últimos 10 segundos.
- Al terminar aparece **tu mapa de emociones**, que se puede guardar como imagen.

### Crea una emoción (ordenador y móvil · mundos 3D y música)
`crea.html`

Eliges una emoción y el programa genera en directo un mundo 3D con su paisaje, sus colores, sus seres, su clima y una música compuesta al momento. Ningún mundo se repite. Mientras viajas, hay que atravesar anillos de luz ("señal limpia") y esquivar artefactos rojos ("ruido"), con una señal EEG simulada en pantalla.

**Controles en el ordenador:**

| Tecla | Acción |
|---|---|
| A D o ← → | Moverse a izquierda y derecha |
| W S o ↑ ↓ | Subir y bajar |
| 1 – 7 | Elegir emoción |
| Espacio | Generar otro mundo |
| M | Mapa de emociones: viajar mezclando emociones |
| N | Silenciar la música |
| Esc | Volver al menú |

En el móvil se juega con botones en pantalla o arrastrando el dedo.

---

## La ciencia que hay detrás

- **Emociones básicas.** Las seis emociones de Paul Ekman (alegría, tristeza, miedo, ira, asco y sorpresa), más la calma.
- **Modelo circumplejo de Russell.** Coloca cada emoción en un mapa con dos ejes: lo agradable o desagradable que es (valencia) y lo activado o relajado que te deja (activación). El mapa final de los dos juegos usa este modelo.
- **Señales cerebrales (EEG) y ruido.** En investigación se registran señales EEG mientras una persona vive una experiencia en realidad virtual. Los "artefactos" son interferencias que contaminan la señal y hay que eliminarlas. En los juegos, la señal EEG es una simulación con fines divulgativos: no se mide nada real.

## Privacidad

"Caza de emociones" usa la cámara y los sensores de movimiento del móvil solo para mostrar las criaturas sobre la imagen. **No se graba, no se guarda ni se envía nada.** Ninguno de los dos juegos recoge datos personales.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | Menú principal con los dos juegos |
| `caza.html` | Caza de emociones |
| `crea.html` | Crea una emoción |

Cada juego es un único archivo HTML autocontenido, que incluye [three.js](https://threejs.org/) para el 3D. La música se genera con la Web Audio API del navegador. "Caza de emociones" necesita HTTPS para usar la cámara, que es lo que ofrece GitHub Pages.

## Autoría

Irene Fondón García · Departamento de Teoría de la Señal y Comunicaciones, Escuela Técnica Superior de Ingeniería, Universidad de Sevilla.

Desarrollado con ayuda de Claude (Anthropic).
