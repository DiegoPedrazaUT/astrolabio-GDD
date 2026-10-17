# Datos y Persistencia

## Descripción de la sección

Define qué información necesita conservar el juego y cómo se estructura.

## Datos persistentes

- **Progreso:** Casas restauradas, fragmentos de estrella obtenidos y último punto guardado.
- **Configuración:** audio, video, controles y accesibilidad.
- **Inventario:** no aplica (no hay inventario).
- **Estadísticas:** muertes y tiempo de juego, que se muestran en la tarjeta final.
- **Desbloqueos:** habilidades entregadas (hilo y estrella) y poemas y notas encontrados.
- **Otros:** ninguno.

## Modelo de datos

Describe las entidades y relaciones.

| Entidad         | Contenido                                                 | Se guarda                     |
| --------------- | --------------------------------------------------------- | ----------------------------- |
| Configuración   | Valores de audio, video, controles y accesibilidad        | Sí (archivo aparte)           |

Relaciones: una Partida referencia Casas y Coleccionables por identificador; la Configuración es independiente de la Partida.

## Formato

**Formato de guardado:** JSON, legible y fácil de depurar.

**Ubicación:** Carpeta de datos persistentes del usuario en Windows (la que Unity ofrece para cada juego). Partida y configuración van en archivos separados.

**Versionado de datos:** Cada archivo lleva un número de versión de datos.

## Migraciones

¿Qué ocurre si cambia la estructura de los datos entre versiones?

- Si el archivo es de una versión anterior, los campos nuevos se completan con valores predeterminados y el archivo se actualiza al guardar.
- Si el archivo está dañado o no se puede leer, se intenta con la copia de respaldo; si tampoco sirve, el juego avisa y ofrece empezar una partida nueva sin borrar el archivo dañado.
- Las partidas de la demo no se garantizan compatibles con la versión completa.


> **Navegación:** [[00 - Índice]] · ← [[03 - Requisitos Técnicos]] · [[05 - Seguridad y Riesgos Técnicos]] →
