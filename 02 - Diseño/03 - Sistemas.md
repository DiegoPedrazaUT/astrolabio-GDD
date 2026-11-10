# Sistemas

| Sistema                           | Funcionamiento actual                                                                             |
| --------------------------------- | ------------------------------------------------------------------------------------------------- |
| Movimiento y salto                | Carrera, salto variable, coyote time y jump buffer; sensores de suelo y pared                      |
| Agarre y escalada                 | Solo en superficies rugosas, con una reserva de cuerda que se recarga al tocar suelo o con un cristal |
| Gancho                            | Balanceo y arrastre sobre superficies, faroles y estrellas ancla; 2 usos; el balanceo tiene tiempo límite |
| Estrella ancla                    | Punto de enganche temporal que el jugador escribe en el vacío; una a la vez                        |
| Recarga                           | Suelo firme o cristal de recarga devuelven usos de gancho, estrella ancla y cuerda                 |
| Plataformas móviles               | Patrulla, zip, rejillas, losas frágiles y elevadores; se pisan y se agarran, no se enganchan       |
| Salas y cámara                    | Cada sala tiene su cámara y sus puntos de aparición; la transición dura medio segundo              |
| Muerte, reaparición y checkpoints | Reaparición en 0,4 s con todo recargado y la sala reiniciada                                       |
| Peligros                          | Engranajes, sierras, nebulosa (también corta el gancho), vacío y aplastamiento                     |
| Coleccionables                    | Fragmento de estrella (objetivo) y poemas, que se leen en un panel al recogerlos                   |
| Diálogos de Efeméride             | Burbujas de texto con disparadores por zona; se avanzan o se saltan con Aceptar                    |
| Elevador y final de la demo       | El elevador del Pozo Celeste sube 72 unidades en 12 s sin cambiar de escena; al terminar, conversación final y tarjeta de estadísticas |
| Guardado                          | Automático en 3 registros (ver más abajo y [[04 - Guardado y Configuración]])                      |

Los sistemas se relacionan por eventos: el reinicio de sala devuelve plataformas, cristales y estrellas ancla a su estado inicial, y la estrella ancla es siempre un objetivo del gancho. Las reglas de cada mecánica están en [[02 - Mecánicas]].

## Guardado

El juego guarda solo, sin que el jugador lo pida: al entrar en una sala, al tomar un checkpoint y al recibir una habilidad. Cada registro conserva la sala y el checkpoint, las habilidades, los poemas recogidos, las conversaciones ya vistas, los elevadores de solo ida usados, las muertes, el tiempo de juego y la fecha. Las plataformas, los cristales, las losas y las compuertas no se guardan: se reinician con la sala. El detalle está en [[04 - Guardado y Configuración]] y [[04 - Datos y Persistencia]].

> **Navegación:** [[00 - Índice]] · ← [[02 - Mecánicas]] · [[04 - Controles]] →
