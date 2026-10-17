# Dirección de Arte

## Descripción de la sección

Define la identidad visual del videojuego y las reglas que deben seguir los recursos gráficos.

## Identidad visual

**Estilo:**
Pixel art 2D de baja resolución, con una paleta oscura con colores calidos y escenarios por capas de parallax. La unidad base es de 16 px: los tiles miden 16×16 px y el personaje, 32×32 px. Se dibuja en Aseprite.

**Referencias:**
- *Celeste*: legibilidad de las superficies, cámara por sala y pixel art de baja resolución.
- *Hollow Knight*: atmósfera solitaria y escala monumental frente a un protagonista pequeño.
- *Cuphead*: carteles de controles pintados dentro del escenario.
- Astrolabios, relojes astronómicos y mapas estelares antiguos como referencia de formas.

**Sensación buscada:**
Inmensidad silenciosa: un mundo antiguo, solitario y oscuro, con luz cálida escasa (ver [[04 - Pilares de Diseño]], Pilar 1). El jugador debe sentirse pequeño, pero protegido.

**Nivel de realismo:**
Estilizado. No se busca realismo: se busca una silueta clara y una forma legible incluso a 640×360 px.

**Formas predominantes:**
Círculos y arcos (engranajes, aros del Astrolabio, cúpulas) contrastados con líneas largas y rectas (cadenas, puentes, torres). Los engranajes tienen el tamaño de edificios; el personaje es diminuto.

**Iluminación:**
Luz global baja y luces cálidas puntuales (faroles, cristales, estrellas y el Astrolabio) que guían el recorrido. El fondo siempre es más oscuro y menos saturado que el primer plano. Se complementa con un poco de bloom, viñeta y ajuste de color.

**Materiales:**
Latón envejecido, hierro oxidado, piedra pulida y piedra rugosa, cristal y luz estelar. Cada Casa añade su carácter: Géminis (dorado pulido frente a hierro oxidado) y Acuario (ánfora agrietada y cascadas de luz).

## Paleta de color

La paleta base es **SLSO8**, de Luis Miguel Maldonado ([Lospec](https://lospec.com/palette-list/slso8)). Es una decisión del equipo; si hiciera falta un color adicional por Casa, se documenta como excepción en el [[03 - Registro de Decisiones]].

| Muestra | Código    | Uso previsto (propuesta que valida el equipo de arte)                       |
| ------- | --------- | --------------------------------------------------------------------------- |
| 1       | `#0d2b45` | Vacío y fondos más profundos                                                |
| 2       | `#203c56` | Fondos medios, sombras y superficies lisas                                  |
| 3       | `#544e68` | Piedra y estructuras de segundo plano                                       |
| 4       | `#8d697a` | Óxido apagado y detalles                                                    |
| 5       | `#d08159` | Latón y cobre de las estructuras                                            |
| 6       | `#ffaa5e` | Luz cálida: faroles, cristales y brillos                                    |
| 7       | `#ffd4a3` | Bordes claros de las superficies que se agarran; luz suave                  |
| 8       | `#ffecd6` | Luz máxima: estrellas, Astrolabio y texto                                   |

**Colores principales:**
`#0d2b45`, `#203c56`, `#d08159` y `#ffaa5e`.

**Colores secundarios:**
`#544e68`, `#8d697a`, `#ffd4a3` y `#ffecd6`.

**Colores para información jugable:**
- Superficies que se agarran: textura rugosa y borde claro (`#ffd4a3`).
- Superficies que se enganchan (metal estelar) y anclajes: brillo propio con `#ffecd6` y `#ffaa5e`.
- Peligros: silueta dentada o de engranaje con contraste fuerte contra el fondo; nunca se distinguen solo por color.
- Recursos (usos del gancho y del anclaje, cuerda): anillos y llave del Astrolabio en la interfaz.

## Reglas visuales

1. El fondo siempre es más oscuro y menos saturado que el primer plano.
2. Lo que se puede agarrar tiene textura rugosa y borde claro; lo liso no tiene borde ni textura.
3. Lo que se puede enganchar brilla; lo que mata se reconoce por su silueta.
4. Se usa únicamente la paleta SLSO8 (más las excepciones documentadas).
5. Se respeta la rejilla de 16 px y se escala solo con múltiplos enteros (×3 en 1080p) para evitar píxeles de tamaños distintos.
6. El personaje siempre se lee sobre el fondo: nunca se coloca un detalle del fondo con el mismo contraste que el personaje.
7. La luz cálida marca el camino o lo importante.

## Referencias

- [Paleta SLSO8 en Lospec](https://lospec.com/palette-list/slso8)
- *Celeste* (Maddy Makes Games), *Hollow Knight* (Team Cherry) y *Cuphead* (Studio MDHR).
- Imágenes de referencia: agregar dentro de la carpeta del proyecto.


> **Navegación:** [[00 - Índice]] · ← [[05 - Misiones y Desafíos]] · [[02 - Personajes y Animación]] →
