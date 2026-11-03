# Seguridad y Riesgos Técnicos

## Descripción de la sección

Documenta riesgos técnicos y medidas para reducir fallos, pérdida de datos o abuso de sistemas.

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
| El pixel art se deforma o tiembla al escalar | Media | Medio | Escala entera (×3 sobre 640×360) y filtro de píxel en todas las texturas |
| La build de Windows no se ejecuta en un equipo limpio | Baja | Alto | Probar la build en un equipo sin Unity antes de publicarla en itch.io |

## Datos sensibles

¿El juego almacena información personal, cuentas, estadísticas en línea u otros datos?

No. No hay cuentas, datos personales, estadísticas en línea ni conexión a internet. El único archivo del jugador es su partida y su configuración, guardados de forma local.

## Multijugador

Si existe conexión en red, documentar:

No aplica: el juego es de un jugador y no usa red. No hay autenticación, validación, autoridad de servidor ni protección contra manipulación.

## Recuperación

¿Qué ocurre ante corrupción de datos, pérdida de conexión o fallo del programa?

- **Corrupción de datos:** se usa la copia de respaldo; si no sirve, el juego avisa y ofrece una partida nueva sin borrar el archivo dañado.
- **Pérdida de conexión:** no aplica.
- **Fallo del programa:** al reiniciar, "Continuar" regresa al último punto guardado (el último ascensor tomado).
- **Pérdida de trabajo del equipo:** el repositorio remoto y las ramas de Gitflow permiten recuperar versiones anteriores.


> **Navegación:** [[00 - Índice]] · ← [[04 - Datos y Persistencia]] · [[01 - Alcance]] →
