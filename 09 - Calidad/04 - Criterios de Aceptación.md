# Criterios de Aceptación

## Descripción de la sección

Permiten decidir de forma objetiva si una característica está lista. Cada criterio sigue el formato **Dado que / Cuando / Entonces**. Los valores numéricos salen de la configuración actual del juego y pueden cambiar mientras se ajusta la dificultad.

## Plantilla

### Característica

**Dado que:** contexto inicial

**Cuando:** acción

**Entonces:** resultado esperado

## Criterios de la demo

### Escalada con cuerda

**Dado que** el Almanaque está agarrado a una superficie rugosa con la cuerda llena (100 puntos),
**cuando** se queda colgado, **entonces** la cuerda dura unos 5 s (20 puntos por segundo); **si** sube, dura unos 3 s (33 por segundo); cada salto de escalada gasta 25 puntos.
**Y cuando** pisa suelo, **entonces** la cuerda se rellena.

### Hilo de luz

**Dado que** el jugador tiene usos del hilo (2),
**cuando** dispara hacia algo enganchable a alcance, **entonces** se engancha, gasta un uso y permite balanceo o arrastre.
**Cuando** dispara sin objetivo, **entonces** el hilo sale, se ve hasta dónde llega y vuelve sin gastar usos.
**Cuando** no quedan usos, **entonces** el hilo sale corto y gris.

### Estrella-anclaje

**Dado que** el jugador tiene la habilidad de la estrella,
**cuando** pulsa E en el aire, **entonces** escribe una estrella que sirve de punto de apoyo para el hilo.

### Gas nebuloso

**Dado que** hay gas en la sala,
**cuando** el Almanaque entra en su hitbox, **entonces** muere; **y cuando** el hilo lo cruza, **entonces** se corta.
La línea de apuntado sale en rojo si cruza el gas.

### Muerte y reaparición

**Dado que** el jugador murió por un peligro o aplastamiento,
**cuando** termina la muerte, **entonces** reaparece en el último checkpoint de la sala.

### Elevador del Pozo Celeste

**Dado que** el jugador entra en el elevador de la sala 18,
**cuando** este sube, **entonces** recorre 72 unidades en 12 s y, al llegar arriba, se carga la escena del Eje Central con el jugador sobre la plataforma.

### Cierre de la demo

**Dado que** el Almanaque está en la sala de llegada del Eje Central,
**cuando** cruza las puertas de Géminis, **entonces** la demo termina con la tarjeta final.

## Criterios del proyecto

| Criterio | Estado |
| --- | --- |
| El bucle principal (moverse, escalar, enganchar, morir y reintentar) funciona | Cumplido en pruebas automáticas; falta prueba a mano |
| Las condiciones de victoria y derrota funcionan | Derrota: cumplido. Victoria (cierre de la demo): decidida, por verificar |
| El progreso puede guardarse | No aplica a la demo |
| Los sistemas principales están integrados | Cumplido: mecánicas, interfaz y escenas conectadas por el elevador |
| Las pruebas críticas están aprobadas | Cumplido: 86 EditMode y 212 PlayMode |
| El rendimiento cumple el objetivo definido | Sin medir |
| No existen errores bloqueantes conocidos | Ninguno registrado en [[03 - Bugs y Seguimiento]] |
| La build de Windows se ejecuta en un equipo limpio | Sin verificar |


> **Navegación:** [[00 - Índice]] · ← [[03 - Bugs y Seguimiento]] · [[01 - Glosario]] →
