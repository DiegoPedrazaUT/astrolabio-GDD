# UI y menús

```text
Menú principal
├── Jugar
│   ├── Nueva partida              (elige uno de los 3 registros)
│   └── Continuar                  (solo si hay una partida guardada)
├── Configuración (Audio, Idioma, Jugabilidad)
├── Créditos
└── Salir

Durante el juego
├── Pausa (Continuar, Configuración, Volver al menú principal)
└── Tarjeta final (al terminar la demo)
```

Los menús se manejan con teclado, ratón o mando; se confirma con Espacio o A.

| Pantalla        | Contenido y acciones                                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Splash Screen   | Pantalla de inicio con el título, el arte de fondo y el texto parpadeante «Presiona cualquier botón para continuar»; cualquier tecla o botón pasa al menú principal con una animación |
| Menú principal  | Título, fondo del Reloj con parallax y las opciones del mapa. Jugar abre la lista de registros; Nueva partida y Continuar llevan al juego con una pantalla de carga |
| Registros       | Tres registros. Cada tarjeta muestra zona, sala, tiempo de juego, fecha, muertes, poemas, progreso y una miniatura. Se puede borrar un registro con Supr (teclado) o X (mando) |
| Pausa           | Opciones sobre el juego atenuado; se abre y cierra con la misma tecla (Esc o P; Start en el mando) y no se puede abrir durante una cinemática; Continuar regresa al punto exacto |
| Configuración   | Pestañas por categoría (Audio, Idioma y Jugabilidad) con controles deslizantes e interruptores; se restablecen por categoría (ver [[04 - Guardado y Configuración]]) |
| Tarjeta final   | «Gracias por jugar la demo» y las estadísticas: tiempo de juego, muertes y poemas encontrados. El botón «Volver al título» regresa al menú; si nadie lo pulsa, vuelve solo a los 30 s |
| Créditos        | Nombres del equipo, qué hizo cada integrante, recursos externos y agradecimientos; se puede acelerar o volver al menú, y termina con un fundido |

**Confirmaciones:**

| Acción del jugador                       | Respuesta del sistema                                                  |
| ---------------------------------------- | ---------------------------------------------------------------------- |
| Nueva partida sobre un registro ocupado  | Pide confirmación para sobrescribirlo                                  |
| Volver al menú principal desde la pausa  | Guarda la partida antes de volver                                      |
| Salir del juego                          | Pide confirmación                                                      |
| Restablecer configuración                | Pide confirmación para volver a los valores predeterminados            |
| Borrar un registro                       | Pide confirmación y se hace aparte del resto de las opciones           |

> **Navegación:** [[00 - Índice]] · ← [[01 - UX y Flujo del Jugador]] · [[03 - Accesibilidad]] →
