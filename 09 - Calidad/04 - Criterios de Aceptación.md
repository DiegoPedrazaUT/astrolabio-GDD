# Criterios de Aceptación

Permiten decidir de forma objetiva si una característica está lista. Cada criterio sigue el formato **Dado que / Cuando / Entonces**. Los valores salen de la configuración actual del juego y pueden cambiar mientras se ajusta la dificultad.

## Criterios de la demo

### Escalada con cuerda

**Dado que** el Almanaque está agarrado a una superficie rugosa con la cuerda llena (100 puntos),
**cuando** se queda colgado, **entonces** la cuerda dura unos 5 s (20 puntos por segundo); **si** sube, dura unos 3 s (33 por segundo); cada salto de escalada gasta 25 puntos.
**Y cuando** pisa suelo, **entonces** la cuerda se rellena.

### Gancho de luz

**Dado que** el jugador tiene usos del gancho (2),
**cuando** dispara hacia algo enganchable a alcance, **entonces** se engancha, gasta un uso y permite balanceo o arrastre.
**Cuando** dispara sin objetivo, **entonces** el gancho sale, se ve hasta dónde llega y vuelve sin gastar usos.
**Cuando** no quedan usos, **entonces** el gancho sale corto y gris.

### Estrella ancla

**Dado que** el jugador tiene la habilidad de la estrella,
**cuando** pulsa E en el aire, **entonces** escribe una estrella que sirve de estrella ancla para el gancho.

### Nebulosa

**Dado que** hay una nebulosa en la sala,
**cuando** el Almanaque entra en su hitbox, **entonces** muere; **y cuando** el gancho la cruza, **entonces** se corta.
La línea de apuntado sale en rojo si cruza la nebulosa.

### Muerte y reaparición

**Dado que** el jugador murió por un peligro o aplastamiento,
**cuando** termina la muerte, **entonces** reaparece en el último checkpoint de la sala.

### Guardado

**Dado que** el jugador entra en una sala nueva, toma un checkpoint o recibe una habilidad,
**cuando** ocurre cualquiera de los tres, **entonces** la partida se guarda en el registro elegido.
**Y cuando** el jugador cierra el juego y pulsa Continuar, **entonces** reaparece en la sala o checkpoint guardado con sus habilidades.

### Elevador del Pozo Celeste

**Dado que** el jugador tomó el fragmento de estrella y entra en el elevador de la sala 18,
**cuando** este sube, **entonces** recorre 72 unidades en 12 s y hace la animación de salida sin cambiar de escena.
**Y si** el jugador no tiene el fragmento, **entonces** el elevador no se puede usar.

### Final de la demo

**Dado que** el elevador terminó de subir,
**cuando** acaba la conversación final, **entonces** aparece la tarjeta con las estadísticas (tiempo, muertes y poemas) y el mensaje «Gracias por jugar la demo».
**Y cuando** el jugador pulsa «Volver al título», o pasan 30 s, **entonces** vuelve al menú principal.

## Criterios del proyecto

| Criterio | Estado |
| --- | --- |
| El bucle principal (moverse, escalar, enganchar, morir y reintentar) funciona | Cumplido en pruebas automáticas; falta prueba a mano |
| Las condiciones de victoria y derrota funcionan | Derrota: cumplido. Victoria (final de la demo en el elevador): en implementación |
| El progreso puede guardarse | Aprobado el 10/11/2026; en implementación |
| Los sistemas principales están integrados | Mecánicas, interfaz y audio integrados; faltan el final de la demo y el guardado |
| Las pruebas críticas están aprobadas | Cumplido: 86 EditMode y 212 PlayMode |
| El rendimiento cumple el objetivo definido | Sin medir |
| No existen errores bloqueantes conocidos | Ninguno registrado en [[03 - Bugs y Seguimiento]] |
| La build de Windows se ejecuta en un equipo limpio | Sin verificar |

> **Navegación:** [[00 - Índice]] · ← [[03 - Bugs y Seguimiento]] · [[01 - Glosario]] →
