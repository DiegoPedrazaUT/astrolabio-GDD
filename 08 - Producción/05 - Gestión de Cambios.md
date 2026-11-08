# Gestión de Cambios

## Descripción de la sección

El diseño de un videojuego cambia. Esta sección evita que las modificaciones importantes se pierdan o aparezcan sin evaluar sus consecuencias.

## Proceso

1. Cualquier integrante propone el cambio con la plantilla de solicitud.
2. Se evalúa contra los pilares de diseño (ver [[04 - Pilares de Diseño]]) y contra el alcance (ver [[01 - Alcance]]).
3. El equipo decide, con el líder del proyecto como responsable de la decisión final.
4. Se anota en el registro de esta página y, si es una decisión importante, también en el [[03 - Registro de Decisiones]].
5. Se actualizan las secciones del GDD afectadas y se registra la nueva versión en el [[04 - Historial de Versiones]].

## Solicitud de cambio

**Fecha:**

**Cambio propuesto:**

**Motivo:**

**Beneficio esperado:**

**Costo estimado:**

**Impacto en otros sistemas:**

**Decisión:**

**Responsable:**

## Registro

| Fecha      | Cambio                                                              | Motivo                                                                                          | Impacto                                                                                                                       | Estado   |
| ---------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | -------- |
| 16/10/2026 | Descartar los *Rule Tiles* y pintar los tiles a mano con *Tile Palette* (sustituido el 03/11/2026) | Es un flujo más complejo de lo que necesita un proyecto escolar de este alcance                 | Cambia [[03 - Entornos]] y [[02 - Motor y Herramientas]]: cada esquina, borde e interior es un tile independiente                | Reemplazado |
| 16/10/2026 | Eliminar los observatorios menores y conservar solo los mayores     | No aportan al juego ni a la historia                                                            | Cambian el descanso y el guardado: el progreso se guarda en los observatorios mayores y al cambiar de Casa; los poemas se releen en los mayores | Aprobado |
| 16/10/2026 | Adoptar la paleta SLSO8 como paleta base                            | Una paleta fija de 8 colores unifica el arte y facilita el trabajo del equipo                   | Afecta a toda la dirección de arte (ver [[01 - Dirección de Arte]]); puede ampliarse con excepciones documentadas              | Aprobado |
| 02/11/2026 | Eliminar la Casa de Acuario y dejar a Géminis como única Casa jugable | Por el tiempo disponible para la entrega de la demo | La demo queda con tres niveles: Las Entrañas, Géminis y el final (Observatorio de Ofiuco y Cámara Central); cambian el número de poemas y notas y el calendario | Aprobado |
| 03/11/2026 | Adoptar los *Rule Tiles* y pasar los tiles de 16×16 a 32×32 px | Los *Rule Tiles* ahorran trabajo al pintar los niveles y mantienen continuas las esquinas y los bordes; con 32 px cada tile admite más detalle | Sustituye el cambio del 16/10/2026. Cambian [[01 - Dirección de Arte]], [[03 - Entornos]], [[02 - Motor y Herramientas]] y [[03 - Requisitos Técnicos]]: la vista base pasa de 640×360 a 1280×720 px (40 × 22,5 tiles) | Aprobado |


> **Navegación:** [[00 - Índice]] · ← [[04 - Backlog del Proyecto]] · [[01 - Criterios de Calidad]] →
