# Seguridad y riesgos técnicos

El juego no tiene cuentas, datos personales, estadísticas en línea, multijugador ni conexión a internet. Lo único que almacenará es la partida y la configuración, de forma local.

| Riesgo                                                           | Prob. | Impacto | Mitigación                                                                                           |
| ---------------------------------------------------------------- | ----- | ------- | ---------------------------------------------------------------------------------------------------- |
| El apuntado con mando es impreciso                               | Media | Medio   | Ayuda de puntería ajustable y pruebas con un mando físico                                            |
| La física del gancho (cuerda que se dobla en esquinas) es inestable | Media | Alto | Física en paso fijo, salas de prueba aisladas y pruebas automáticas de cada mecánica                 |
| Los límites de una sala cortan un balanceo o dejan la cámara fija | Media | Medio  | Margen en los límites de cada sala y revisión con Cinemachine sala por sala                          |
| El archivo de partida se corrompe o se pierde (cuando exista)    | Baja  | Alto    | Copia de respaldo antes de escribir; si falla, aviso y partida nueva sin borrar el archivo dañado    |
| Conflictos al combinar escenas y prefabs en Git                  | Alta  | Medio   | Gitflow, Git LFS, una persona por escena y no editar a mano los `.unity`, `.prefab` ni `.meta`       |
| El rendimiento baja de 60 FPS por las luces 2D y el post-proceso | Baja  | Medio   | Medir en la build y ofrecer la opción de calidad de efectos                                          |
| El pixel art se deforma o tiembla al escalar                     | Media | Medio   | Filtro de píxel, tiles sin costuras y vista base de 1280×720                                         |
| La build de Windows no se ejecuta en un equipo limpio            | Baja  | Alto    | Probar la build en un equipo sin Unity antes de publicarla en itch.io                                |

La pérdida de trabajo del equipo se cubre con el repositorio remoto y las ramas de Gitflow.

> **Navegación:** [[00 - Índice]] · ← [[04 - Datos y Persistencia]] · [[01 - Alcance]] →
