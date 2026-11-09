# Entregas y trabajo pendiente

| Área | Estado al 8 de noviembre |
| --- | --- |
| Jugador | Movimiento, salto, pared, escalada con cuerda, gancho y estrella ancla integrados, con pruebas automáticas. |
| Nivel | Salas con cámara, checkpoints, compuertas, plataformas (patrulla, zip, rejillas, losas) y cristales. |
| Peligros | Engranajes, sierras y gas nebuloso (mata y corta el gancho). |
| Arte | Almanaque con 13 animaciones, tiles del tutorial con Rule Tiles de 32 × 32, fondo y decorado de las Entrañas. |
| Elevadores | De solo ida en la sala 10 y del Pozo Celeste, con cambio a la escena del Eje Central. |
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
| HAZ-01 | Peligros pintados con tiles: engranajes, sierras y gas. | Integrado | Pruebas de PlayMode. |
| ART-01 | Almanaque XII con Animator (13 clips). | Integrado | Pruebas de EditMode y PlayMode. |
| ART-02 | Tiles del tutorial con Rule Tiles y metal estelar con efecto al engancharlo. | Integrado | Pruebas de PlayMode. |
| ELEV-01 | Elevador de la sala 10 y elevador del Pozo Celeste con cambio de escena. | Integrado | Pruebas de PlayMode; recorrido visto en Play. |
| UI-01 | Menús, pausa, ajustes y créditos. | Integrado | Pruebas de EditMode y PlayMode. |
| UI-02 | HUD (usos del gancho y de la estrella, nombre de zona) y caja de diálogo. | Integrado | Pruebas de PlayMode; visto en Play en el Eje Central. |
| DEVOPS-01 | CI: formato, pruebas, análisis estático y compilación hacia `main`. | Integrado | Ejecuciones en verde desde el 30 de octubre. |

## Pendientes identificados

| ID | Tarea | Prioridad propuesta | Responsable según el reparto | Dependencia | Criterio de aceptación |
| --- | --- | --- | --- | --- | --- |
| QA-01 | Probar a mano el recorrido completo con teclado, ratón y mando. | Alta | Todo el equipo, coordinado por Diego Angel Ramirez Fernandez | Build jugable. | Los casos CP-01 a CP-05 de [[02 - Pruebas]] quedan ejecutados y los fallos registrados en [[03 - Bugs y Seguimiento]]. |
| QA-02 | Probar con jugadores nuevos y ajustar la dificultad. | Alta | Todo el equipo | QA-01. | Una persona nueva termina el tutorial sin ayuda externa y sabe por qué murió. |
| TECH-01 | Validar la build de Windows en un equipo limpio y fijar la escena inicial. | Alta | Diego Roman Pedraza Keb y Diego Angel Ramirez Fernandez | Build candidata y equipo de prueba. | La build descarga, abre y corre desde el menú; resolución, FPS y memoria registrados con el commit usado. |
| END-01 | Implementar el cierre: el Almanaque cruza las puertas de Géminis y aparece la tarjeta final. | Alta | Diego Angel Ramirez Fernandez, con Aleksander Rocha Baeza para el texto | Escena del Eje Central. | Al cruzar las puertas termina la demo con la tarjeta final y el jugador puede volver al menú. |
| AUDIO-01 | Integrar música y efectos de sonido. | Alta | Felipe Natanael Chan Uc | Escenas finales; audio configurable en el juego. | Todos los eventos de [[05 - Audio y Música]] suenan y los volúmenes sobreviven a recargar. |
| SAVE-01 | Decidir e implementar el guardado (propuesta de 3 registros con autoguardado). | Media, según decisión | Equipo; programación de Felipe Natanael Chan Uc | Decisión del equipo. | *Continuar* se desbloquea, las habilidades se conservan entre escenas y *Volver al menú* guarda. |
| BUG-01 | Conservar las habilidades al cambiar de escena. | Media | Diego Angel Ramirez Fernandez | SAVE-01 o ajuste propio. | En el Eje Central el jugador tiene las habilidades que ganó, no las del prefab (ver [[03 - Bugs y Seguimiento]]). |
| ART-03 | Integrar a Efeméride (sprites de reposo y habla ya dibujados). | Media | Dalia Jimena Chim Uc y Victor Alexis Yah Alpuche | Diálogos finales. | Efeméride aparece en pantalla con sus burbujas de texto. |
| UX-01 | Confirmar los nombres de zona del HUD (provisionales). | Baja | Aleksander Rocha Baeza y Diego Angel Ramirez Fernandez | Revisión del equipo. | Los nombres de cada zona quedan fijados en el HUD de cada escena. |
| UI-03 | Revisar la interfaz a 1280 × 720, 1600 × 900 y 1920 × 1080, y medir con el Profiler. | Media | Victor Alexis Yah Alpuche | Build jugable. | Interfaz legible en las tres resoluciones y sin saltos de rendimiento. |
| INPUT-01 | Evaluar una opción para elegir cómo se controla el gancho. | Baja | Diego Angel Ramirez Fernandez | Resultados de QA-02. | Decisión registrada en [[03 - Registro de Decisiones]]. |
| TECH-02 | Verificar la build de WebGL, si se decide publicarla. | Baja | Diego Roman Pedraza Keb | TECH-01. | Menús, ajustes, controles y escalas comprobados en navegador. |

Estos puntos son necesidades identificadas en la bitácora del juego; el estado de cada uno se actualiza aquí al cerrarse.

> **Navegación:** [[00 - Índice]] · [[00 - Avance jugable]] · ← [[03 - Roadmap]] · [[05 - Gestión de Cambios]] →
