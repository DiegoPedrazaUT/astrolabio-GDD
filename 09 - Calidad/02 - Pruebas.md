# Pruebas

| Capa                                  | Resultado     | Fecha      | Qué demuestra                                                     |
| ------------------------------------- | ------------- | ---------- | ----------------------------------------------------------------- |
| Pruebas EditMode                      | 86 en verde   | 07/11/2026 | Datos, ajustes y reglas puras (por ejemplo, la cuerda de escalada) |
| Pruebas PlayMode                      | 212 en verde  | 07/11/2026 | Física y comportamiento de cada pieza dentro de una escena         |
| Análisis estático y formato           | 0 avisos      | 07/11/2026 | Código sin problemas detectables por Roslyn y con estilo uniforme  |
| Prueba a mano (teclado, ratón, mando) | Realizada por el equipo | 10/11/2026 | El recorrido se jugó; faltan por registrar los casos y los fallos |
| Build WebGL                           | No probada    | —          | —                                                                 |


Las pruebas automáticas corren en el CI de GitHub en cada PR; Windows y WebGL se compilan solo hacia `main`. EditMode cubre la configuración, `PlayerTuning`, la cuerda de escalada (`ClimbStamina`), las cajas de peligro y la interfaz. PlayMode cubre sensores, movimiento, salto, pared y escalada, reaparición, compuertas, peligros, zonas de cámara, gancho, apuntado y mando, plataformas, recogidos, nebulosa, interfaz, diálogos y elevadores, además del recorrido de la cuerda a toda velocidad. Cada mecánica llega con sus pruebas de PlayMode. Faltan las del nuevo elevador sin cambio de escena y las del guardado (TEST-01 y TEST-02 en [[04 - Backlog del Proyecto]]).

## Pruebas manuales pendientes

| ID    | Caso                                               | Objetivo                                                        |
| ----- | -------------------------------------------------- | --------------------------------------------------------------- |
| CP-01 | Entrañas del Reloj completas con teclado y ratón   | Que una persona termine las 18 salas sin ayuda                  |
| CP-02 | Entrañas del Reloj completas con mando             | Que el apuntado y los botones funcionen igual                   |
| CP-03 | Elevador del Pozo Celeste y final de la demo       | Que el elevador suba sin cambiar de escena y salgan la conversación y la tarjeta |
| CP-04 | Guardado: Continuar y Borrar registro              | Que se guarden y se recuperen sala, checkpoint, habilidades y poemas |
| CP-05 | Menús, pausa y ajustes                             | Que todas las opciones respondan y se lean                      |
| CP-06 | Build de Windows en un equipo limpio               | Que descargue, abra y corra                                     |
| CP-07 | Resoluciones 1280×720, 1600×900 y 1920×1080        | Que la interfaz y el juego se vean correctos                    |
| CP-08 | Modos del gancho (mantener, alternar, alternar con Saltar) | Que cada modo funcione con teclado y con mando          |

Las pruebas con jugadores nuevos forman parte de la etapa de pruebas del [[03 - Roadmap]]. Deben responder si entienden el gancho y la estrella ancla sin explicación, si saben por qué murieron, dónde se atascan y si quieren seguir jugando al terminar las Entrañas del Reloj.

> **Navegación:** [[00 - Índice]] · ← [[01 - Criterios de Calidad]] · [[03 - Bugs y Seguimiento]] →
