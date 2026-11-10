# Audio y música

Responsable: audio (ver [[02 - Roles y Responsabilidades]]).

## Música

**Estilo:** ambiental, melancólico y cálido. Acompaña sin competir con la concentración que exige el juego.

**Base sonora permanente:** tres capas suenan desde que arranca el juego hasta que termina, sin cortes entre escenas:

- El tic-tac del Reloj.
- Un pad.
- Un ambiente espacial.

**Canciones por zona:**

| Zona               | Música                                                      |
| ------------------ | ----------------------------------------------------------- |
| Los Nichos         | Sin canción: solo pad, ambiente y reloj                      |
| La Galería         | La Galería Dormida → Luz entre Engranajes                    |
| El Puente Roto     | Sobre el Puente Roto                                         |
| El Pozo de Cadenas | Cadenas que Cantan → Memorias Celestes (entra poco a poco)   |
| El Pozo Celeste    | Memorias Celestes                                            |

**Música dinámica:** sí, por zonas.

- La canción cambia al entrar en otra sala.
- Una canción puede entrar poco a poco a lo largo de varias salas.
- Al volver a una sala anterior, la música se ajusta a esa sala.
- El pad baja a la mitad mientras suena una canción y vuelve a su volumen en las zonas sin canción.
- La música no cambia de ritmo, melodía ni instrumentación según lo que haga el jugador.

## Efectos de sonido

| Evento                           | Sonido                                                                  | Propósito                                      |
| -------------------------------- | ----------------------------------------------------------------------- | ---------------------------------------------- |
| Saltar                           | Tono corto que sube (estilo retro)                                      | Confirmar el despegue                          |
| Aterrizar                        | Golpe sobre piso de chapa; más fuerte cuanto más alta la caída          | Confirmar el contacto con el suelo             |
| Gancho: enganchar                | Chasquido metálico y «zing» del hilo tenso                              | Confirmar el enganche                          |
| Gancho: impulso                  | La misma mordida, con un «zing» que sube y el carrete acelerando        | Distinguir el impulso del balanceo             |
| Escribir una estrella ancla      | Clic de latón y campana celeste con eco                                 | Confirmar que la estrella ancla existe         |
| Cristal de recarga (estrella verde) | Destellos de cristal que suben                                       | Indicar que los usos y la cuerda volvieron     |
| Checkpoint                       | Dos campanadas cortas que suben                                         | Confirmar que el progreso quedó guardado       |
| Muerte                           | Estallido del astrolabio: golpe grave y chapa rompiéndose               | Cerrar el intento                              |
| Engranajes y sierras             | Loop de engranajes que crece al acercarse                               | Avisar del peligro antes de verlo              |
| Plataformas móviles y elevador   | Motor con engranaje reductor; al subirse, pasa al frente                | Dar peso a los mecanismos del Reloj            |
| Plataforma rompible              | Chapa oxidada que gime (aviso) y crujido de metal viejo (rotura)        | Avisar y confirmar la ruptura                  |
| Nombre de zona en pantalla       | Soplo de aire, «bum» grave y brillo                                     | Marcar la entrada a una sección nueva          |

Los eventos que faltan por sonorizar (fin de la demo, lectura de un poema y guardado) deben lanzar su propio evento para que audio ponga el sonido.

## Audio espacial

El audio es posicional en 2D:

- Los **sonidos del mundo** (engranajes, plataformas, compuertas, rompibles, elevador) suenan desde donde están: se oyen por el lado correcto y bajan con la distancia a la cámara hasta apagarse.
- Los **sonidos del jugador**, el checkpoint, el cristal de recarga, la interfaz, la música y la base permanente se oyen igual en cualquier sitio.
- No hay un ambiente distinto por sala: la base (reloj, pad y espacio) es la misma en todo el juego, y lo que cambia por zona es la música.

## Voz

No hay narración ni voz grabada. Efeméride habla con burbujas de texto; el Almanaque no habla. Los textos están en español.

## Mezcla

**Grupos del mezclador:** Master → Music (canciones y pad), Ambience (reloj y espacio), SFX → Player y World, y UI.

**Prioridad** (de más a menos importante):

1. Efectos del jugador (deben oírse siempre).
2. Música.
3. Efectos del mundo.
4. Base permanente (reloj, pad y espacio).

El volumen general, el de la música, el de los efectos y el del ambiente son independientes (ver [[04 - Guardado y Configuración]]). Los recursos de terceros deben tener una licencia que permita su uso y se atribuyen en los créditos.

> **Navegación:** [[00 - Índice]] · ← [[04 - Interfaz Visual]] · [[06 - Registro visual]] →
