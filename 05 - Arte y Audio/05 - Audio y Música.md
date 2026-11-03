# Audio y Música

## Descripción de la sección

Define la identidad sonora y cómo el audio comunica información al jugador.

## Música

**Estilo:**
Ambiental, melancólico y cálido. Debe acompañar sin competir con la concentración que exige el juego.

**Instrumentación:**
Bajos, cuerdas, pads, guitarras, piano, sintetizadores y el tic-tac del Reloj.

**Temas principales:**
- Un tema por nivel, acorde a su ambiente: Entrañas, Géminis y final. 
- Un tema independiente para el menú, que será el tema principal del juego. 
- El tema de las Entrañas (el tutorial) es una versión de solo piano del tema principal.

**Música dinámica:** Sí.
La música se adaptará (volumen, ritmo, melodía o instrumentación) según lo que el jugador haga o el momento del juego.

Responsable: audio (ver [[02 - Roles y Responsabilidades]]).

## Efectos de sonido

| Evento                          | Sonido                                          | Propósito                          |
| ------------------------------- | ----------------------------------------------- | ---------------------------------- |
| Saltar                          | Resorte corto                                   | Confirmar el despegue              |
| Aterrizar                       | Golpe seco de metal                             | Confirmar el contacto con el suelo |
| Agarrarse a la pared            | Clic metálico                                   | Confirmar el agarre                |
| Cuerda a punto de agotarse      | Clic acelerado                                  | Avisar sin mirar el HUD            |
| Hilo: enganchar                 | Chasquido metálico con chispa                   | Confirmar el enganche              |
| Hilo: soltar o cortar           | Silbido corto                                   | Indicar que se perdió el enganche  |
| Pulsar el hilo sin usos         | Tono apagado                                    | Avisar que no quedan usos          |
| Escribir una estrella           | Campanilla suave                                | Confirmar que el anclaje existe    |
| Anclaje que caduca              | Desvanecimiento suave                           | Avisar que desaparece              |
| Cristal de recarga              | Campanilla cristalina                           | Indicar que los usos volvieron     |
| Muerte                          | Chasquido de engranaje                          | Cerrar el intento sin castigar     |
| Reaparición                     | Tic-tac seco                                    | Indicar que se puede reintentar    |
| Fragmento de estrella           | Acorde cálido                                   | Marcar un logro                    |
| Diálogo de Efeméride            | Un sonido por letra, distinto según el hablante | Dar voz al texto sin grabar voz    |
| Plataformas y ascensor          | Engranajes y cadenas                            | Dar peso al Reloj                  |
| Dar cuerda a la llave           | Giro de llave                                   | Marcar el guardado                 |

## Audio espacial

¿Se utilizará audio posicional?

No. El audio es 2D: cada sala tiene su propio ambiente y se funde al cambiar de sala. Los sonidos continuos importantes (como el tic-tac y los engranajes) pueden bajar de volumen con la distancia al jugador.

## Voz

**Narración:** No hay.

**Diálogos hablados:** No hay voz grabada: Efeméride habla con burbujas de texto y un sonido por letra. El Almanaque no habla.

**Idiomas:** Textos en español (base); el inglés está por confirmar.

## Mezcla

Define prioridades, volumen relativo y comportamiento de la música ante eventos importantes.

1. Efectos del jugador (deben oírse siempre).
2. Diálogo de Efeméride.
3. Música.
4. Ambiente de la sala.

- La música baja de volumen durante las conversaciones y se recupera al terminar.
- El volumen de música, efectos y ambiente es independiente (ver [[04 - Guardado y Configuración]]).
- Los recursos de terceros deben tener una licencia que permita su uso en el proyecto y se atribuyen en los créditos.


> **Navegación:** [[00 - Índice]] · ← [[04 - Interfaz Visual]] · [[01 - UX y Flujo del Jugador]] →
