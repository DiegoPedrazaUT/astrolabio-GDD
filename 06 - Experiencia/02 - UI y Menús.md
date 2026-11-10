# UI y menús

```text
Menú principal
├── Nueva partida
├── Continuar                      (bloqueado en la demo: no hay guardado)
├── Configuración (Audio, Video, Accesibilidad, Controles)
├── Créditos
└── Salir

Durante el juego
├── Pausa (Continuar, Configuración, Volver al menú principal)
└── Tarjeta final (al terminar la demo)
```

Los menús se manejan con teclado, ratón o mando; se confirma con Espacio o A.

| Pantalla        | Contenido y acciones                                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Menú principal  | Título, fondo del Reloj con parallax y las opciones del mapa; Nueva partida lleva al juego con un fundido                                  |
| Pausa           | Opciones sobre el juego atenuado; se abre y cierra con la misma tecla (Esc o P; Start en el mando) y no se puede abrir durante una cinemática; Continuar regresa al punto exacto |
| Configuración   | Pestañas por categoría con controles deslizantes e interruptores; los valores se prueban en el momento y se restablecen por categoría (ver [[04 - Guardado y Configuración]]) |
| Tarjeta final   | Poemas encontrados, muertes y tiempo de juego; permite ver créditos o volver al menú principal                                              |

**Confirmaciones:** Nueva partida con una partida guardada pregunta si se desea reemplazarla, volver al menú desde la pausa avisa de que se pierde el progreso, salir solo pide confirmación si hay progreso sin guardar, y restablecer la configuración pide confirmación. Borrar la partida requiere doble confirmación.

> **Navegación:** [[00 - Índice]] · ← [[01 - UX y Flujo del Jugador]] · [[03 - Accesibilidad]] →
