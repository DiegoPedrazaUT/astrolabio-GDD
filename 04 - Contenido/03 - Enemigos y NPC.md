# Enemigos y NPC

## Descripción de la sección

Documenta las entidades controladas por el juego y su comportamiento.

## Enemigos

El juego **no tiene enemigos ni combate**. El peligro es el entorno: un toque mata y el jugador reaparece al inicio de la sala o en su último checkpoint. Por eso las plantillas de enemigo y de IA no aplican.

## Peligros del entorno

| Peligro             | Comportamiento                                                                                                                                                                                  | Efecto               |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------- |
| Engranajes letales  | Giran en su sitio; matan al rozarlos. Su zona de daño es un círculo algo menor que el dibujo, para que no maten al jugador cuando se detiene en el borde.                                         | Muerte y reaparición |
| Sierras             | Engranajes semihundidos en la pared o el suelo; matan por contacto en la franja que asoma.                                                                                                      | Muerte y reaparición |
| Gas nebuloso        | Estático; mata al tocarlo y corta el hilo del gancho si lo cruza. La línea de apuntado se vuelve roja ante él.                                                                                   | Muerte y reaparición, o pérdida del enganche |
| Vacío               | Caer fuera de las plataformas                                                                                                                                                                   | Muerte y reaparición |
| Aplastamiento       | Una plataforma o un sólido atrapa al jugador contra una pared, el suelo o el techo                                                                                                              | Muerte y reaparición |
| Losas que se rompen | Tiemblan al pisarlas o agarrarlas, se rompen y reaparecen                                                                                                                                       | Pérdida del apoyo    |
| Farol que se apaga  | Un punto de enganche que corta el hilo por ciclos o tras un solo enganche                                                                                                                       | Pérdida del enganche |

## Plantilla de NPC

### Efeméride

**Nombre:** Efeméride.

**Función:** Guía narrativa y de tutorial; la voz del Gran Reloj Cósmico.

**Ubicación:** Aparece como holograma al inicio y al final de las zonas, y en las indicaciones de recorrido.

**Interacción:** No se conversa con ella: habla en burbujas de texto y el jugador solo escucha. Las conversaciones se pueden saltar manteniendo Espacio.

**Diálogos:** Ver [[04 - Diálogos y Narrativa]].

**Condiciones:** Sus intervenciones se activan al entrar en una zona.

**Recompensas / información:** Los controles, el contexto de la misión y, sin quererlo, las pistas de lo que oculta.

### Otros NPC

No hay otros NPC. El equipo ha considerado incluir NPC al estilo de Celeste, pero aún no hay ninguno definido. El único otro «habitante» del Reloj, además de Efeméride, es el reflejo del jugador en Géminis (una copia suya, no un NPC).

> **Navegación:** [[00 - Índice]] · ← [[02 - Niveles]] · [[04 - Objetos y Coleccionables]] →
