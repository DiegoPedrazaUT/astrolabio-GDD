# Seguridad y Riesgos Técnicos

## Descripción de la sección

Documenta riesgos técnicos y medidas para reducir fallos, pérdida de datos o abuso de sistemas.

## Riesgos

| Riesgo                                                | Probabilidad | Impacto | Mitigación                                                                                    |
| ----------------------------------------------------- | ------------ | ------- | --------------------------------------------------------------------------------------------- |
| El apuntado con mando es impreciso                    | Media        | Medio   | Ayuda de puntería ajustable y pruebas con un mando físico                                     |

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
- **Fallo del programa:** al reiniciar, "Continuar" regresa al último punto guardado (observatorio mayor o ascensor).
- **Pérdida de trabajo del equipo:** el repositorio remoto y las ramas de Gitflow permiten recuperar versiones anteriores.


> **Navegación:** [[00 - Índice]] · ← [[04 - Datos y Persistencia]] · [[01 - Alcance]] →
