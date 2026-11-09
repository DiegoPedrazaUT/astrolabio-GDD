# Bugs y Seguimiento

## Reporte de bug

**Título:**

**Versión:**

**Nivel / escena:**

**Pasos para reproducir:**

1.
2.
3.

**Resultado esperado:**

**Resultado actual:**

**Frecuencia:** Siempre / A veces / Rara vez

**Severidad:** Crítica / Alta / Media / Baja

**Evidencia:**

**Estado:** Abierto / En progreso / Resuelto / Cerrado

## Registro

| ID | Bug | Severidad | Área | Estado |
| --- | --- | --- | --- | --- |
| BUG-01 | Las habilidades no pasan de una escena a otra. En el Eje Central el jugador las tiene porque el prefab `Player` las trae activadas; en las Entrañas la escena las desactiva | Media | Programación | Abierto: lo corrige el guardado propuesto en [[04 - Guardado y Configuración]] |
| BUG-02 | El CI fallaba siempre con `no space left on device` al bajar la imagen de Unity | Alta | DevOps | Resuelto el 29/10/2026 (paso «Liberar espacio en disco») |
| BUG-03 | El Editor moría a los segundos de abrir el proyecto en el CI (código 137) por una caché de `Library` en mal estado | Alta | DevOps | Mitigado: se versionaron las claves de caché |
| BUG-04 | La caída tenía un límite de 21,4 en lugar de 20 | Baja | Programación | Resuelto el 27/10/2026 |
| BUG-05 | El deslizamiento en pared iba a 4,4 aunque el diseño decía 3 (el límite se aplicaba antes de la gravedad del paso) | Baja | Programación | Resuelto el 29/10/2026: el límite es exacto y se siente igual |
| BUG-06 | Unity se bloquea con el diálogo «Scene(s) Have Been Modified» si se lanzan pruebas tras guardar una escena por script | Baja | Herramientas | Conocido: hay que cerrar el diálogo en el Editor |

## Limitaciones conocidas (no son bugs)

| Tema | Descripción |
| --- | --- |
| Salto desde la plataforma zip | A media carrera el impulso se queda corto (tope de 14 frente a 20 de la plataforma). Se salta al final del recorrido o ya frenada |
| Velocidad en el aire | Solo dura la velocidad que supera la de carrera (7,6); saltar desde una plataforma lenta no lanza |
| Gas y cuerda | Una cuerda que pasa por debajo del gas no se corta: al colocarlo hay que dejar sitio al balanceo |
| Salas junto a un muro | Si el borde de una sala coincide con un muro, no se ve desde dentro: el límite se pone detrás del muro |
| Guardado | No existe en la demo (ver [[00 - Avance jugable]]) |

## Estado de la prueba a mano

No se han probado a mano el teclado, el ratón, el mando ni la versión WebGL. Los fallos que aparezcan en esas pruebas se añaden a este registro.

> **Navegación:** [[00 - Índice]] · ← [[02 - Pruebas]] · [[04 - Criterios de Aceptación]] →
