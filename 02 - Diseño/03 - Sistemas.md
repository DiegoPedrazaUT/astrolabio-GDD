# Sistemas

| Sistema                           | Funcionamiento actual                                                                            |
| --------------------------------- | ------------------------------------------------------------------------------------------------ |
| Movimiento y salto                | Carrera, salto variable, coyote time y jump buffer; sensores de suelo y pared                     |
| Agarre y escalada                 | Solo en superficies rugosas, con una reserva de cuerda que se recarga al tocar suelo              |
| Gancho                            | Balanceo y arrastre sobre superficies, estrellas ancla y plataformas enganchables; 2 usos         |
| Estrella ancla                    | Punto de enganche temporal que el jugador escribe en el vacío; una a la vez                       |
| Recarga                           | Suelo firme o cristal de recarga devuelven usos de gancho, estrella ancla y cuerda                |
| Plataformas móviles               | Patrulla, zip, rejillas, losas frágiles y elevadores                                              |
| Salas y cámara                    | Cada sala tiene su cámara y sus puntos de aparición; la transición dura medio segundo             |
| Muerte, reaparición y checkpoints | Reaparición en 0,4 s con todo recargado y la sala reiniciada                                      |
| Peligros                          | Engranajes, sierras, gas nebuloso (también corta el gancho), vacío y aplastamiento                |
| Coleccionables                    | Fragmento de estrella (objetivo) y poemas                                                         |
| Diálogos de Efeméride             | Burbujas de texto con disparadores por zona y la tecla de interactuar                             |
| Elevador y transición             | El elevador del Pozo Celeste sube 72 unidades en 12 s y carga el Eje Central                      |
| Guardado                          | No existe en la demo; hay una propuesta pendiente (ver [[04 - Guardado y Configuración]])         |

Los sistemas se relacionan por eventos: el reinicio de sala devuelve plataformas, cristales y estrellas ancla a su estado inicial, y la estrella ancla es siempre un objetivo del gancho. Las reglas de cada mecánica están en [[02 - Mecánicas]].

> **Navegación:** [[00 - Índice]] · ← [[02 - Mecánicas]] · [[04 - Controles]] →
