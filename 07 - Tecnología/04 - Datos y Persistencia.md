# Datos y persistencia

| Entidad         | Contenido                                                                        | Se guarda                                  |
| --------------- | -------------------------------------------------------------------------------- | ------------------------------------------ |
| Partida         | Fragmentos obtenidos, habilidades entregadas, poemas, escena y sala, muertes y tiempo | Sí (archivo de partida)               |
| Configuración   | Valores de audio, video, controles y accesibilidad                               | Sí (archivo aparte)                        |
| Salas           | Límites de cámara y puntos de aparición                                          | No (forman parte de las escenas)           |
| Estado temporal | Usos del gancho y de la estrella ancla, cuerda, sala actual y checkpoint activo  | No (se reinicia al reaparecer o al cargar) |

El formato es JSON, en la carpeta de datos persistentes del usuario en Windows, con partida y configuración en archivos separados y un número de versión en cada uno. Si el archivo es de una versión anterior, los campos nuevos se completan con valores predeterminados; si está dañado, se intenta con la copia de respaldo y, si tampoco sirve, el juego avisa y ofrece una partida nueva sin borrar el archivo dañado.

> **Navegación:** [[00 - Índice]] · ← [[03 - Requisitos Técnicos]] · [[05 - Seguridad y Riesgos Técnicos]] →
