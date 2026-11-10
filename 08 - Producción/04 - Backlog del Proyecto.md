# Entregas y trabajo pendiente

| Área | Estado al 10 de noviembre |
| --- | --- |
| Jugador | Movimiento, salto, pared, escalada con cuerda, gancho y estrella ancla integrados, con pruebas automáticas. |
| Nivel | Salas con cámara, checkpoints, compuertas, plataformas (patrulla, zip, rejillas, losas) y cristales. |
| Peligros | Engranajes, sierras y nebulosa (mata y corta el gancho). |
| Arte | Almanaque con 13 animaciones, tiles de las Entrañas con Rule Tiles de 32 × 32, fondo y decorado. |
| Elevadores | De solo ida en la sala 10 y del Pozo Celeste; este último pasa a cerrar la demo sin cambio de escena (END-01). |
| Audio | Efectos y música por sala integrados. |
| Interfaz | Menús, pausa, ajustes, créditos, HUD y caja de diálogo en UI Toolkit. |
| Calidad | 86 pruebas de EditMode y 212 de PlayMode en verde; análisis estático sin avisos (7 de noviembre). |
| Documentación | GDD alineado con la demo; registro visual con la procedencia de las imágenes. |

## Integraciones cerradas

| ID | Tarea | Estado | Comprobación |
| --- | --- | --- | --- |
| CORE-01 | Movimiento y salto de precisión. | Integrado | Pruebas de EditMode y PlayMode; límite de caída exacto. |
| CORE-02 | Pared, salto de pared y escalada con cuerda (100 puntos). | Integrado | Pruebas de EditMode y PlayMode. |
| CORE-03 | Gancho: balanceo, arrastre, cuerda en esquinas y vista previa. | Integrado | Pruebas de PlayMode, con 1350 recorridos a toda velocidad. |
| CORE-04 | Estrella ancla que escribe el jugador. | Integrado | Pruebas de PlayMode. |
| LEVEL-01 | Salas, cámara, muerte, reaparición, checkpoints y compuertas. | Integrado | Pruebas de PlayMode y *Revisar escena*. |
| LEVEL-02 | Plataformas móviles, rejillas, losas y cristales de recarga. | Integrado | Pruebas de PlayMode. |
| HAZ-01 | Peligros pintados con tiles: engranajes, sierras y nebulosa. | Integrado | Pruebas de PlayMode. |
| ART-01 | Almanaque XII con Animator (13 clips). | Integrado | Pruebas de EditMode y PlayMode. |
| ART-02 | Tiles de las Entrañas con Rule Tiles y metal estelar con efecto al engancharlo. | Integrado | Pruebas de PlayMode. |
| ELEV-01 | Elevador de la sala 10 y elevador del Pozo Celeste (la versión con cambio de escena se sustituye por el final de la demo, ver END-01). | Integrado | Pruebas de PlayMode; recorrido visto en Play. |
| UI-01 | Menús, pausa, ajustes y créditos. | Integrado | Pruebas de EditMode y PlayMode. |
| UI-02 | HUD (usos del gancho y de la estrella, nombre de zona) y caja de diálogo. | Integrado | Pruebas de PlayMode; visto en Play. |
| AUDIO-01 | Música por sala y efectos de sonido. | Integrado | Todos los eventos de [[05 - Audio y Música]] suenan; falta confirmar que los volúmenes sobreviven a recargar. |
| QA-01 | Probar a mano el recorrido con teclado, ratón y mando. | Completado | Revisión del equipo del 10 de noviembre; los casos detallados se registran en [[02 - Pruebas]]. |
| DEVOPS-01 | CI: formato, pruebas, análisis estático y compilación hacia `main`. | Integrado | Ejecuciones en verde desde el 30 de octubre. |

## Pendientes identificados

| ID | Tarea | Prioridad propuesta | Responsable según el reparto | Dependencia | Criterio de aceptación |
| --- | --- | --- | --- | --- | --- |
| END-01 | Final de la demo: el elevador del Pozo Celeste sube sin cambiar de escena, con la conversación final, la tarjeta de estadísticas (muertes, tiempo y poemas) y «Gracias por jugar la demo». | Alta | Diego Angel Ramirez Fernandez, con Aleksander Rocha Baeza para el texto | Elevador del Pozo Celeste. | La demo termina en la sala 18, aparece la tarjeta y el botón «Volver al título» (o, a los 30 s, vuelve solo) lleva al menú. |
| COLL-01 | Poema coleccionable: panel de lectura al recogerlo y contador. | Alta | Diego Angel Ramirez Fernandez, con Aleksander Rocha Baeza para el texto | Texto del poema. | El panel se cierra con Aceptar y el poema cuenta en el guardado, en la tarjeta de Continuar y en las estadísticas. |
| SAVE-01 | Guardado automático de 3 registros (aprobado el 10 de noviembre). | Alta | Diego Angel Ramirez Fernandez y Felipe Natanael Chan Uc | Propuesta de [[04 - Guardado y Configuración]]. | *Continuar* se desbloquea, las tarjetas muestran el progreso real, *Volver al menú* guarda y «Borrar registro» funciona con partidas reales. |
| INPUT-01 | Tres modos del gancho en Configuración › Jugabilidad, guardados en los ajustes. | Alta | Diego Angel Ramirez Fernandez | — | Mantener, alternar y alternar con Saltar funcionan con teclado y mando. |
| TEST-01 | Pruebas automáticas del elevador sin cambio de escena y del final de la demo. | Alta | Diego Angel Ramirez Fernandez | END-01. | Las pruebas de PlayMode del nuevo elevador pasan en el CI. |
| TEST-02 | Pruebas automáticas del sistema de guardado. | Alta | Diego Angel Ramirez Fernandez | SAVE-01. | Las pruebas de guardar, continuar y borrar pasan en el CI. |
| QA-02 | Probar con jugadores nuevos y ajustar la dificultad. | Alta | Todo el equipo | QA-01. | Una persona nueva termina las Entrañas del Reloj sin ayuda externa y sabe por qué murió. |
| TECH-01 | Validar la build de Windows en un equipo limpio y fijar la escena inicial. | Alta | Diego Roman Pedraza Keb y Diego Angel Ramirez Fernandez | Build candidata y equipo de prueba. | La build descarga, abre y corre desde el menú; resolución, FPS y memoria registrados con el commit usado. |
| ART-03 | Integrar a Efeméride (sprites de reposo y habla ya dibujados). | Media | Dalia Jimena Chim Uc y Victor Alexis Yah Alpuche | Diálogos finales. | Efeméride aparece en pantalla con sus burbujas de texto. |
| UX-01 | Confirmar los nombres de zona del HUD (provisionales). | Baja | Aleksander Rocha Baeza y Diego Angel Ramirez Fernandez | Revisión del equipo. | Los nombres de cada zona quedan fijados en el HUD de cada escena. |
| UI-03 | Revisar la interfaz a 1280 × 720, 1600 × 900 y 1920 × 1080, y medir con el Profiler. | Media | Victor Alexis Yah Alpuche | Build jugable. | Interfaz legible en las tres resoluciones y sin saltos de rendimiento. |
| TECH-02 | Verificar la build de WebGL, si se decide publicarla. | Baja | Diego Roman Pedraza Keb | TECH-01. | Menús, ajustes, controles y escalas comprobados en navegador. |

Estos puntos salen de la bitácora del juego y de la revisión del equipo; el estado de cada uno se actualiza aquí al cerrarse.

> **Navegación:** [[00 - Índice]] · [[00 - Avance jugable]] · ← [[03 - Roadmap]] · [[05 - Gestión de Cambios]] →
