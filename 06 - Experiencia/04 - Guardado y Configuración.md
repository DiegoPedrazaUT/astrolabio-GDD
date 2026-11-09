# Guardado y Configuración

## Guardado

**Tipo:** Automático (previsto)

**Estado en la demo:** el guardado aún no existe. «Continuar» aparece bloqueado y «Volver al menú» avisa de que la demo no guarda el progreso. La propuesta de guardado queda pendiente de aprobación (ver [[04 - Backlog del Proyecto]]).

**Cuándo se guarda:**
- Al tomar el elevador del Pozo Celeste (diseño previsto).

Entre dos puntos de guardado, morir solo devuelve al jugador al inicio de la sala o al último checkpoint, con todo recargado. Al salir del juego, "Continuar" regresa al último punto guardado.

**Qué datos se guardan:**
- Fragmentos de estrella obtenidos.
- Habilidades entregadas (gancho y estrella ancla).
- Poemas encontrados.
- Último punto guardado (nivel).
- Muertes y tiempo de juego (para la tarjeta final).

**Cantidad de ranuras:** 3 registros (propuesta).

**Qué ocurre si el guardado falla:**
El juego avisa con un mensaje breve, sigue funcionando y reintenta en el siguiente punto de guardado. Antes de escribir, se conserva una copia de respaldo de la partida anterior.

## Configuración

| Categoría     | Opciones                                                                                             |
| ------------- | ---------------------------------------------------------------------------------------------------- |
| Audio         | Volumen general, música, efectos y ambiente                                                          |
| Video         | Pantalla completa o ventana, resolución, sincronización vertical y calidad de efectos                |
| Controles     | Reasignar teclado y mando; ver los iconos del dispositivo en uso                                     |
| Accesibilidad | Reducir temblor y movimiento, reducir destellos y ayuda de puntería (ver [[03 - Accesibilidad]])      |
| Jugabilidad   | Ayuda de puntería por dispositivo; mantener o alternar el agarre y el balanceo  |

## Restablecimiento

- Cada categoría de configuración se puede restablecer por separado.
- También hay una opción para restablecer toda la configuración.
- Borrar la partida es una acción aparte, con doble confirmación (ver [[02 - UI y Menús]]).

> **Navegación:** [[00 - Índice]] · ← [[03 - Accesibilidad]] · [[01 - Arquitectura Técnica]] →
