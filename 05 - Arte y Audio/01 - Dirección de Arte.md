# Dirección de arte

Astrolabio es pixel art 2D de baja resolución, con una paleta oscura de colores cálidos y escenarios por capas de parallax. La unidad base es de 32 px: los tiles miden 32×32 px y el personaje se dibuja en 32×32 px y se muestra al doble, unos 2 tiles de alto. La vista de referencia es de 1280×720 px (40 × 22,5 tiles) y se dibuja en Aseprite. El estilo es estilizado: importa una silueta clara y legible, no el realismo.

La sensación buscada es la **inmensidad silenciosa** (ver [[04 - Pilares de Diseño]]): un mundo antiguo, solitario y oscuro, con luz cálida escasa, donde el jugador se siente pequeño pero protegido. Predominan los círculos y arcos (engranajes del tamaño de edificios, aros del Astrolabio, cúpulas) contrastados con líneas largas y rectas (cadenas, puentes, torres). Los materiales son latón envejecido, hierro oxidado, piedra pulida y rugosa, cristal y luz estelar. Las referencias son *Celeste* (legibilidad y cámara por sala), *Hollow Knight* (atmósfera y escala), *Cuphead* (carteles pintados en el escenario) y los astrolabios y relojes astronómicos antiguos.

La luz global es baja y las luces cálidas puntuales (faroles, cristales, estrellas y el Astrolabio) guían el recorrido; se complementa con un poco de bloom, viñeta y ajuste de color.

## Paleta

La paleta base es **SLSO8**, de Luis Miguel Maldonado ([Lospec](https://lospec.com/palette-list/slso8)). Cualquier color adicional se documenta como excepción en [[05 - Gestión de Cambios]].

| Código    | Uso previsto (propuesta que valida el equipo de arte)             |
| --------- | ----------------------------------------------------------------- |
| `#0d2b45` | Vacío y fondos más profundos                                      |
| `#203c56` | Fondos medios, sombras y superficies lisas                        |
| `#544e68` | Piedra y estructuras de segundo plano                             |
| `#8d697a` | Óxido apagado y detalles                                          |
| `#d08159` | Latón y cobre de las estructuras                                  |
| `#ffaa5e` | Luz cálida: faroles, cristales y brillos                          |
| `#ffd4a3` | Bordes claros de las superficies que se agarran; luz suave        |
| `#ffecd6` | Luz máxima: estrellas, Astrolabio y texto                         |

## Reglas visuales

1. El fondo es siempre más oscuro y menos saturado que el primer plano, y el personaje siempre se lee sobre él.
2. Lo que se agarra tiene textura rugosa y borde claro (`#ffd4a3`); lo liso no tiene borde ni textura.
3. Lo que se engancha brilla (`#ffecd6` y `#ffaa5e`); lo que mata se reconoce por su silueta dentada o de engranaje, nunca solo por color.
4. Se usa únicamente la paleta SLSO8, la rejilla de 32 px y *Rule Tiles*, con filtro de punto y sin deformar píxeles.
5. La luz cálida marca el camino o lo importante.

> **Navegación:** [[00 - Índice]] · ← [[05 - Misiones y Desafíos]] · [[02 - Personajes y Animación]] →
