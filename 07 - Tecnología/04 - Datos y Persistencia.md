# Datos y persistencia

| Entidad         | Contenido                                                                                                                                  | Se guarda                                  |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------ |
| Registro        | Escena y sala, checkpoint tomado, habilidades, poemas, conversaciones vistas, elevadores de solo ida usados, muertes, tiempo, fecha y miniatura | Sí (un archivo JSON por registro, 3 en total) |
| Ajustes         | Valores de audio, idioma y jugabilidad (modo del gancho, ayuda de puntería)                                                                | Sí (almacén de preferencias, aparte)       |
| Salas           | Límites de cámara y puntos de aparición                                                                                                    | No (forman parte de las escenas)           |
| Estado temporal | Usos del gancho y de la estrella ancla, cuerda, plataformas, cristales, losas y compuertas                                                 | No (se reinicia al reaparecer o al cargar) |

Los registros son JSON con su miniatura (PNG de 320 × 180) en la carpeta de datos persistentes del usuario; en la versión web esa carpeta vive en el almacenamiento del navegador, y hay que comprobar en la build si hace falta forzar la escritura. Cada archivo lleva un número de versión: si es de una versión anterior, los campos nuevos se completan con valores predeterminados; si está dañado, se intenta con la copia de respaldo y, si tampoco sirve, el juego avisa y ofrece una partida nueva sin borrar el archivo dañado.

Se guarda al entrar en una sala, al tomar un checkpoint y al recibir una habilidad (ver [[04 - Guardado y Configuración]]).

> **Navegación:** [[00 - Índice]] · ← [[03 - Requisitos Técnicos]] · [[05 - Seguridad y Riesgos Técnicos]] →
