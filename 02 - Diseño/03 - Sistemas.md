# Sistemas del Juego

## Descripción de la sección

Los sistemas son conjuntos de reglas y componentes que trabajan juntos: combate, inventario, IA, diálogo, progresión, economía, misiones, etc.

## Inventario de sistemas

| Sistema                           | Propósito                                                             | Dependencias                         |
| --------------------------------- | --------------------------------------------------------------------- | ------------------------------------ |
| Movimiento y salto                | Desplazamiento de precisión                                           | Sensores de suelo y pared, entrada   |
| Agarre y escalada                 | Subir por superficies rugosas con una reserva de cuerda               | Sensor de pared, tipos de superficie |
| Gancho                            | Movilidad principal (balanceo y arrastre)                             | Entrada, superficies enganchables    |
| Anclaje de apoyo                  | Crear puntos de enganche                                              | Gancho, entrada                      |
| Recarga de usos                   | Devolver usos de gancho, anclaje y cuerda                             | Suelo, cristal de recarga            |
| Plataformas móviles               | Movimiento en el nivel                                                | Física, gancho                       |
| Salas y cámara                    | Dividir el nivel en pantallas con su propia cámara                    | Cámara, reaparición                  |
| Muerte, reaparición y checkpoints | Reintento rápido sin vidas                                            | Salas, peligros                      |
| Peligros                          | Obstáculos que matan (pinchos, vacío, aplastamiento)                  | Salas, reaparición                   |
| Observatorios y guardado          | Descanso, progreso guardado y lectura de poemas y notas               | Guardado de partida, coleccionables  |
| Coleccionables                    | Fragmentos de estrella (objetivo), poemas y notas del Almanaque XI    | Observatorios                        |
| Diálogos de Efeméride             | Burbujas de texto con disparadores por zona                           | Tecla de interactuar, zonas          |
| Ascensor y transición             | Pasar de una Casa a otra; pantalla de carga                           | Progresión, audio                    |
| Sistemas de cada Casa             | Anclaje reflejado (Géminis) y corrientes, deriva y esclusas (Acuario) | Anclaje, gancho, física              |

## Plantilla de sistema

### Nombre

**Objetivo:**

**Entradas:**

**Procesamiento / reglas:**

**Salidas:**

**Estados posibles:**

**Dependencias:**

**Interacciones:**

**Datos que necesita:**

**Datos que genera:**

**Riesgos:**

**Criterios de aceptación:**

## Sistemas documentados

### Salas, muerte y reaparición

**Objetivo:** Dividir el nivel en salas y permitir un reintento inmediato.

**Entradas:** el jugador cruza el borde de una sala; el jugador toca un peligro o es aplastado; el jugador toca un checkpoint.

**Procesamiento / reglas:**
- Cada sala tiene su cámara y uno o varios puntos de aparición. Al entrar el centro del jugador en otra sala, se activa su cámara y el punto de aparición pasa a ser el más cercano a la entrada.
- Al morir, unos segundos después el jugador reaparece con todo recargado y el nivel se reinicia (plataformas, cristales y anclaje).
- Un checkpoint dentro de una sala larga sustituye el punto de aparición hasta que se entra en otra sala.

**Salidas:** nueva cámara, nueva posición del jugador, nivel reiniciado.

**Estados posibles:** jugando, muerto, reapareciendo.

**Dependencias:** peligros, plataformas, cristales, anclaje.

**Datos que necesita:** tamaño de cada sala y posición de sus puntos de aparición.

**Datos que genera:** sala actual y contador de muertes (para las estadísticas finales).

**Riesgos:** una sala mal dimensionada puede dejar la cámara fija o cortar un balanceo; los límites de cada sala deben dejar margen.

**Criterios de aceptación:** al morir se reaparece en la sala correcta con todo recargado; cambiar de sala no pausa el juego.

### Observatorios y guardado

**Objetivo:** Dar descanso al jugador, guardar el progreso y servir de espacio de lectura.

**Entradas:** el jugador interactúa con el asiento del observatorio.

**Procesamiento / reglas:**
- El Almanaque se sienta, da cuerda a su llave y se guarda el progreso. Si el jugador sale del juego, continúa desde el último punto guardado. El progreso también se guarda al tomar el ascensor hacia otra Casa.
- Al morir, el jugador reaparece al inicio de la sala, no en el observatorio.
- Solo existen observatorios mayores: uno por Casa (el de las Dos Lentes en Géminis y el del Cauce en Acuario) y uno final (Ofiuco). Sirven para descansar, guardar, leer las notas del Almanaque XI, releer los poemas encontrados y mirar la Tierra por el telescopio.
- Efeméride nunca habla dentro de un observatorio, solo al salir.

**Estados posibles:** libre, sentado, leyendo, observando.

**Dependencias:** sistema de guardado, tecla de interactuar.

### Relaciones entre sistemas

Describe qué sistemas dependen de otros y qué información intercambian.

- El anclaje es un objetivo del gancho, y el cristal de recarga devuelve usos a ambos.
- Salas, muerte y reaparición reinician plataformas, cristales y anclajes mediante un evento de reinicio.
- Observatorios guardan los coleccionables recogidos; los diálogos de Efeméride dependen de las zonas.


> **Navegación:** [[00 - Índice]] · ← [[02 - Mecánicas]] · [[04 - Controles]] →
