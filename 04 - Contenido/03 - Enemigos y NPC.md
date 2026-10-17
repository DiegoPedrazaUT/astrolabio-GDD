# Enemigos y NPC

## Descripción de la sección

Documenta las entidades controladas por el juego y su comportamiento.

## Enemigos

El juego **no tiene enemigos ni combate**. El peligro es el entorno: un toque mata y el jugador reaparece al inicio de la sala. Por eso las plantillas de enemigo y de IA no aplican.

## Peligros del entorno

| Peligro                | Comportamiento                                                                                  | Efecto                                    |
| ---------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------- |
| Pinchos                | Estáticos; matan al rozarlos (con la caja de colisión reducida para no matar al pararse al borde). Su aspecto final será de engranajes u otro elemento del espacio | Muerte y reaparición |
| Vacío                  | Caer fuera de las plataformas                                                                    | Muerte y reaparición                      |
| Aplastamiento          | Una plataforma o un sólido atrapa al jugador contra una pared, el suelo o el techo                | Muerte y reaparición                      |
| Losas que se rompen    | Tiemblan al pisarlas o agarrarlas, se rompen y reaparecen                                        | Pérdida del apoyo                         |
| Farol que se apaga     | Un anclaje que corta el hilo por ciclos o tras un solo enganche                                  | Pérdida del enganche                      |
| Esclusas y corrientes  | Fuerzas que empujan al jugador por ciclos                                                        | Cambian el movimiento                     |

## Plantilla de NPC

### Efeméride

**Nombre:** Efeméride.

**Función:** Guía narrativa y de tutorial; la voz del Gran Reloj Cósmico.

**Ubicación:** Aparece como holograma al inicio y al final de las zonas, en las indicaciones de recorrido y en los hologramas de la Tierra. Nunca dentro de un observatorio.

**Interacción:** No se conversa con ella: habla en burbujas de texto y el jugador solo escucha. Las conversaciones se pueden saltar manteniendo Espacio.

**Diálogos:** Ver [[04 - Diálogos y Narrativa]].

**Condiciones:** Se activan por zona o al terminar un observatorio.

**Recompensas / información:** Los controles, el contexto de la misión y, sin quererlo, las pistas de lo que oculta.

### Otros NPC

No hay otros NPC. El equipo ha hablado de NPC al estilo de Celeste, pero no hay ninguno definido. Sus únicos «habitantes» son el reflejo del jugador en Géminis (una copia suya, no un NPC) y el holograma del Almanaque que muestra los controles en el tutorial.


> **Navegación:** [[00 - Índice]] · ← [[02 - Niveles]] · [[04 - Objetos y Coleccionables]] →
