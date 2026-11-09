# Astrolabio — Documento de Diseño de Videojuego (GDD)

> [!info] Estructura
> Estructura base: guía de **Ing. Luis Fernando Villafaña Rejón** (ver [[00 - Acerca de esta guía]]). Adaptada al proyecto Astrolabio.

> [!abstract] Propósito
> Este documento es la **fuente central de verdad del diseño de Astrolabio**: qué es el juego, qué experiencia busca, cómo funciona, qué contiene, cómo se construye y cómo se comprueba. Documenta también el **estado real** del desarrollo, con sus límites.

## Resumen

**Astrolabio** es un plataformas 2D de precisión (Unity, PC Windows, un jugador). El Almanaque XII, un autómata, asciende por el Gran Reloj Cósmico usando escalada, un hilo de luz y estrellas-anclaje que él mismo escribe en el vacío.

**La demo** dura el tutorial completo y su cierre: las Entrañas del Reloj (18 salas) → el elevador del Pozo Celeste → la llegada al Eje Central → el Almanaque cruza las puertas de Géminis y la demo termina. Los dos niveles del juego completo quedaron fuera del alcance el 08/11/2026 (ver [[03 - Registro de Decisiones]]).

**Estado:** en producción, con luz verde del profesor. Lo jugable hoy y sus límites están en [[00 - Avance jugable]]; los resultados de pruebas, en [[02 - Pruebas]].

## Entrada recomendada

| Si quieres… | Lee |
| --- | --- |
| Entender el juego en cinco minutos | [[02 - Visión del Juego]] → [[04 - Pilares de Diseño]] → [[01 - Jugabilidad]] |
| Saber qué funciona hoy | [[00 - Avance jugable]] |
| Ver el arte real | [[06 - Registro visual]] |
| Saber qué entra en la demo | [[01 - Alcance]] y [[02 - Niveles]] |
| Revisar la calidad | [[01 - Criterios de Calidad]] → [[02 - Pruebas]] |
| Ver por qué se decidió algo | [[03 - Registro de Decisiones]] |

## Navegación

### Portada y avance
- [[00 - Acerca de esta guía]]
- [[00 - Avance jugable]]

### 01 — Visión
- [[01 - Ficha del Proyecto]]
- [[02 - Visión del Juego]]
- [[03 - Público y Plataforma]]
- [[04 - Pilares de Diseño]]

### 02 — Diseño
- [[01 - Jugabilidad]]
- [[02 - Mecánicas]]
- [[03 - Sistemas]]
- [[04 - Controles]]
- [[05 - Progresión]]
- [[06 - Economía y Recursos]]
- [[07 - Reglas y Estados del Juego]]

### 03 — Historia y Mundo
- [[01 - Premisa y Trama]]
- [[02 - Mundo]]
- [[03 - Personajes]]
- [[04 - Diálogos y Narrativa]]

### 04 — Contenido
- [[01 - Estructura del Contenido]]
- [[02 - Niveles]]
- [[03 - Enemigos y NPC]]
- [[04 - Objetos y Coleccionables]]
- [[05 - Misiones y Desafíos]]

### 05 — Arte y Audio
- [[01 - Dirección de Arte]]
- [[02 - Personajes y Animación]]
- [[03 - Entornos]]
- [[04 - Interfaz Visual]]
- [[05 - Audio y Música]]
- [[06 - Registro visual]]

### 06 — Experiencia
- [[01 - UX y Flujo del Jugador]]
- [[02 - UI y Menús]]
- [[03 - Accesibilidad]]
- [[04 - Guardado y Configuración]]

### 07 — Tecnología
- [[01 - Arquitectura Técnica]]
- [[02 - Motor y Herramientas]]
- [[03 - Requisitos Técnicos]]
- [[04 - Datos y Persistencia]]
- [[05 - Seguridad y Riesgos Técnicos]]

### 08 — Producción
- [[01 - Alcance]]
- [[02 - Roles y Responsabilidades]]
- [[03 - Roadmap]]
- [[04 - Backlog del Proyecto]]
- [[05 - Gestión de Cambios]]

### 09 — Calidad
- [[01 - Criterios de Calidad]]
- [[02 - Pruebas]]
- [[03 - Bugs y Seguimiento]]
- [[04 - Criterios de Aceptación]]

### 10 — Referencia
- [[01 - Glosario]]
- [[02 - Referencias e Inspiración]]
- [[03 - Registro de Decisiones]]
- [[04 - Historial de Versiones]]

### 11 — Biblioteca de Clasificación
- [[00 - Biblioteca de Clasificación]]
- [[01 - Géneros]]
- [[02 - Subgéneros y Combinaciones]]
- [[03 - Plataformas y Consolas]]
- [[04 - Perspectivas y Cámaras]]
- [[05 - Modos de Juego]]
- [[06 - Clasificaciones y Etiquetas]]

> [!tip] Principio de diseño
> El GDD evoluciona con el proyecto y registra las decisiones que importan. Cuando el juego y el documento discrepan, el desfase se anota en [[00 - Avance jugable]] o en [[03 - Bugs y Seguimiento]], no se oculta.


> **Navegación:** [[README]] · [[00 - Acerca de esta guía]] · [[00 - Avance jugable]] →
