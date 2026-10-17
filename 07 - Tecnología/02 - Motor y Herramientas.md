# Motor y Herramientas

## Descripción de la sección

Documenta las herramientas utilizadas para crear el videojuego y por qué fueron seleccionadas.

## Motor

**Motor:** Unity. Se eligió por su soporte para 2D, su editor visual de niveles y porque el equipo lo conoce.

**Versión:** Unity 6 (serie 6000.6.4f1).

**Renderizado:** Universal Render Pipeline (URP) con el renderizador 2D: luces 2D, bloom, viñeta y ajuste de color.

**Física:** Physics 2D (Box2D) con paso fijo de 0.02 s.

**Sistema de entrada:** Input System (nuevo), con un archivo de acciones para teclado, ratón y mando.

## Lenguajes

| Lenguaje | Uso                                                                                          |
| -------- | -------------------------------------------------------------------------------------------- |
| C#       | Todo el código del juego (nombres de clases, variables y métodos en inglés; comentarios y documentación en español) |

## Herramientas

| Herramienta            | Propósito                                                  | Versión                    |
| ---------------------- | ---------------------------------------------------------- | -------------------------- |
| Unity                  | Motor, editor de niveles y construcción del juego          | Unity 6 (serie 6000.6.4f1) |
| Aseprite               | Pixel art y animación de sprites                           | Última estable             |
| Git y Git LFS (GitHub) | Control de versiones; los recursos pesados van por LFS     | Última estable             |
| Obsidian               | Documento de diseño (GDD)                                  | Última estable             |
| Reaper y Ableton Live  | Composición y edición de música y efectos (la elige audio) | Última estable             |
| Unity Test Framework   | Pruebas automáticas de las mecánicas                       | Incluida en Unity          |

## Dependencias

Paquetes de Unity:

- Universal RP (renderizado 2D y post-proceso)
- Input System
- Cinemachine (una cámara por sala, transiciones y confinamiento)
- 2D Tilemap Editor (*Tilemap* y *Tile Palette*)

**Decisión del equipo:** no se usan *Rule Tiles* ni el paquete 2D Tilemap Extras. Los tiles se pintan a mano con *Tile Palette*, porque es un flujo más simple y suficiente para el alcance del proyecto (ver [[05 - Gestión de Cambios]]).

No hay servicios externos ni conexión a internet.

## Convenciones del proyecto

- **Estructura de carpetas:** por tipo de recurso (escenas, scripts, prefabs, arte, audio, interfaz y recursos cargados por nombre).
- **Nomenclatura:** clases y métodos en inglés con PascalCase; campos del Inspector privados con `[SerializeField]` y un valor por defecto razonable; archivos de arte en minúsculas con guiones bajos.
- **Control de versiones:** Gitflow (ramas `feature/*` → `develop` → `main`). Los archivos de escena, prefab, textura y audio van por Git LFS. Cada archivo se sube con su `.meta`; no se editan a mano los archivos `.unity`, `.prefab` ni `.meta`.
- **Formato de assets:** PNG sin compresión y con filtro de píxel para el arte; música y efectos en WAV de trabajo y OGG dentro del juego.
- **Convenciones de código:**
  - Un script por responsabilidad; solo el controlador del jugador tiene la física por paso fijo.
  - Física en el paso fijo y entrada mediante los eventos del Input System.
  - Cada mecánica nueva llega con sus pruebas automáticas.
  - Los prefabs se reutilizan; cambiar un prefab cambia todas sus copias.


> **Navegación:** [[00 - Índice]] · ← [[01 - Arquitectura Técnica]] · [[03 - Requisitos Técnicos]] →
