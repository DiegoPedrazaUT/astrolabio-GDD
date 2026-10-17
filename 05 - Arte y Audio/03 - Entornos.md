# Entornos

## Descripción de la sección

Define la estética y necesidades visuales de escenarios, fondos, objetos y elementos ambientales.

## Zonas

| Zona                  | Estilo                                                                                          | Elementos                                                                                   | Función                                              |
| --------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| Las Entrañas del Reloj | Base de la torre: engranajes del tamaño de edificios, cadenas y polvo; formas casi humanas; latón apagado, óxido y azul profundo | Nichos, galería de engranajes, puente roto, pozo de cadenas, pozo celeste                     | Tutorial y presentación del mundo                    |
| El Eje                | Columna de maquinaria que atraviesa el Reloj                                                    | Ascensor de engranajes, raíles, cadenas                                                      | Transición entre zonas (sirve de pantalla de carga)  |
| Casa de Géminis       | Dos torres gemelas unidas por puentes: una pulida y dorada, la otra oxidada y agrietada          | Espejos, muros espejo, puentes paralelos, losas doradas y azules, observatorio de las Dos Lentes | Reflejos y anclaje reflejado                         |
| Casa de Acuario       | Un ánfora gigante, inclinada y agrietada, de la que caen cascadas de luz                         | Corrientes, acueductos, esclusas, remolino, muros mojados, observatorio del Cauce            | Física del entorno: corrientes y agua                |
| Observatorio de Ofiuco y Cámara Central *(versión completa)* | Cúpula rodeada por una serpiente de hierro; cámara circular donde convergen los engranajes | Cuerpo de XI, telescopio gigante, prisión abierta de Ofiuco                         | Clímax y desenlace                                   |

## Modularidad

¿Qué elementos pueden reutilizarse?

- **Tilesets de 16×16 px** por tipo de superficie: piedra lisa, piedra rugosa, metal estelar, rejilla, decorado y pinchos. Se pintan **a mano** sobre la cuadrícula con *Tile Palette*, con cada esquina, borde e interior como un tile independiente. **No se usan *Rule Tiles*** (ver [[03 - Registro de Decisiones]]).
- **Plataformas** con un sprite escalable que no se deforma al alargarse (9-slice).
- **Piezas reutilizables:** faroles, cristales de recarga, checkpoints, compuertas, carteles y engranajes decorativos.
- **Fondos por capas** de parallax (cielo, estrellas, engranajes lejanos y cercanos) que se comparten entre zonas con otra paleta de uso.

## Iluminación

Describe iluminación global, fuentes de luz y cambios durante el juego.

- **Global:** baja, para que el fondo sea siempre más oscuro que el primer plano.
- **Puntuales:** faroles, cristales, checkpoints, nichos, el Astrolabio y el propio personaje.
- **Zonas de luz:** al entrar a un túnel oscuro baja la luz global y se recupera al salir.
- **Evolución:** las Entrañas son cálidas y apagadas; Géminis alterna dorado y óxido; Acuario es más fría y húmeda; el desenlace cambia según la decisión final.
- **Post-proceso:** bloom suave, viñeta y ajuste de color.

## Efectos visuales

- **Partículas:** polvo al saltar y aterrizar, chispas al enganchar o soltar el hilo.
- **Clima:** no hay.
- **Humo:** vapor en Acuario (el agua que sube al cielo).
- **Fuego:** no hay.
- **Agua:** corrientes, cascadas y muros mojados.
- **Magia / energía:** destello de la estrella al escribirse, estela con gran velocidad, el hilo de luz.
- **Impactos:** temblor de cámara y destello en eventos narrativos; efecto de muerte y de reaparición.

## Recursos requeridos

Lista los modelos, sprites, texturas, materiales y efectos necesarios.

- Tileset de cada zona (Entrañas, Géminis y Acuario) con las seis superficies.
- Fondos de parallax (3 a 4 capas por zona).
- Piezas de nivel: faroles, plataformas (patrulla, zip, rejilla, losa y elevador), cristal de recarga, checkpoint, pinchos, compuertas, fragmento de estrella y poemas.
- Piezas de Casa: espejos y reflejo (Géminis); corrientes, esclusas y remolino (Acuario).
- Carteles de controles y rótulos de zona.
- Hologramas de la Tierra y de Efeméride.
- Efectos de partículas del personaje y del mundo.


> **Navegación:** [[00 - Índice]] · ← [[02 - Personajes y Animación]] · [[04 - Interfaz Visual]] →
