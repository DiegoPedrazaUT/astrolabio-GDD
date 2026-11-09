# Criterios de Calidad

En un plataformas de precisión, la calidad se juega en tres cosas: que los controles respondan, que cada muerte se sienta justa y que el jugador entienda qué puede agarrar y qué lo mata. La columna **Estado** dice si cada criterio ya se comprobó y cómo: una prueba automática verifica la regla, y solo una persona jugando verifica la sensación.

## Calidad funcional

| Criterio | Cómo se comprueba | Estado |
| --- | --- | --- |
| Cada mecánica cumple las reglas de [[02 - Mecánicas]] | Pruebas automáticas de cada mecánica (ver [[02 - Pruebas]]) | Cumplido (07/11/2026) |
| La cuerda del gancho no atraviesa ningún sólido, tampoco a toda velocidad | 1350 recorridos automáticos a toda velocidad | Cumplido (07/11/2026) |
| Muerte y reaparición llevan siempre a un punto válido | Revisor de escena y pruebas de reaparición | Cumplido (07/11/2026) |
| Las habilidades se conservan entre escenas | Prueba manual del cambio de escena | No cumplido: ver [[03 - Bugs y Seguimiento]] |
| El progreso se guarda | Prueba de guardado | No aplica a la demo: el guardado no existe |

## Calidad de experiencia

| Criterio | Cómo se comprueba | Estado |
| --- | --- | --- |
| El jugador entiende el objetivo de cada sala sin texto largo | Prueba con jugadores nuevos | Sin verificar |
| Cada muerte se entiende: el jugador sabe qué lo mató | Prueba con jugadores nuevos | Sin verificar |
| La dificultad crece sin saltos (ver [[05 - Progresión]]) | Prueba con jugadores nuevos | Sin verificar |
| Lo que se puede agarrar se distingue de lo que no | Revisión visual con [[06 - Registro visual]] y prueba con jugadores | Sin verificar |
| Los controles responden igual con teclado y con mando | Prueba a mano con ambos | Sin verificar |
| La interfaz se lee a 1280×720, 1600×900 y 1920×1080 | Revisión en cada resolución | Sin verificar |

## Calidad técnica

| Criterio | Cómo se comprueba | Estado |
| --- | --- | --- |
| Pruebas EditMode y PlayMode en verde | CI en cada PR | Cumplido: 86 y 212 (07/11/2026) |
| Análisis estático sin avisos | Job `static-analysis` del CI (falla con cualquier aviso) | Cumplido: 0 avisos |
| Formato limpio | `dotnet format whitespace` en el CI | Cumplido |
| La escena no tiene avisos de nivel | *Astrolabio > Revisar escena* | Se ejecuta a mano desde el menú; no se guarda el resultado |
| Build de Windows funciona en un equipo limpio | Descarga y ejecución en otro equipo | Sin verificar |
| Rendimiento aceptable en el equipo mínimo | Profiler y prueba en el equipo mínimo de [[03 - Requisitos Técnicos]] | Sin verificar |

## Definición de terminado

Una característica se considera terminada cuando:

1. Cumple su criterio de aceptación de [[04 - Criterios de Aceptación]].
2. Tiene pruebas automáticas que pasan en el CI.
3. El análisis estático y el formato siguen limpios.
4. Está documentada en el GDD (esta bitácora y [[00 - Avance jugable]]).
5. Alguien la jugó a mano con teclado o mando y lo anotó en [[02 - Pruebas]].

Mientras falte el punto 5, la característica figura como **implementada**, no como terminada.

> **Navegación:** [[00 - Índice]] · ← [[05 - Gestión de Cambios]] · [[02 - Pruebas]] →
