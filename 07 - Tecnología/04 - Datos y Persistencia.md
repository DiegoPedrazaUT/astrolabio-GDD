# Datos y Persistencia

## Datos persistentes

- **Progreso:** escena, sala y checkpoint, y habilidades (gancho y estrella ancla); en el diseño previsto, también fragmentos de estrella y poemas. **No se guarda en la demo actual.**
- **Configuración:** audio, video, controles y accesibilidad.
- **Inventario:** no aplica (no hay inventario).
- **Estadísticas:** muertes y tiempo de juego, que se muestran en la tarjeta final.
- **Desbloqueos:** habilidades entregadas (gancho y estrella ancla) y poemas encontrados.
- **Otros:** ninguno.

## Modelo de datos

| Entidad         | Contenido                                                 | Se guarda                     |
| --------------- | --------------------------------------------------------- | ----------------------------- |
| Partida | Fragmentos obtenidos, habilidades entregadas, escena y sala, muertes y tiempo de juego | Sí (archivo de partida) |
| Coleccionables | Identificadores de los poemas encontrados | Sí (dentro de la Partida) |
| Salas | Límites de cámara y puntos de aparición de cada sala | No (forma parte de las escenas) |
| Estado temporal | Usos del gancho y de la estrella ancla, cuerda, sala actual y checkpoint activo | No (se reinicia al reaparecer o al cargar) |
| Configuración   | Valores de audio, video, controles y accesibilidad        | Sí (archivo aparte)           |

Relaciones: una Partida referencia los Coleccionables por identificador; la Configuración es independiente de la Partida.

## Formato

**Formato de guardado:** JSON, legible y fácil de depurar.

**Ubicación:** Carpeta de datos persistentes del usuario en Windows (la que Unity ofrece para cada juego). Partida y configuración van en archivos separados.

**Versionado de datos:** Cada archivo lleva un número de versión de datos.

## Migraciones

- Si el archivo es de una versión anterior, los campos nuevos se completan con valores predeterminados y el archivo se actualiza al guardar.
- Si el archivo está dañado o no se puede leer, se intenta con la copia de respaldo; si tampoco sirve, el juego avisa y ofrece empezar una partida nueva sin borrar el archivo dañado.

> **Navegación:** [[00 - Índice]] · ← [[03 - Requisitos Técnicos]] · [[05 - Seguridad y Riesgos Técnicos]] →
