# Entornos

| Zona                   | Estilo                                                                                                                      | Función                           |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| Las Entrañas del Reloj | Base del Eje: engranajes del tamaño de edificios, cadenas y polvo; formas casi humanas; latón apagado, óxido y azul profundo | Tutorial y presentación del mundo |
| El Eje Central         | Sala flotante alrededor del eje del Reloj, con el Gran Reloj enorme al fondo, las doce Casas y un cielo estrellado           | Cierre de la demo                 |

El entorno se construye con piezas modulares:

- **Tilesets de 32×32 px** por tipo de superficie: piedra lisa, piedra rugosa (se agarra), metal estelar, rejilla, decorado y pinchos. Se pintan con *Rule Tiles*: basta pintar la forma y el tile elige solo la esquina, el borde o el interior, con costuras continuas.
- **Plataformas** con sprite escalable que no se deforma al alargarse (9-slice).
- **Piezas reutilizables:** faroles, cristales de recarga, checkpoints, compuertas, carteles, engranajes decorativos, fragmento de estrella y poemas.
- **Fondos por capas** de parallax (cielo, estrellas, engranajes lejanos y cercanos).

La iluminación sigue la dirección de arte: luz global baja, luces puntuales cálidas, y un paso gradual de las Entrañas, cálidas y apagadas, al cielo estrellado del Eje Central. Los efectos son polvo al saltar y aterrizar, chispas al enganchar o soltar, destello de la estrella al escribirse, estela con gran velocidad, temblor de cámara y destello en eventos narrativos, y los efectos de muerte y reaparición.

> **Navegación:** [[00 - Índice]] · ← [[02 - Personajes y Animación]] · [[04 - Interfaz Visual]] →
