# Mecánicas

## Descripción de la sección

Una mecánica es una regla o interacción mediante la cual el jugador puede actuar dentro del sistema del juego.

Documenta cada mecánica con suficiente detalle para que otro integrante pueda implementarla.

## Plantilla de mecánica

### Nombre de la mecánica

**Propósito:**  
¿Qué aporta a la experiencia?

**Activación:**  
¿Qué debe hacer el jugador?

**Reglas:**  
¿Qué puede y qué no puede ocurrir?

**Entrada:**  
¿Qué botón, gesto o acción la activa?

**Estado inicial:**

**Estado final:**

**Recursos utilizados:**

**Recompensa:**

**Penalización:**

**Interacciones con otras mecánicas:**

**Casos límite:**  
¿Qué ocurre en situaciones poco comunes?

## Mecánicas principales

### Mecánica 01
### Gancho (Grappling hook)

**Propósito:**  
Dar al jugador movilidad rápida y fluida: cruzar abismos, alcanzar zonas altas y encadenar movimientos que el salto no permite. Es la mecánica principal; un jugador hábil recorre tramos enteros sin tocar el suelo.

**Activación:**  
El jugador apunta con el puntero y pulsa el botón del modo que quiere. Se activa si hay un objetivo enganchable dentro del alcance y queda al menos un uso.

Objetivos válidos:
- Bloques sólidos enganchables (también se pueden pisar y escalar).
- Anclajes aéreos, que se atraviesan: los fijos del nivel y los que escribe el jugador.
- Plataformas móviles enganchables.

**Reglas:**  
- Dos modos con los mismos 2 usos compartidos. Un uso solo se gasta si el gancho engancha; los usos se recargan al tocar suelo firme (o con un cristal de recarga).
- **Balanceo:** funciona como un péndulo. Dura hasta que el jugador lo corta. Con los pies en el suelo la cuerda es solo una correa: se camina y se salta con normalidad.
- **Arrastre:** línea recta hacia el punto. Al llegar al objetivo, o si algo lo bloquea, el gancho se suelta solo y conserva parte de la velocidad. Nunca queda anclado.
- La cuerda del balanceo choca con los sólidos: se dobla en las esquinas y el jugador se balancea desde la esquina con la cuerda que le queda. Al volver, se desdobla.
- Pulsar de nuevo el botón del modo en uso corta el gancho.
- Mientras está enganchado no se puede agarrar una pared; con Shift mantenido el jugador se agarra al llegar o al cortar.

**Entrada:**  
Clic izquierdo: balanceo. Clic derecho: arrastre. Con mando: RT (mantener) para el balanceo y RB para el arrastre; se apunta con el stick derecho.

**Estado inicial:**  
El personaje está en el suelo, en el aire o en una pared, con al menos un uso disponible y un objetivo dentro del alcance.

**Estado final:**
- Balanceo cortado: el personaje queda en el aire con toda la velocidad acumulada.
- Arrastre terminado: el personaje llega al objetivo o se suelta con velocidad.
- Si el objetivo desaparece, el gancho se suelta y el personaje cae con su velocidad actual.

**Recursos utilizados:**  
Un uso de los 2 disponibles por cada enganche logrado.

**Recompensa:**
- Acceso a zonas que el salto no alcanza.
- Rutas más rápidas.
- Sensación de fluidez al encadenar balanceos.

**Penalización:**
- Calcular mal el balanceo o soltar a destiempo provoca una caída al vacío o contra un peligro.
- Gastar los 2 usos en el aire deja al jugador sin opciones hasta tocar suelo (o un cristal).

**Interacciones con otras mecánicas:**
- Salto: se puede lanzar el gancho durante el salto; al soltarse, el impulso se suma al movimiento.
- Escalada: se puede lanzar el gancho desde la pared (suelta la pared). Es la combinación central del diseño avanzado: escalar, escribir un anclaje y lanzarse.
- Anclaje: el anclaje del jugador es uno de los objetivos del gancho.
- Plataformas móviles: el punto de enganche sigue al objeto enganchado. Enganchar una plataforma cuenta como subirse a ella; la plataforma zip sale disparada y arrastra al jugador por la cuerda.
- Cristal de recarga: devuelve un uso.

**Casos límite:**  
- El jugador muere enganchado: el gancho se libera de inmediato.
- Algo bloquea el arrastre: el gancho se suelta.
- El anclaje que se estaba usando desaparece: el gancho se libera automáticamente.
- La cuerda del balanceo se corta sola tras unos segundos.

### Mecánica 02
### Punto de anclaje (Grapple point)

**Propósito:**  
Permitir que el jugador cree su propio camino: el Astrolabio ponga una estrella diminuta en el vacío que sirve de punto de enganche.

**Activación:**  
El jugador apunta a una posición y pulsa la entrada. Se coloca el anclaje si queda el uso del anclaje (ver la espera de recarga en Reglas).

**Reglas:**  
- Alcance de colocación: Si el puntero está más lejos del rango permitido, el anclaje se coloca en el límite del alcance en esa dirección. Si hay una pared en medio, se coloca delante de ella.
- Un uso por vez. Solo puede existir un anclaje a la vez; colocar uno nuevo borra el anterior.
- Se puede colocar en el aire o sobre superficies, y puede engancharse con el gancho.
- Dura unos segundos si no se usa, para no abusar de la habilidad.
- Una vez usado, desaparece cuando el gancho lo suelta o a los pocos segundos de estar enganchado ya que el punto de anclaje no dura mucho.
- El uso se recarga al tocar suelo: al instante si el anclaje se usó (el gancho se enganchó a él) y, si no se usó. El cristal de recarga lo devuelve sin espera.
- Mientras el jugador apunta se muestra una vista previa de dónde quedará el anclaje.

**Entrada:**  
Tecla E. Con mando: LB.

**Estado inicial:**  
El personaje está en el suelo, en el aire o en una pared, con el uso del anclaje disponible.

**Estado final:**  
Existe una estrella-anclaje en el mundo. Si no se usa, desaparece a los ; si pocos segundos se usa, desaparece según se describe arriba.

**Recursos utilizados:**  
El uso del anclaje (1).

**Recompensa:**
- Rutas que el nivel no ofrece.
- La libertad de resolver la misma sala de más de una manera.

**Penalización:**
- Colocar el anclaje mal, obliga a esperar la recarga.
- El anclaje caduca si se tarda demasiado en usarlo.

**Interacciones con otras mecánicas:**
- Gancho: el anclaje es un objetivo del gancho.
- Escalada: E no depende del estado, así que se puede colocar desde la pared.
- Cristal de recarga: devuelve el uso sin esperar a tocar el piso.
- Casa de Géminis: dentro de un espejo, cada estrella escrita tiene una gemela al otro lado de la línea, que también se puede enganchar.
- Casa de Acuario: un anclaje dentro de una corriente deriva con ella.

**Casos límite:**  
- Reaparecer borra el anclaje.
- Si el anclaje desaparece estando enganchado, el gancho se libera.


### Mecánica 03
### Agarre y escalada

**Propósito:**  
Subir por paredes rugosas y combinar la escalada con el anclaje y el gancho. La cuerda limitada obliga a planear y a decidir cuánto subir.

**Activación:**  
El jugador mantiene el botón de agarre junto a una pared rugosa.

**Reglas:**  
- Solo se agarran superficies rugosas. Las superficies lisas no dan agarre y se distinguen a simple vista; en ellas el jugador solo se desliza y puede saltar de la pared.
- Tienes estamina: se gasta al estar colgado y al estar subiendo.
- La estamina se recarga al tocar suelo.
- Un salto desde la pared (climb jump) cuesta estamina.
- Mientras el gancho está enganchado no se puede agarrar.

**Entrada:**  
Shift izquierdo (mantener).

**Estado inicial:**  
El personaje está junto a una pared rugosa con estamina disponible.

**Estado final:**  
Colgado o subiendo, hasta que se suelta, se agota la estamina o se salta.

**Recursos utilizados:**  
Estamina de escalada.

**Recompensa:**  
Altura y acceso a zonas verticales.

**Penalización:**  
Al agotarse la cuerda, el jugador cae.

**Interacciones con otras mecánicas:**
- Anclaje y gancho: se coloca un anclaje y se lanza el gancho desde la pared.
- Casa de Acuario: los muros mojados gastan el doble de estamina y resbalan.
- Casa de Géminis: el muro espejo es pulido (sin agarre ni salto de pared) y devuelve el impulso de quien llega con velocidad.

**Casos límite:**  
- Pararse encima de una superficie rugosa cuenta como suelo y recarga.
- Con Shift mantenido, el jugador se agarra al llegar a la pared tras un gancho.

## Mecánicas secundarias

### Mecánica 04
### Movimiento y salto

**Propósito:** Movimiento de precisión con control justo y predecible.  
**Reglas:**
- Carrera horizontal con aceleración y desaceleración.
- Salto variable: la altura depende de cuánto se mantiene el botón. Incluye coyote time, jump buffer y caída más pesada.
- En el aire el jugador conserva la velocidad que supere la de carrera (inercia del gancho, del salto de pared o de las plataformas).
- Deslizamiento y salto de pared en superficies lisas.

**Entrada:** A/D o W/A/S/D para mover; Espacio para saltar. Con mando: stick izquierdo o cruceta, y A.  
**Casos límite:** las paredes no cuentan como suelo; el jugador hereda la velocidad de la plataforma que pisa o agarra (hasta 0.15 s después de que frene).

### Mecánica 05
### Cristal de recarga

**Propósito:** Devolver recursos en el aire para encadenar movimientos.  
**Reglas:** devuelve 1 uso de gancho y 1 de anclaje; solo se consume si falta alguno; reaparece a los 2 segundos.  
**Interacciones:** gancho, anclaje.

### Mecánica 06
### Plataformas móviles

**Propósito:** Añadir movimiento al nivel y a la ruta del jugador.  
**Reglas:**
- Tipos: patrulla (ida y vuelta constante; un muro cuenta como final del recorrido) y zip (se activa al pisarla, agarrarla o engancharla; va rápido y vuelve lento).
- La capa de la plataforma decide si solo se pisa, además se agarra, o además se engancha.
- El jugador hereda su velocidad al saltar, hacia arriba y de lado.
- No atraviesan sólidos ni otras plataformas: se detienen y dan la vuelta. Vuelven a su inicio cuando el jugador reaparece.
- Además hay rejillas (se atraviesan desde abajo), losas que tiemblan y se rompen al pisarlas y elevadores (montacargas) que llevan al jugador mientras habla Efeméride.


### Mecánica 07
### Peligros, salas, muerte y reaparición

**Propósito:** Castigo justo y reintento inmediato.  
**Reglas:**
- Cualquier peligro (pinchos, vacío) o un aplastamiento mata. Un toque basta; no hay vidas ni salud.
- Al instante el jugador reaparece en su punto de aparición con todo recargado, y el nivel se reinicia (plataformas a su inicio, cristales disponibles, anclaje borrado).
- Cada sala tiene su cámara; al entrar en otra, la cámara cambia con una transición de  y el punto de reaparición pasa a ser el más cercano a la entrada. El juego no se pausa durante la transición.
- Los checkpoints son opcionales y van dentro de salas largas: al tocarlos pasan a ser el punto de reaparición hasta que se entra en otra sala.
- El progreso se guarda al descansar en un observatorio mayor y al tomar el ascensor entre Casas.

### Mecánica 08
### Habilidades narrativas

**Propósito:** Acciones con las que el Almanaque descubre la historia. No tienen reto, pero cada una tiene una señal visual propia.

| Habilidad                  | Qué hace                                                                                  |
| -------------------------- | ----------------------------------------------------------------------------------------- |
| Observar                   | Se detiene frente a hologramas y telescopios para ver el mundo; lo que ve cambia según la Casa. |
| Recolectar fragmentos      | Objetivo principal; cada fragmento se guarda en el Astrolabio, que brilla más con cada uno. |
| Leer notas del Almanaque XI | Solo en los observatorios mayores.                                                        |
| Descansar                  | En un observatorio mayor se sienta, da cuerda a su llave y guarda el progreso.             |

Interactuar: W (o flecha arriba) en teclado e Y en mando; el equipo debe confirmar la tecla.

> **Navegación:** [[00 - Índice]] · ← [[01 - Jugabilidad]] · [[03 - Sistemas]] →
