# Criterios de calidad

En un plataformas de precisión, la calidad se juega en tres cosas: que los controles respondan, que cada muerte se sienta justa y que el jugador entienda qué puede agarrar y qué lo mata. Una prueba automática verifica la regla; solo una persona jugando verifica la sensación.

| Criterio                                                                   | Cómo se comprueba                                        | Estado                                          |
| -------------------------------------------------------------------------- | -------------------------------------------------------- | ----------------------------------------------- |
| Cada mecánica cumple las reglas de [[02 - Mecánicas]]                      | Pruebas automáticas (ver [[02 - Pruebas]])               | Cumplido (07/11/2026)                           |
| La cuerda del gancho no atraviesa sólidos, tampoco a toda velocidad        | 1350 recorridos automáticos                              | Cumplido (07/11/2026)                           |
| Muerte y reaparición llevan siempre a un punto válido                      | Revisor de escena y pruebas de reaparición               | Cumplido (07/11/2026)                           |
| Pruebas EditMode y PlayMode en verde                                       | CI en cada PR                                            | Cumplido: 86 y 212 (07/11/2026)                 |
| Análisis estático y formato sin avisos                                     | CI (`static-analysis` y `dotnet format`)                 | Cumplido: 0 avisos                              |
| Las habilidades se conservan entre escenas                                 | Prueba manual del cambio de escena                       | No cumplido: ver [[03 - Bugs y Seguimiento]]    |
| El jugador entiende el objetivo de cada sala y por qué murió               | Prueba con jugadores nuevos                              | Sin verificar                                   |
| La dificultad crece sin saltos (ver [[05 - Progresión]])                   | Prueba con jugadores nuevos                              | Sin verificar                                   |
| Lo que se agarra se distingue de lo que no                                 | Revisión con [[06 - Registro visual]] y jugadores        | Sin verificar                                   |
| Los controles responden igual con teclado y con mando                      | Prueba a mano con ambos                                  | Sin verificar                                   |
| La interfaz se lee a 1280×720, 1600×900 y 1920×1080                        | Revisión en cada resolución                              | Sin verificar                                   |
| La build de Windows funciona en un equipo limpio y rinde bien en el mínimo | Ejecución en otro equipo y Profiler ([[03 - Requisitos Técnicos]]) | Sin verificar                         |

Una característica está **terminada** cuando cumple su criterio de [[04 - Criterios de Aceptación]], tiene pruebas automáticas en verde, mantiene limpios el análisis estático y el formato, está documentada en el GDD y alguien la jugó a mano y lo anotó en [[02 - Pruebas]]. Mientras falte esto último, figura como **implementada**.

> **Navegación:** [[00 - Índice]] · ← [[05 - Gestión de Cambios]] · [[02 - Pruebas]] →
