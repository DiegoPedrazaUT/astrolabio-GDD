# Pruebas

| Capa                                  | Resultado     | Fecha      | Qué demuestra                                                     |
| ------------------------------------- | ------------- | ---------- | ----------------------------------------------------------------- |
| Pruebas EditMode                      | 86 en verde   | 07/11/2026 | Datos, ajustes y reglas puras (por ejemplo, la cuerda de escalada) |
| Pruebas PlayMode                      | 212 en verde  | 07/11/2026 | Física y comportamiento de cada pieza dentro de una escena         |
| Análisis estático y formato           | 0 avisos      | 07/11/2026 | Código sin problemas detectables por Roslyn y con estilo uniforme  |
| Prueba a mano (teclado, ratón, mando) | No realizada  | —          | —                                                                 |
| Build WebGL                           | No probada    | —          | —                                                                 |


Las pruebas automáticas corren en el CI de GitHub en cada PR; Windows y WebGL se compilan solo hacia `main`. EditMode cubre la configuración, `PlayerTuning`, la cuerda de escalada (`ClimbStamina`), las cajas de peligro y la interfaz. PlayMode cubre sensores, movimiento, salto, pared y escalada, reaparición, compuertas, peligros, zonas de cámara, gancho, apuntado y mando, plataformas, recogidos, gas, interfaz, diálogos y llegada del elevador, además del recorrido de la cuerda a toda velocidad. Cada mecánica llega con sus pruebas de PlayMode.

## Pruebas manuales pendientes

| ID    | Caso                                               | Objetivo                                                        |
| ----- | -------------------------------------------------- | --------------------------------------------------------------- |
| CP-01 | Tutorial completo con teclado y ratón              | Que una persona termine las 18 salas sin ayuda                  |
| CP-02 | Tutorial completo con mando                        | Que el apuntado y los botones funcionen igual                   |
| CP-03 | Elevador del Pozo Celeste y llegada al Eje Central | Que el cambio de escena conserve el control y las habilidades   |
| CP-04 | Cierre de la demo en las puertas de Géminis        | Que la demo termine con claridad                                |
| CP-05 | Menús, pausa y ajustes                             | Que todas las opciones respondan y se lean                      |
| CP-06 | Build de Windows en un equipo limpio               | Que descargue, abra y corra                                     |
| CP-07 | Resoluciones 1280×720, 1600×900 y 1920×1080        | Que la interfaz y el juego se vean correctos                    |

Las pruebas con jugadores nuevos forman parte de la etapa de pruebas del [[03 - Roadmap]]. Deben responder si entienden el gancho y la estrella ancla sin explicación, si saben por qué murieron, dónde se atascan y si quieren seguir jugando al terminar el tutorial.

> **Navegación:** [[00 - Índice]] · ← [[01 - Criterios de Calidad]] · [[03 - Bugs y Seguimiento]] →
