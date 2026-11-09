# Seguridad y Riesgos Técnicos

## Riesgos

| Riesgo                                                | Probabilidad | Impacto | Mitigación                                                                                    |
| ----------------------------------------------------- | ------------ | ------- | --------------------------------------------------------------------------------------------- |
| El apuntado con mando es impreciso                    | Media        | Medio   | Ayuda de puntería ajustable y pruebas con un mando físico                                     |
| La física del gancho (balanceo, cuerda que se dobla en las esquinas) es inestable o impredecible | Media | Alto | Física en paso fijo, salas de prueba aisladas y pruebas automáticas de cada mecánica |
| Los límites de una sala cortan un balanceo o dejan la cámara fija | Media | Medio | Margen en los límites de cada sala y revisión con Cinemachine sala por sala |
| El archivo de partida se corrompe o se pierde | Baja | Alto | Copia de respaldo antes de escribir; si falla, aviso y partida nueva sin borrar el archivo dañado |
| Cambia la estructura de los datos entre versiones | Media | Medio | Número de versión en cada archivo y valores predeterminados para los campos nuevos |
| Conflictos al combinar escenas y prefabs en Git | Alta | Medio | Gitflow, Git LFS, una persona por escena y no editar a mano los archivos .unity, .prefab ni .meta |
| El rendimiento baja de 60 FPS por las luces 2D y el post-proceso | Baja | Medio | Medir en la build y ofrecer la opción de calidad de efectos |
| El pixel art se deforma o tiembla al escalar | Media | Medio | Filtro de píxel en todas las texturas, tiles sin costuras y vista base de 1280×720 (escala ×1,5 en 1080p; entera en 720p, 1440p y 2160p) |
| La build de Windows no se ejecuta en un equipo limpio | Baja | Alto | Probar la build en un equipo sin Unity antes de publicarla en itch.io |

## Datos sensibles

**¿El juego almacena información personal, cuentas, estadísticas en línea u otros datos?**

No. No hay cuentas, datos personales, estadísticas en línea ni conexión a internet. El único archivo del jugador es su partida y su configuración, guardados de forma local.

## Multijugador

Si existe conexión en red, documentar:

No aplica: el juego es de un jugador y no usa red. No hay autenticación, validación, autoridad de servidor ni protección contra manipulación.

## Recuperación

- **Corrupción de datos:** se usa la copia de respaldo; si no sirve, el juego avisa y ofrece una partida nueva sin borrar el archivo dañado.
- **Pérdida de conexión:** no aplica.
- **Fallo del programa:** con el guardado implementado, "Continuar" regresará al último punto guardado; en la demo actual no hay guardado y se empieza de nuevo.
- **Pérdida de trabajo del equipo:** el repositorio remoto y las ramas de Gitflow permiten recuperar versiones anteriores.

> **Navegación:** [[00 - Índice]] · ← [[04 - Datos y Persistencia]] · [[01 - Alcance]] →
