# Avance jugable

## Recorrido de la demo

| Tramo | Contenido | Estado |
| --- | --- | --- |
| Menú principal | Menús, ajustes y créditos con interfaz propia | Implementado (el guardado no existe: *Continuar* aparece bloqueado) |
| Entrañas del Reloj | Tutorial de 18 salas: movimiento, salto, pared, escalada, gancho y estrella ancla | Escena armada con arte, fondo, decorado y HUD |
| Elevador del Pozo Celeste | Elevador al aire libre: sube 72 unidades en 12 s hacia un cielo con el Gran Reloj y Géminis III iluminados y carga la escena siguiente | Implementado |
| Eje Central | Sala de llegada donde el elevador deja al Almanaque | Escena y HUD creados |
| Cierre | El Almanaque cruza las puertas de Géminis y termina la demo | Decidido el 08/11/2026 (ver [[03 - Registro de Decisiones]]) |

El HUD muestra el nombre de la zona. Los nombres actuales son **provisionales**: Los Nichos (sala 1), La Galería (2–10), El Puente Roto (11–13), El Pozo de Cadenas (14–17) y El Pozo Celeste (18).

## Qué ya funciona

| Sistema | Qué hace | Respaldo |
| --- | --- | --- |
| Movimiento y salto | Correr, saltar, caída con límite exacto | Pruebas de EditMode y PlayMode |
| Pared y escalada | Deslizar, saltar de la pared y escalar superficies rugosas con una cuerda de resistencia (100 puntos; se rellena al pisar suelo) | Pruebas de EditMode y PlayMode |
| Gancho de luz | Se dispara aunque no haya objetivo; balanceo, arrastre, cuerda que dobla esquinas; 2 usos; vista previa punteada solo si hay algo enganchable | Pruebas de PlayMode, incluidos 1350 recorridos a toda velocidad que comprueban que la cuerda no atraviesa sólidos |
| Estrella ancla | El jugador la escribe con la tecla E en el vacío; es una estrella ancla para el gancho | Pruebas de PlayMode |
| Muerte y reaparición | Muerte por peligros o aplastamiento; reaparece en el último checkpoint de la sala | Pruebas de PlayMode |
| Salas, checkpoints y compuertas | Cámara y reaparición por sala; compuertas que se abren al acercarse | Pruebas de PlayMode |
| Peligros | Engranajes y sierras (letales, pintados con tiles) y **gas nebuloso** (mata y corta el gancho) | Pruebas de PlayMode |
| Plataformas | Patrulla, zip, rejillas de un solo sentido y losas que se caen | Pruebas de PlayMode |
| Metal estelar | Superficie enganchable que responde al gancho con una onda de luz | Pruebas de PlayMode |
| Elevadores | De solo ida (sala 10) y de cielo abierto (Pozo Celeste), con cambio de escena | Pruebas de PlayMode |
| Interfaz (UI Toolkit) | Menús, pausa, ajustes, créditos, HUD (usos del gancho y de la estrella, nombre de zona) y caja de diálogo con texto letra a letra | Pruebas de EditMode y PlayMode |
| Personaje | 13 animaciones con Animator a partir de siete hojas de 32×32 | Pruebas de EditMode y PlayMode |

## Qué falta o es provisional

| Tema | Situación |
| --- | --- |
| Guardado | **No existe en la demo.** *Continuar* está bloqueado («Sin registros») y *Volver al menú* avisa «La demo no guarda el progreso». Hay una propuesta lista (3 registros, autoguardado) que espera la decisión del equipo; ver [[04 - Guardado y Configuración]] |
| Habilidades entre escenas | No pasan de una escena a otra: en el Eje Central el jugador las tiene porque el prefab las trae activadas (ver [[03 - Bugs y Seguimiento]]) |
| Nombres de zona del HUD | Provisionales hasta que el equipo los confirme |
| Efeméride | Sprites de reposo y habla dibujados; sin integrar en el juego (ver [[02 - Personajes y Animación]]) |
| Audio | La integración de música y efectos no consta en la bitácora del juego; el área de audio la confirma ([[05 - Audio y Música]]) |

## Verificación

| Comprobación | Resultado (07/11/2026) |
| --- | --- |
| Pruebas EditMode | 86 en verde |
| Pruebas PlayMode | 212 en verde |
| Análisis estático (Roslyn) | 0 avisos |
| Formato (`dotnet format whitespace`) | Limpio |
| Prueba a mano con teclado, ratón y mando físicos | **No realizada** |
| Compilación y prueba en WebGL | **No realizada** (el CI compila Windows y WebGL solo hacia `main`) |

Las pruebas automáticas demuestran que cada pieza cumple sus reglas; no demuestran que el juego **se sienta bien**. Eso solo lo dice una persona jugando. Plan y casos en [[02 - Pruebas]].

## Imágenes

El arte real y su procedencia están en [[06 - Registro visual]].

> **Navegación:** [[00 - Índice]] · ← [[00 - Índice]] · [[01 - Ficha del Proyecto]] →
