# UX y Flujo del Jugador

## Descripción de la sección

UX (experiencia de usuario) describe qué tan comprensible, cómoda y coherente resulta la interacción con el videojuego.

## Flujo principal

```text
Inicio → Menú → Nueva partida → Introducción con Efeméride → Entrañas del Reloj (tutorial)
       → Ascensor y dial de Casas → Casa de Géminis / Casa de Acuario → Juego ⇄ Pausa
       → Observatorio de Ofiuco → Cámara Central → Final → Créditos
```

En la demo, el recorrido termina con la tarjeta final al restaurar las dos Casas jugables.

## Primeros minutos

Documenta exactamente qué descubre y aprende el jugador.

El objetivo es que el jugador entienda cada herramienta jugándola, no leyendo. Cada idea nueva se presenta primero en un espacio seguro y después se examina con riesgo.

| Momento (objetivo) | Qué descubre                                                                                                                        |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| Minuto 0           | Despierta en un nicho y escucha a Efeméride. No controla al personaje hasta la última burbuja de texto.                             |
| Minutos 1 a 3      | Aprende a moverse y a saltar en la Sala de los Nichos, por demostraciones  en el escenario.                                         |
| Minutos 3 a 6      | Aprende a agarrarse y escalar en la Galería de Engranajes; descubre que su aguante (stamina)  se agota y se recarga al tocar suelo. |
| Minutos 6 a 9      | Recibe el gancho en el Puente Roto: balanceo, arrastre y faroles.                                                                   |
| Minutos 9 a 14     | Pone a prueba todo lo aprendido en el Pozo de Cadenas y recibe el astrolabio en el Pozo Celeste.                                    |
| Minuto 14 a 15     | Obtiene el primer fragmento de estrella y elige hacia qué Casa subir.                                                               |

Para enseñar los controles se usa y un holograma del Almanaque que repite el movimiento y desaparece cuando el jugador lo logra.

## Retroalimentación

Para cada acción importante define:

**Entrada → Respuesta visual → Respuesta sonora → Resultado**

| Entrada                     | Respuesta visual                                               | Respuesta sonora       | Resultado                               |
| --------------------------- | -------------------------------------------------------------- | ---------------------- | --------------------------------------- |
| Saltar                      | Polvo y chispa breve; aplastar y estirar del personaje         | Salto pesado           | El personaje salta                      |
| Aterrizar                   | Polvo; aplastar del personaje                                  | Golpe seco de metal    | Se recargan los usos                    |
| Agarrarse a la pared        | El personaje se aferra; la estamina se consume                 | Clic metálico          | Puede escalar mientras haya cuerda      |
| Cuerda por agotarse         | La llave tiembla y parpadea en rojo                            | Clic acelerado         | El jugador decide dónde soltarse        |
| Lanzar el hilo              | Anillo sobre el objetivo; el hilo sale disparado y vibra       | Chasquido con chispa   | Balanceo o arrastre                     |
| Lanzar el hilo sin objetivo | Círculo que muestra el alcance; el anillo no se gasta          | Aviso apagado          | No se gasta ningún uso                  |
| Escribir una estrella       | Vista previa de la mira (azul válida, roja inválida); destello | Campanilla suave       | Aparece un anclaje temporal             |
| Morir                       | Efecto de destrucción                                          | Chasquido de engranaje | Reaparece en 0.4 s al inicio de la sala |
| Cambiar de sala             | Transición de cámara de 0.5 s sin pausar el juego              | El ambiente se funde   | Nuevo punto de reaparición              |
| Obtener un fragmento        | El Astrolabio brilla más                                       | Acorde cálido          | Avanza la restauración de la Casa       |

## Fricción intencional

¿Qué dificultad forma parte del diseño y qué dificultad es simplemente mala experiencia de usuario?

**Dificultad intencional (parte del diseño):**
- Saltos de precisión, calcular el balanceo y gestionar los usos y la cuerda.
- Morir muchas veces: un toque mata.
- Combinar escalar, poner un punto de apoyo  y lanzarse sin tocar el suelo.

**Fricción que se debe evitar (mala experiencia):**
- Controles que no responden como el jugador pretendía: por eso hay *coyote time*, memoria de pulsación y ayuda de puntería.
- Muertes que el jugador no entiende: los peligros se ven y siempre se muere por un error propio.
- Castigos largos: no hay vidas, la reaparición es inmediata y los checkpoints evitan repetir tramos extensos.
- Límites de sala que cortan un balanceo.
- Instrucciones escondidas o texto que interrumpe la acción.

## Descubrimiento

¿Cómo sabe el jugador:

- **Qué hacer?** Efeméride presenta el objetivo (reunir los fragmentos y restaurar la Casa) y cada sala presenta una idea nueva.
- **Dónde ir?** La cámara muestra la sala completa; la luz cálida y los faroles marcan el camino; en algunos puntos la cámara viaja para enseñar lo que viene.
- **Qué puede interactuar?** Poemas y asientos de observatorio.
- **Qué ocurrió?** Cada acción tiene una señal visual y una sonora propias (ver la tabla de retroalimentación).
- **Por qué ganó o perdió?** Al morir se ve el peligro que mató al personaje y se reaparece de inmediato para reintentar; no existe una pantalla de derrota.


> **Navegación:** [[00 - Índice]] · ← [[05 - Audio y Música]] · [[02 - UI y Menús]] →
