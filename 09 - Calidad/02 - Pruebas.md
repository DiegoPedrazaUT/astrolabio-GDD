# Pruebas

## Descripción de la sección

Define cómo se comprueba que Astrolabio funciona como fue diseñado y registra qué se probó, cuándo y con qué resultado.

## Resumen de resultados

| Capa | Resultado | Fecha | Qué demuestra |
| --- | --- | --- | --- |
| Pruebas EditMode | 86 en verde | 07/11/2026 | Datos, ajustes y reglas puras (por ejemplo la cuerda de escalada) |
| Pruebas PlayMode | 212 en verde | 07/11/2026 | Física y comportamiento de cada pieza dentro de una escena |
| Análisis estático | 0 avisos | 07/11/2026 | Código sin problemas detectables por Roslyn |
| Formato | Limpio | 07/11/2026 | Estilo de código uniforme |
| Prueba a mano (teclado, ratón, mando) | No realizada | — | — |
| Build WebGL | No probada | — | — |

> [!warning] Límite de estas cifras
> Que las pruebas automáticas pasen **no** quiere decir que el juego sea agradable ni que esté libre de errores. Cubren lo que alguien pensó en comprobar. La sensación del salto, la dificultad y la legibilidad del nivel necesitan jugadores.

## Pruebas automáticas

Se ejecutan en el CI de GitHub en cada PR. Las compilaciones de Windows y WebGL se hacen solo hacia `main`.

### EditMode

Configuración del proyecto, valores del jugador (`PlayerTuning`), la cuerda de escalada (`ClimbStamina`), las cajas de peligro, el contenido de la interfaz y el vestido del personaje.

### PlayMode

Sensores de suelo y pared, movimiento, salto, pared y escalada, reaparición y muerte, compuertas, peligros pintados con tiles, zonas de cámara, hilo, apuntado y mando, plataformas (patrulla, zip, elevador, rejillas y losas), recogidos, gas, jugador sobre plataformas, metal estelar, interfaz, diálogos, fondo y llegada del elevador, y el recorrido de la cuerda a toda velocidad (1350 recorridos).

### Reglas del repositorio

- Cada mecánica llega con sus pruebas de PlayMode.
- Una prueba inconclusa cuenta como fallo.
- Las pruebas que no pueden correr en el servidor usan `Assert.Ignore`.

## Pruebas manuales

Estos casos están preparados y **todavía no se ejecutaron**. Cada uno se rellena con el formato de la sección siguiente.

| ID | Caso | Objetivo | Estado |
| --- | --- | --- | --- |
| CP-01 | Tutorial completo con teclado y ratón | Que una persona termine las 18 salas sin ayuda | Sin ejecutar |
| CP-02 | Tutorial completo con mando | Que el apuntado y los botones funcionen igual | Sin ejecutar |
| CP-03 | Elevador del Pozo Celeste y llegada al Eje Central | Que el cambio de escena conserve el control y las habilidades | Sin ejecutar |
| CP-04 | Cierre de la demo en las puertas de Géminis | Que la demo termine con claridad | Sin ejecutar |
| CP-05 | Menús, pausa y ajustes | Que todas las opciones respondan y se lean | Sin ejecutar |
| CP-06 | Build de Windows en un equipo limpio | Que descargue, abra y corra | Sin ejecutar |
| CP-07 | Resoluciones 1280×720, 1600×900 y 1920×1080 | Que la interfaz y el juego se vean correctos | Sin ejecutar |

## Pruebas con jugadores nuevos

Etapa **Pruebas** del [[03 - Roadmap]]. Preguntas que debe contestar:

- ¿Entienden el hilo y la estrella-anclaje sin que se les explique?
- ¿Saben por qué murieron?
- ¿Dónde se atascan y cuánto tardan en cada sala?
- ¿Quieren seguir jugando al terminar el tutorial?

## Caso de prueba (formato)

### Nombre

**Objetivo:**

**Precondiciones:**

**Pasos:**

1.
2.
3.

**Resultado esperado:**

**Resultado obtenido:**

**Estado:** Correcto / Incorrecto


> **Navegación:** [[00 - Índice]] · ← [[01 - Criterios de Calidad]] · [[03 - Bugs y Seguimiento]] →
