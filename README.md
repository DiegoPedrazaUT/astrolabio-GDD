<p align="center">
  <img src="Media/Logo-Astrolabio.png" alt="Astrolabio" width="560">
</p>

# Astrolabio — Documento de Diseño de Videojuego (GDD)

**Astrolabio** es un plataformas 2D de precisión hecho en Unity. Eres el **Almanaque XII**, un pequeño autómata que asciende por el Gran Reloj Cósmico. Escalas, escribes estrellas ancla en el vacío y te lanzas con un gancho de luz para devolver las constelaciones rotas a su órbita.

Es el proyecto integrador del equipo de la Universidad Tecnológica de Cancún. Este repositorio contiene **solo el documento de diseño**; el juego vive en su propio repositorio (ver [[01 - Ficha del Proyecto]]).

## Estado del proyecto (resumen)

| Aspecto | Estado |
| --- | --- |
| **Versión del GDD** | 0.8.0 (ver [[04 - Historial de Versiones]]) |
| **Desarrollo** | En producción |
| **Motor** | Unity 6000.6.4f1, URP 2D, nuevo Input System, C# |
| **Plataforma** | PC (Windows), un jugador |
| **Alcance de la demo** | Entrañas del Reloj (18 salas) → elevador del Pozo Celeste → fin de la demo con tarjeta de estadísticas |
| **Pruebas automáticas** | 86 de EditMode y 212 de PlayMode en verde, análisis estático sin avisos (07/11/2026) |
| **Pruebas a mano** | Aún no hechas con teclado, ratón o mando físicos, ni en WebGL (ver [[02 - Pruebas]]) |

El detalle de lo que ya se puede jugar está en [[00 - Avance jugable]], con sus límites.

## Por dónde empezar

1. [[00 - Índice]]: mapa completo del documento.
2. [[00 - Avance jugable]]: qué funciona hoy y qué no.
3. [[02 - Visión del Juego]] y [[04 - Pilares de Diseño]]: qué experiencia busca el juego.
4. [[06 - Registro visual]]: arte real del juego, con su procedencia.
5. [[01 - Alcance]]: qué entra y qué no en la demo.

## Cómo está organizado

| Sección | Contenido |
| --- | --- |
| 01 — Visión | Ficha, visión, público y pilares |
| 02 — Diseño | Jugabilidad, mecánicas, sistemas, controles, progresión, economía y reglas |
| 03 — Historia y Mundo | Premisa, mundo, personajes y diálogos |
| 04 — Contenido | Estructura, niveles, enemigos y peligros, objetos y misiones |
| 05 — Arte y Audio | Dirección de arte, personajes, entornos, interfaz, audio y registro visual |
| 06 — Experiencia | UX, interfaz, accesibilidad, guardado y configuración |
| 07 — Tecnología | Arquitectura, motor, requisitos, datos y riesgos |
| 08 — Producción | Alcance, roles, roadmap, backlog y gestión de cambios |
| 09 — Calidad | Criterios, pruebas, bugs y aceptación |
| 10 — Referencia | Glosario, referencias, decisiones y versiones |
| 11 — Referencia de Diseño | Biblioteca de clasificación (géneros, plataformas, cámaras…) |

## Equipo

| Integrante | Áreas |
| --- | --- |
| Diego Roman Pedraza Keb | Líder del proyecto, gestión, DevOps, marketing |
| Diego Angel Ramirez Fernandez | Programación, DevOps, game design, diseño de niveles |
| Dalia Jimena Chim Uc | Diseño, concept art, pixel art |
| Felipe Natanael Chan Uc | Audio, programación |
| Victor Alexis Yah Alpuche | Arte, diseño, UI/UX |
| Aleksander Rocha Baeza | Narrativa, ambientación |

## Cómo abrirlo

Abre esta carpeta como bóveda en **Obsidian**: los enlaces `[[ ]]` y la navegación al pie de cada página funcionan ahí. Las imágenes están en `Media/` y se guardan con Git LFS (`*.png`).

## Créditos de la plantilla

La estructura base de este GDD es la guía de **Ing. Luis Fernando Villafaña Rejón** (ver [[00 - Acerca de esta guía]]).
