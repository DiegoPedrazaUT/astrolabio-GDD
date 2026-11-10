# Reglas y estados del juego

| Estado origen        | Evento                                              | Estado destino       | Condición                                                        |
| -------------------- | --------------------------------------------------- | -------------------- | ---------------------------------------------------------------- |
| Menú principal       | Nueva partida                                       | Diálogo de Efeméride | Empieza en la Sala de los Nichos                                 |
| Menú principal       | Continuar                                           | Jugando              | Carga el registro elegido: sala o checkpoint guardado y habilidades |
| Diálogo de Efeméride | Termina la última burbuja                           | Jugando              | El jugador recupera el control                                   |
| Jugando              | Toca un peligro o es aplastado                      | Muerte y reaparición | Un toque basta                                                   |
| Muerte y reaparición | Al instante                                         | Jugando              | Con todo recargado y la sala reiniciada                          |
| Jugando              | El centro del jugador cruza el borde de otra sala   | Cambio de sala       | Termina la transición de cámara, se guarda la partida y vuelve a Jugando |
| Jugando              | Obtiene un fragmento o llega al final de una zona   | Diálogo de Efeméride | Si la zona tiene conversación                                    |
| Jugando              | Pulsa Esc, P o Start                                | Pausa                | Solo si el jugador tiene el control (no en cinemáticas)          |
| Pausa                | Continuar, o pulsar de nuevo Esc, P o Start         | Jugando              | Regresa al punto exacto donde se pausó                           |
| Pausa                | Volver al menú principal                            | Menú principal       | Guarda la partida antes de salir                                 |
| Jugando              | Entra al elevador del Pozo Celeste con el fragmento | Elevador             | El elevador sube y hace la animación de salida, sin cambiar de escena |
| Elevador             | Termina de subir                                    | Final                | Conversación final y tarjeta con las estadísticas (tiempo, muertes y poemas) |
| Final                | Pulsa «Volver al título», o pasan 30 s              | Menú principal       | Termina la demo; el registro queda guardado                      |

No existen los estados «Victoria», «Derrota» ni «Game Over»: no hay vidas y fallar solo significa reaparecer.

## Reglas globales

1. Cualquier peligro o aplastamiento (entre una plataforma y un sólido, el suelo o el techo) mata y el jugador reaparece de inmediato en el inicio de la sala o en su checkpoint.
2. Reaparecer recarga todo y reinicia plataformas, cristales y estrella ancla.
3. Tocar suelo firme recarga el gancho, la estrella ancla y la cuerda.
4. Solo se agarran las superficies rugosas, y el gancho solo engancha en objetivos enganchables.
5. Morir enganchado libera el gancho de inmediato.
6. Un checkpoint dentro de una sala larga cambia el punto de reaparición hasta que se entra en otra sala.
7. La partida se guarda sola al entrar en una sala, al tomar un checkpoint y al recibir una habilidad (ver [[04 - Guardado y Configuración]]).

> **Navegación:** [[00 - Índice]] · ← [[06 - Economía y Recursos]] · [[01 - Premisa y Trama]] →
