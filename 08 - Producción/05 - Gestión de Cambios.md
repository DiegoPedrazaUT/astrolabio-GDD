# Gestión de Cambios

## Descripción de la sección

El diseño de un videojuego evoluciona durante la revisión del equipo y la retroalimentación del profesor. Esta sección establece el protocolo para evaluar y registrar las modificaciones sin romper la coherencia entre apartados.

## Flujo para aprobar un cambio

1. **Propuesta:** cualquier integrante describe la necesidad (alcance, mecánica, arte, interfaz o narrativa), el motivo y los archivos afectados.
2. **Validación técnica y de reglas:** Diego Angel Ramirez Fernandez verifica el impacto en mecánicas, niveles, rendimiento o pruebas.
3. **Decisión y cierre:** Diego Roman Pedraza Keb (líder) confirma que el cambio respeta el alcance y los pilares ([[04 - Pilares de Diseño]]), coordina la actualización de todos los documentos relacionados y lo anota en [[03 - Registro de Decisiones]] y en [[04 - Historial de Versiones]].

## Registro de cambios

| Fecha | Cambio | Motivo | Impacto en otros sistemas | Responsable | Estado |
|---|---|---|---|---|---|
| 16/10/2026 | Descartar los *Rule Tiles* y pintar los tiles a mano con *Tile Palette*. | Flujo más complejo de lo que necesitaba el proyecto. | [[03 - Entornos]] y [[02 - Motor y Herramientas]]. | Diego Roman Pedraza Keb / Dalia Jimena Chim Uc | Reemplazado el 03/11/2026 |
| 16/10/2026 | Eliminar los observatorios menores. | No aportan al juego ni a la historia. | Descanso y guardado. | Diego Roman Pedraza Keb | Histórico |
| 16/10/2026 | Adoptar la paleta SLSO8 como paleta base. | Una paleta fija de 8 colores unifica el arte. | [[01 - Dirección de Arte]]. | Diego Roman Pedraza Keb / Dalia Jimena Chim Uc | Vigente |
| 02/11/2026 | Recortar la Casa de Acuario (descartada en desarrollo el 29/10/2026). | Tiempo y complicaciones de producción. | Alcance y [[02 - Niveles]]. | Diego Roman Pedraza Keb | Vigente |
| 02/11/2026 | Eliminar los observatorios mayores. | Tiempo de producción. | El guardado ya no depende de ellos; el Observatorio de Ofiuco queda fuera de la demo. | Diego Roman Pedraza Keb | Vigente |
| 02/11/2026 | Eliminar las notas del Almanaque XI. | Tiempo de producción. | XI solo se conoce por su cuerpo y su carta de despedida. | Aleksander Rocha Baeza | Vigente |
| 02/11/2026 | Eliminar los hologramas de la Tierra y el del tutorial. | Tiempo de producción. | Efeméride se queda como holograma. | Aleksander Rocha Baeza | Vigente |
| 03/11/2026 | Usar *Rule Tiles* y tiles de 32 × 32 en lugar de 16 × 16. | Tiles que se conectan solos y sin costuras. | [[01 - Dirección de Arte]], [[03 - Entornos]], [[02 - Motor y Herramientas]]. | Diego Angel Ramirez Fernandez / Dalia Jimena Chim Uc | Vigente |
| 03/11/2026 | Fijar la resolución de referencia en 1280 × 720. | Una sola referencia para cámara e interfaz. | [[03 - Requisitos Técnicos]], [[04 - Interfaz Visual]]. | Diego Angel Ramirez Fernandez / Victor Alexis Yah Alpuche | Vigente |
| 08/11/2026 | Quitar los dos niveles del juego: la demo termina en el Eje Central, cuando el Almanaque cruza las puertas de Géminis. | El profesor dio luz verde y le gustó el tutorial. | [[01 - Alcance]], [[02 - Niveles]], [[05 - Progresión]], [[05 - Misiones y Desafíos]] y la narrativa. | Diego Roman Pedraza Keb | Vigente |
| 08/11/2026 | Adaptar la estructura del GDD al formato del profesor: portada, avance jugable, calidad, referencia y registro visual. | El profesor pidió un GDD organizado como el modelo del curso. | Todas las secciones; nuevas 09 y 10. | Diego Roman Pedraza Keb | Vigente |

Los valores de filas históricas se conservan como antecedentes y no describen la demo vigente. La columna Responsable es una propuesta basada en las áreas de cada integrante, igual que el reparto de [[02 - Roles y Responsabilidades]].

## Revisión 0.6.0 del 8 de noviembre

La edición 0.6.0 recoge el nuevo alcance y el estado real del desarrollo: tutorial de 18 salas, elevador del Pozo Celeste, llegada al Eje Central, interfaz, HUD y pruebas. Géminis y el Observatorio de Ofiuco pasan a ser trasfondo de la historia. El guardado se registra como pendiente de decisión, no como función de la demo.


> **Navegación:** [[00 - Índice]] · [[00 - Avance jugable]] · ← [[04 - Backlog del Proyecto]] · [[01 - Criterios de Calidad]] →
