# Guardado y configuración

## Guardado

**Tipo:** automático, en 3 registros. La propuesta quedó aprobada el 10/11/2026 y se implementa antes de la entrega.

**Cuándo se guarda:**

- Al entrar en una sala nueva.
- Al tomar un checkpoint.
- Al recibir una habilidad.

Un indicador pequeño («Guardando…») aparece en el HUD mientras se escribe. Entre dos guardados, morir solo devuelve al jugador al inicio de la sala o al último checkpoint, con todo recargado. «Volver al menú» desde la pausa también guarda.

**Qué se guarda en cada registro:**

- Escena y sala (el nombre de cada sala es único) y el checkpoint tomado, si lo hay: ahí reaparece el jugador.
- Habilidades (gancho y estrella ancla).
- Poemas recogidos y conversaciones ya vistas.
- Elevadores de solo ida ya usados.
- Muertes, tiempo de juego y fecha.
- Una miniatura de la partida (320 × 180, sin interfaz).

**Qué no se guarda:** plataformas, cristales, losas y compuertas; se reinician con la sala.

**Dónde:** un archivo JSON por registro y su miniatura, en la carpeta de datos persistentes (en la versión web, en el almacenamiento del navegador). Los ajustes van aparte (ver [[04 - Datos y Persistencia]]).

**Pantalla de registros:** Continuar queda habilitado cuando hay registros. Nueva partida pide elegir uno y confirma antes de sobrescribirlo. Cada tarjeta muestra zona, sala, tiempo, fecha, muertes, poemas y el progreso real.

**En el evento:** el registro se reinicia a mano entre jugador y jugador con «Borrar registro» (Supr en teclado, X en mando). No hay modo evento ni atajo oculto.

**Si el guardado falla:** el juego avisa con un mensaje breve, sigue funcionando y reintenta en el siguiente punto de guardado; antes de escribir se conserva una copia de la partida anterior.

## Configuración

| Categoría   | Opciones                                                                                                  |
| ----------- | --------------------------------------------------------------------------------------------------------- |
| Audio       | Volumen general, música, efectos y ambiente                                                               |
| Idioma      | Selector de idioma (español; la traducción al inglés llega después de la demo)                            |
| Jugabilidad | Ayuda de puntería por dispositivo y modo del gancho (ver abajo)                                           |

**Modos del gancho** (teclado y mando):

1. Mantener pulsado el botón; al soltarlo, el gancho se corta (predeterminado).
2. Pulsar para enganchar y pulsar otra vez para soltar.
3. Pulsar para enganchar y pulsar Saltar para soltar.

Cada categoría se puede restablecer por separado, y también toda la configuración. Los controles no se pueden reasignar. Borrar un registro es una acción aparte, con confirmación (ver [[02 - UI y Menús]]).

> **Navegación:** [[00 - Índice]] · ← [[03 - Accesibilidad]] · [[01 - Arquitectura Técnica]] →
