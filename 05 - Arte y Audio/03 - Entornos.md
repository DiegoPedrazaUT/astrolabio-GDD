# Entornos

## Descripción de la sección

Define la estética y necesidades visuales de escenarios, fondos, objetos y elementos ambientales.

## Zonas

| Zona                                                         | Estilo                                                                                                                           | Elementos                                                                                        | Función                                             |
| ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| Las Entrañas del Reloj                                       | Base del Eje: engranajes del tamaño de edificios, cadenas y polvo; formas casi humanas; latón apagado, óxido y azul profundo | Nichos, galería de engranajes, puente roto, pozo de cadenas, pozo celeste                        | Tutorial y presentación del mundo                   |
| El Eje Central                                               | Sala flotante alrededor del eje del Reloj, con el Gran Reloj enorme al fondo y las doce Casas; cielo estrellado                  | Llegada del elevador, puertas de Géminis, faroles                                                | Cierre de la demo y futuro selector de Casas        |

## Modularidad

- **Tilesets de 32×32 px** por tipo de superficie: piedra lisa, piedra rugosa (se agarra), metal estelar, rejilla, decorado y pinchos. Se pintan con *Rule Tiles*: cada superficie es un solo tile con reglas que elige por sí mismo la esquina, el borde o el interior según los tiles vecinos, así que basta pintar la forma y las costuras salen continuas (ver [[05 - Gestión de Cambios]]).
- **Plataformas** con un sprite escalable que no se deforma al alargarse (9-slice).
- **Piezas reutilizables:** faroles, cristales de recarga, checkpoints, compuertas, carteles y engranajes decorativos.
- **Fondos por capas** de parallax (cielo, estrellas, engranajes lejanos y cercanos) que se comparten entre zonas con otra paleta de uso.

## Iluminación

Describe iluminación global, fuentes de luz y cambios durante el juego.

- **Global:** baja, para que el fondo sea siempre más oscuro que el primer plano.
- **Puntuales:** faroles, cristales, checkpoints, nichos, el Astrolabio y el propio personaje.
- **Zonas de luz:** al entrar a un túnel oscuro baja la luz global y se recupera al salir.
- **Evolución:** las Entrañas son cálidas y apagadas; el Eje Central se abre a un cielo estrellado.
- **Post-proceso:** bloom suave, viñeta y ajuste de color.

## Efectos visuales

- **Partículas:** polvo al saltar y aterrizar, chispas al enganchar o soltar el hilo.
- **Clima:** no hay.
- **Fuego:** no hay.
- **Magia / energía:** destello de la estrella al escribirse, estela con gran velocidad, el hilo de luz.
- **Impactos:** temblor de cámara y destello en eventos narrativos; efecto de muerte y de reaparición.

## Recursos requeridos

Lista los modelos, sprites, texturas, materiales y efectos necesarios.

- Tileset de 32×32 px de cada zona (Entrañas), armado como *Rule Tiles*, con las seis superficies.
- Fondos de parallax (3 a 4 capas por zona).
- Piezas de nivel: faroles, plataformas (patrulla, zip, rejilla, losa y elevador), cristal de recarga, checkpoint, pinchos, compuertas, fragmento de estrella y poemas.
- Carteles de controles y rótulos de zona.
- Holograma de Efeméride.
- Efectos de partículas del personaje y del mundo.


> **Navegación:** [[00 - Índice]] ·  [[02 - Personajes y Animación]] · [[04 - Interfaz Visual]] →
