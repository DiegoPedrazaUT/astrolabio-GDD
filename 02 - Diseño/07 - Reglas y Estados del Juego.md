# Reglas y estados del juego

| Estado origen        | Evento                                            | Estado destino       | Condición                                              |
| -------------------- | ------------------------------------------------- | -------------------- | ------------------------------------------------------ |
| Menú principal       | Iniciar partida                                   | Diálogo de Efeméride | Empieza en la Sala de los Nichos                       |
| Diálogo de Efeméride | Termina la última burbuja                         | Jugando              | El jugador recupera el control                         |
| Jugando              | Toca un peligro o es aplastado                    | Muerte y reaparición | Un toque basta                                         |
| Muerte y reaparición | Al instante                                       | Jugando              | Con todo recargado y la sala reiniciada                |
| Jugando              | El centro del jugador cruza el borde de otra sala | Cambio de sala       | Termina la transición de cámara y vuelve a Jugando     |
| Jugando              | Obtiene un fragmento o llega al final de una zona | Diálogo de Efeméride | Si la zona tiene conversación                          |
| Jugando              | Entra al elevador                                 | Carga                | Cambio de escena; al terminar, llega al Eje Central    |
| Jugando              | Pulsa Esc, P o Start                               | Pausa                | Solo si el jugador tiene el control (no en cinemáticas) |
| Pausa                | Continuar o pulsar de nuevo Esc, P o Start         | Jugando              | Regresa al punto exacto donde se pausó                 |
| Jugando              | Cruza las puertas de Géminis en el Eje Central    | Final                | Termina la demo y aparece la tarjeta final             |

No existen los estados «Victoria», «Derrota» ni «Game Over»: no hay vidas y fallar solo significa reaparecer.

## Reglas globales

1. Cualquier peligro o aplastamiento (entre una plataforma y un sólido, el suelo o el techo) mata y el jugador reaparece de inmediato en el inicio de la sala o en su checkpoint.
2. Reaparecer recarga todo y reinicia plataformas, cristales y estrella ancla.
3. Tocar suelo firme recarga el gancho, la estrella ancla y la cuerda.
4. Solo se agarran las superficies rugosas, y el gancho solo engancha en objetivos enganchables.
5. Morir enganchado libera el gancho de inmediato.
6. Un checkpoint dentro de una sala larga cambia el punto de reaparición hasta que se entra en otra sala.
7. La demo no guarda el progreso (ver [[04 - Guardado y Configuración]]).

> **Navegación:** [[00 - Índice]] · ← [[06 - Economía y Recursos]] · [[01 - Premisa y Trama]] →
