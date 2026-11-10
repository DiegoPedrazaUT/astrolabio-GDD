# Gestión de Cambios

El diseño evoluciona con la revisión del equipo y la retroalimentación del profesor. Esta página fija cómo se evalúan y registran los cambios sin romper la coherencia entre apartados.

## Flujo para aprobar un cambio

1. **Propuesta:** cualquier integrante describe la necesidad (alcance, mecánica, arte, interfaz o narrativa), el motivo y los archivos afectados.
2. **Validación técnica y de reglas:** Diego Angel Ramirez Fernandez verifica el impacto en mecánicas, niveles, rendimiento o pruebas.
3. **Decisión y cierre:** Diego Roman Pedraza Keb (líder) confirma que el cambio respeta el alcance y los pilares ([[04 - Pilares de Diseño]]), coordina la actualización de todos los documentos relacionados y lo anota en [[03 - Registro de Decisiones]] y en [[04 - Historial de Versiones]].

## Registro de cambios

Solo recoge los cambios del proyecto actual (repositorio de producción desde el 27 de octubre).

| Fecha | Cambio | Motivo | Impacto en otros sistemas | Responsable | Estado |
|---|---|---|---|---|---|
| 30/10/2026 | La nebulosa (antes «gas») es un tile de 32 × 32, estático, que mata y corta el gancho. | Alcance y facilidad de configurar. | [[02 - Mecánicas]], [[03 - Enemigos y NPC]]. | Diego Angel Ramirez Fernandez | Vigente |
| 30/10/2026 | La lente y el raíl de luz no van en los niveles; las plataformas no se enganchan. | Alcance. | [[02 - Mecánicas]], [[03 - Sistemas]]. | Diego Angel Ramirez Fernandez | Vigente |
| 30/10/2026 | El gancho se dispara aunque no haya objetivo, con vista previa solo si hay algo enganchable. | Que el jugador vea el alcance sin gastar usos. | [[02 - Mecánicas]]. | Diego Angel Ramirez Fernandez | Vigente; por validar con jugadores |
| 02/11/2026 | Eliminar las notas del Almanaque XI y los hologramas de la Tierra. | Tiempo de producción. | XI solo se conoce por su cuerpo; Efeméride se queda como holograma. | Aleksander Rocha Baeza | Vigente |
| 03/11/2026 | Usar *Rule Tiles* y tiles de 32 × 32. | Tiles que se conectan solos y sin costuras. | [[01 - Dirección de Arte]], [[03 - Entornos]], [[02 - Motor y Herramientas]]. | Diego Angel Ramirez Fernandez / Dalia Jimena Chim Uc | Vigente |
| 03/11/2026 | Fijar la resolución de referencia en 1280 × 720. | Una sola referencia para cámara e interfaz. | [[03 - Requisitos Técnicos]], [[04 - Interfaz Visual]]. | Diego Angel Ramirez Fernandez / Victor Alexis Yah Alpuche | Vigente |
| 08/11/2026 | Renombrar el hilo de luz como gancho de luz y el punto de apoyo como estrella ancla; simplificar las páginas y quitar secciones repetidas. | Nombres más claros y un documento más corto. | Todos los apartados. | Diego Roman Pedraza Keb | Vigente |
| 10/11/2026 | La entrega pasa al 13 de noviembre. El elevador del Pozo Celeste ya no cambia de escena: la demo termina ahí con una tarjeta de estadísticas. Se descartan el Eje Central, las puertas de Géminis y la carta de despedida del Almanaque XI. | Plazo de entrega y alcance. | [[01 - Alcance]], [[02 - Niveles]], [[05 - Progresión]], [[07 - Reglas y Estados del Juego]], [[04 - Diálogos y Narrativa]]. | Diego Roman Pedraza Keb | Vigente |
| 10/11/2026 | «Tutorial» pasa a llamarse «Entrañas del Reloj». | Ahora es un nivel para principiantes, no un tutorial aparte (propuesta de Diego Angel Ramirez Fernandez). | Todos los apartados. | Diego Roman Pedraza Keb | Vigente |
| 10/11/2026 | Se aprueba el guardado automático de 3 registros. | La demo necesita *Continuar* y un progreso real. | [[04 - Guardado y Configuración]], [[04 - Datos y Persistencia]], [[03 - Sistemas]]. | Diego Roman Pedraza Keb | Vigente; en implementación |
| 10/11/2026 | Se quitan la acción de interactuar y la reasignación de controles; la pausa usa Esc, P o Start. | No hay nada que interactuar y los controles no se reasignan. | [[04 - Controles]], [[03 - Accesibilidad]]. | Diego Angel Ramirez Fernandez | Vigente |
| 10/11/2026 | Tres modos para controlar el gancho en Configuración › Jugabilidad. | Que cada jugador elija cómo soltar el gancho. | [[04 - Guardado y Configuración]], [[03 - Accesibilidad]]. | Diego Angel Ramirez Fernandez | Vigente; en implementación |

La columna Responsable es una propuesta basada en las áreas de cada integrante, igual que el reparto de [[02 - Roles y Responsabilidades]].

> **Navegación:** [[00 - Índice]] · [[00 - Avance jugable]] · ← [[04 - Backlog del Proyecto]] · [[01 - Criterios de Calidad]] →
