# Mecánicas

## Mecánicas principales

### Gancho de luz

**Propósito:** movilidad rápida y fluida: cruzar abismos, alcanzar zonas altas y encadenar movimientos que el salto no permite. Es la mecánica central; un jugador hábil recorre tramos enteros sin tocar el suelo.

**Cómo funciona:** el jugador apunta con el puntero y pulsa el botón del modo que quiere. Se lanza si hay un objetivo enganchable dentro del alcance y queda al menos un uso.

- **Objetivos válidos:** bloques sólidos enganchables (también se pisan y se escalan), estrellas ancla aéreas (las fijas del nivel y las que escribe el jugador, que se atraviesan). Las plataformas móviles no se enganchan.
- **Usos:** dos modos comparten 2 usos. Un uso solo se gasta si el gancho engancha. Se recargan al tocar suelo firme o con un cristal de recarga.
- **Balanceo:** funciona como péndulo y dura hasta que el jugador lo corta o hasta que se acaba su tiempo límite de uso (unos segundos), lo que ocurra primero. Con los pies en el suelo la cuerda es solo una correa: se camina y se salta con normalidad.
- **Arrastre:** línea recta hacia el punto. Al llegar, o si algo lo bloquea, el gancho se suelta y conserva parte de la velocidad. Nunca queda anclado.
- **Cuerda y sólidos:** la cuerda del balanceo se dobla en las esquinas y el jugador se balancea desde la esquina con la cuerda que le queda. Al volver, se desdobla.
- **Cortar:** el jugador suelta el gancho según el modo de control elegido en Configuración › Jugabilidad: soltar el botón (predeterminado), pulsar de nuevo el botón o pulsar Saltar. Si no lo corta, la cuerda del balanceo se corta sola al llegar a su tiempo límite.
- **Nebulosa:** si el gancho cruza una nebulosa se corta; al apuntar, la línea se pone roja y el disparo se detiene en ella.
- **Agarre:** mientras está enganchado no se puede agarrar una pared; con Shift mantenido el jugador se agarra al llegar o al cortar.

**Entrada:** clic izquierdo para el balanceo y clic derecho para el arrastre. Con mando, RT (mantener) para el balanceo y RB para el arrastre; se apunta con el joystick derecho. Con la opción de Configuración › Jugabilidad se puede elegir otro modo para soltar el gancho.

**Riesgo y recompensa:** calcular mal el balanceo o soltar a destiempo lleva a una caída o a un peligro, y gastar los 2 usos en el aire deja al jugador sin opciones hasta tocar suelo. A cambio, el gancho da acceso a zonas que el salto no alcanza y rutas más rápidas.

**Combina con:**
- *Salto:* se puede lanzar durante el salto; al soltarse, el impulso se suma al movimiento.
- *Escalada:* se lanza desde la pared (suelta la pared). Es la combinación central del diseño avanzado: escalar, escribir una estrella ancla y lanzarse.
- *Estrella ancla:* la que escribe el jugador es uno de sus objetivos.
- *Cristal de recarga:* devuelve un uso.

**Casos límite:** si el jugador muere enganchado, o si la estrella ancla o el objetivo desaparecen, el gancho se libera de inmediato. Si algo bloquea el arrastre, se suelta. La nebulosa también lo corta.

### Estrella ancla

**Propósito:** que el jugador cree su propio camino: el Astrolabio pone una estrella diminuta en el vacío que sirve de punto de enganche.

**Cómo funciona:** el jugador apunta a una posición y pulsa la entrada. Mientras apunta se muestra una vista previa de dónde quedará.

- **Alcance:** si el puntero está más lejos del rango permitido, la estrella se coloca en el límite del alcance en esa dirección. Si hay una pared en medio, se coloca delante de ella.
- **Una a la vez:** solo existe una estrella ancla; colocar otra borra la anterior. Se puede colocar en el aire o sobre superficies.
- **Duración:** desaparece a los pocos segundos si no se usa, y también a los pocos segundos de estar enganchado o cuando el gancho la suelta.
- **Recarga:** la estrella ancla vuelve a estar disponible al tocar suelo. Si se usó (el gancho se enganchó a ella), la recarga es inmediata. Si no se usó, hay que esperar unos segundos desde que se colocó, para que no se abuse de la habilidad. El cristal de recarga la devuelve sin esperar.

**Entrada:** tecla E. Con mando, LB. No depende del estado del personaje, así que se puede colocar también desde la pared.

**Riesgo y recompensa:** colocarla mal obliga a esperar la recarga y tardar en usarla la hace caducar. A cambio, abre rutas que el nivel no ofrece y permite resolver una misma sala de más de una manera.

**Casos límite:** reaparecer borra la estrella ancla; si desaparece estando enganchado, el gancho se libera.

### Agarre y escalada

**Propósito:** subir por paredes rugosas y combinar la escalada con la estrella ancla y el gancho. La cuerda limitada obliga a planear y a decidir cuánto subir.

**Cómo funciona:** el jugador mantiene el botón de agarre junto a una pared rugosa.

- **Superficies:** solo se agarran las rugosas. Las lisas se distinguen a simple vista; en ellas el jugador solo se desliza y puede saltar de la pared.
- **Cuerda de escalada:** tiene 100 puntos. Se gastan 20 por segundo al estar colgado, 33 por segundo al subir y 25 por cada salto desde la pared. Se recarga al tocar suelo; al agotarse, el jugador cae.
- **Gancho:** mientras está enganchado no se puede agarrar.

**Entrada:** Shift izquierdo (mantener).

**Combina con:** estrella ancla y gancho, que se lanzan desde la pared. Pararse encima de una superficie rugosa cuenta como suelo y recarga; con Shift mantenido el jugador se agarra al llegar a la pared tras un gancho.

## Mecánicas secundarias

### Movimiento y salto

Movimiento de precisión con control justo y predecible.

- Carrera horizontal con aceleración y desaceleración.
- Salto variable: la altura depende de cuánto se mantiene el botón. Incluye coyote time, jump buffer y caída más pesada.
- En el aire el jugador conserva la velocidad que supere la de carrera (inercia del gancho, del salto de pared o de las plataformas).
- Deslizamiento y salto de pared en superficies lisas. Las paredes no cuentan como suelo.
- El jugador hereda la velocidad de la plataforma que pisa o agarra (hasta 0.15 s después de que frene).

**Entrada:** A/D o W/A/S/D para mover y Espacio para saltar. Con mando, stick izquierdo o cruceta, y A.

### Cristal de recarga

Devuelve recursos en el aire para encadenar movimientos: 1 uso de gancho, 1 de estrella ancla y la cuerda de escalada. Solo se consume si falta alguno y reaparece a los 2 segundos.

### Plataformas móviles

Añaden movimiento al nivel y a la ruta del jugador.

- **Patrulla:** ida y vuelta constante; un muro cuenta como final del recorrido.
- **Zip:** se activa al pisarla o agarrarla; va rápido y vuelve lento.
- La capa de la plataforma decide si solo se pisa o además se agarra. No se enganchan.
- El jugador hereda su velocidad al saltar, hacia arriba y de lado.
- No atraviesan sólidos ni otras plataformas: se detienen y dan la vuelta. Vuelven a su inicio cuando el jugador reaparece.
- También hay rejillas (se atraviesan desde abajo), losas que tiemblan y se rompen al pisarlas, y elevadores que llevan al jugador mientras habla Efeméride.

### Peligros, salas, muerte y reaparición

Castigo justo y reintento inmediato.

- Cualquier peligro (engranajes, sierras, nebulosa, vacío) o un aplastamiento mata. Un toque basta; no hay vidas ni salud.
- El jugador reaparece al instante en su punto de aparición con todo recargado, y la sala se reinicia (plataformas a su inicio, cristales disponibles, estrella ancla borrada).
- Cada sala tiene su cámara; al entrar en otra, la cámara cambia con una transición de medio segundo y el punto de reaparición pasa a ser el más cercano a la entrada. El juego no se pausa durante la transición.
- Los checkpoints son opcionales y van dentro de salas largas: al tocarlos pasan a ser el punto de reaparición hasta que se entra en otra sala.
- El progreso se guarda solo al entrar en una sala, al tomar un checkpoint y al recibir una habilidad (ver [[04 - Guardado y Configuración]]).

### Habilidades narrativas

Acciones con las que el Almanaque descubre la historia. No tienen reto, pero cada una tiene una señal visual propia.

| Habilidad             | Qué hace                                                                                      |
| --------------------- | --------------------------------------------------------------------------------------------- |
| Recolectar fragmentos | Objetivo principal; cada fragmento se guarda en el Astrolabio, que brilla más con cada uno.   |
| Leer                  | Al recoger un poema se abre un panel con su texto; se cierra con Aceptar. |

**Entrada:** Aceptar (Espacio o A) cierra el panel del poema.

> **Navegación:** [[00 - Índice]] · ← [[01 - Jugabilidad]] · [[03 - Sistemas]] →
