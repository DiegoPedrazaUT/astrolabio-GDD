# Bugs y seguimiento

Los fallos de las pruebas a mano (teclado, ratón, mando y WebGL) se añaden a este registro.

| ID     | Bug                                                                                                                                                  | Severidad | Área          | Estado                                                                       |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | ------------- | ---------------------------------------------------------------------------- |
| BUG-01 | Las habilidades no pasaban de una escena a otra: en el Eje Central el jugador las tenía porque el prefab `Player` las traía activadas | Media | Programación | Cerrado el 10/11/2026: ya no hay cambio de escena; el guardado restaura las habilidades |
| BUG-02 | El CI fallaba siempre con `no space left on device` al bajar la imagen de Unity                                                                      | Alta      | DevOps        | Resuelto el 29/10/2026                                                       |
| BUG-03 | El Editor moría a los segundos de abrir el proyecto en el CI (código 137) por una caché de `Library` en mal estado                                   | Alta      | DevOps        | Mitigado: se versionaron las claves de caché                                 |
| BUG-04 | La caída tenía un límite de 21,4 en lugar de 20                                                                                                      | Baja      | Programación  | Resuelto el 27/10/2026                                                       |
| BUG-05 | El deslizamiento en pared iba a 4,4 aunque el diseño decía 3                                                                                         | Baja      | Programación  | Resuelto el 29/10/2026                                                       |
| BUG-06 | Unity se bloquea con el diálogo «Scene(s) Have Been Modified» si se lanzan pruebas tras guardar una escena por script                                | Baja      | Herramientas  | Conocido: hay que cerrar el diálogo en el Editor                             |

## Limitaciones conocidas (no son bugs)

| Tema                          | Descripción                                                                                                    |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Salto desde la plataforma zip | A media carrera el impulso se queda corto (tope de 14 frente a 20 de la plataforma); se salta al final o ya frenada |
| Velocidad en el aire          | Solo dura la velocidad que supera la de carrera (7,6); saltar desde una plataforma lenta no lanza              |
| Nebulosa y cuerda             | Una cuerda que pasa por debajo de la nebulosa no se corta: al colocarla hay que dejar sitio al balanceo         |
| Salas junto a un muro         | Si el borde de una sala coincide con un muro, el límite se pone detrás del muro                                |
| Reinicio en el evento         | El registro se borra a mano con «Borrar registro» entre jugador y jugador; no hay modo evento                  |

> **Navegación:** [[00 - Índice]] · ← [[02 - Pruebas]] · [[04 - Criterios de Aceptación]] →
