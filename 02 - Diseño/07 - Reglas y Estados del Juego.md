# Reglas y Estados del Juego

## Descripción de la sección

Define las reglas globales y los estados que puede atravesar el videojuego.

## Estados principales

- Menú principal
- Carga
- Diálogo de Efeméride (burbujas de texto)
- Jugando (libre, enganchado o escalando)
- Cambio de sala
- Muerte y reaparición
- Leyendo un poema o la carta
- Pausa
- Final
- Créditos

No existen los estados «Victoria», «Derrota» ni «Game Over»: no hay vidas y fallar solo significa reaparecer.

## Transiciones

| Estado origen        | Evento                                             | Estado destino       | Condición                                                 |
| -------------------- | -------------------------------------------------- | -------------------- | --------------------------------------------------------- |
| Menú principal       | Iniciar partida                                    | Diálogo de Efeméride | Partida nueva (el juego empieza en la Sala de los Nichos) |
| Diálogo de Efeméride | Termina la última burbuja                          | Jugando              | El jugador recupera el control                            |
| Jugando              | Toca un peligro o es aplastado                     | Muerte y reaparición | Un toque basta                                            |
| Muerte y reaparición | Al instante                                        | Jugando              | Reaparece con todo recargado y el nivel reiniciado        |
| Jugando              | El centro del jugador cruza el borde de otra sala  | Cambio de sala       | Aparece en otra zona                                      |
| Cambio de sala       | Termina la transición de cámara                    | Jugando              | El jugador toma el control                                |
| Jugando              | Obtiene un fragmento o llega al final de una zona  | Diálogo de Efeméride | Si la zona tiene conversación                             |
| Jugando              | Entra al elevador                                  | Carga                | Cambio de escena                                           |
| Carga                | Termina el ascenso                                 | Jugando              | Llega al Eje Central                                    |
| Jugando              | Pulsa Tab / Start                                  | Pausa                | Cuando el jugador tiene el control (no en cinemáticas)                                               |
| Pausa                | Elige Continuar o pulsa de nuevo Tab / Start       | Jugando              | Regresa al punto exacto donde se pausó                    |
| Jugando              | Cruza las puertas de Géminis en el Eje Central     | Final                | Termina la demo                                          |
| Final                | Termina la escena                                  | Créditos             | Al terminar, se vuelve al menú principal                                          |

## Reglas globales

1. No hay vidas ni salud: cualquier peligro o aplastamiento mata y el jugador reaparece de inmediato.
2. Reaparecer recarga todo y reinicia plataformas, cristales y anclaje.
3. Tocar suelo firme recarga el gancho, el anclaje (al instante si se usó; si no, espera de cooldown) y la cuerda.
4. Solo se agarran las superficies rugosas.
5. El gancho solo engancha en objetivos enganchables.

## Casos especiales

Documenta excepciones importantes para evitar interpretaciones diferentes durante la implementación.

- Morir enganchado libera el gancho de inmediato.
- Un checkpoint dentro de una sala larga cambia el punto de reaparición hasta que se entra en otra sala.
- El progreso se guardaría al tomar el elevador entre niveles (diseño previsto); la demo actual no guarda (ver [[04 - Guardado y Configuración]]).
- La muerte lleva al jugador al inicio de la sala o a su checkpoint.
- Aplastar al jugador entre una plataforma y un sólido, el suelo o el techo cuenta como muerte.

> **Navegación:** [[00 - Índice]] · ← [[06 - Economía y Recursos]] · [[01 - Premisa y Trama]] →
