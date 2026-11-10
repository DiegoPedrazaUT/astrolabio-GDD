# Motor y herramientas

| Tecnología / herramienta | Uso en el proyecto                                                                                                  |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| Unity 6000.6.4f1         | Motor elegido por su soporte 2D, su editor visual de niveles y porque el equipo lo conoce                           |
| URP (renderizador 2D)    | Luces 2D, bloom, viñeta y ajuste de color                                                                           |
| Physics 2D (Box2D)       | Física con paso fijo de 0,02 s                                                                                      |
| Input System             | Un archivo de acciones para teclado, ratón y mando                                                                  |
| Cinemachine 6.6.0        | Una cámara por sala, transiciones y confinamiento                                                                   |
| 2D Tilemap Editor y Extras | *Tilemap*, *Tile Palette* y *Rule Tiles*                                                                          |
| UI Toolkit               | Menús, HUD y caja de diálogo; panel de 1280×720 y fuentes SDF                                                       |
| Unity Test Framework     | Pruebas automáticas de las mecánicas (EditMode y PlayMode)                                                          |
| C#                       | Todo el código del juego (clases, variables y métodos en inglés; comentarios y documentación en español)            |
| Aseprite                 | Pixel art y animación de sprites                                                                                    |
| Reaper y Ableton Live    | Composición y edición de música y efectos (la elige audio)                                                          |
| Obsidian                 | Documento de diseño (GDD)                                                                                           |
| Git, Git LFS y GitHub    | Control de versiones; los recursos pesados van por LFS                                                              |
| GitHub Actions           | CI (`ci.yml`): formato, pruebas, análisis estático (Roslyn) y compilación de Windows y WebGL hacia `main`           |

Los tiles de 32×32 px se pintan con *Rule Tiles*, que eligen solos la esquina, el borde o el interior y mantienen continuas las costuras; esta decisión sustituye a la del 16/10/2026, que los descartaba (ver [[05 - Gestión de Cambios]]). No hay servicios externos ni conexión a internet.

**Convenciones:** carpetas por tipo de recurso; clases y métodos en PascalCase; campos del Inspector privados con `[SerializeField]` y un valor por defecto razonable; arte en PNG sin compresión y con filtro de píxel; música y efectos en WAV de trabajo y OGG dentro del juego. Se usa Gitflow (`feature/*` → `develop` → `main`) y cada archivo se sube con su `.meta`, sin editar a mano los `.unity`, `.prefab` ni `.meta`. Un script por responsabilidad, física en el paso fijo, pruebas automáticas con cada mecánica nueva y prefabs reutilizados.

> **Navegación:** [[00 - Índice]] · ← [[01 - Arquitectura Técnica]] · [[03 - Requisitos Técnicos]] →
