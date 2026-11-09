# Niveles

## Descripción de la sección

Cada nivel debe documentar su propósito jugable, estructura, dificultad, contenido y condiciones de entrada/salida.

## Plantilla de nivel

### Nombre del nivel

**Objetivo principal:**

**Objetivos secundarios:**

**Duración estimada:**

**Dificultad:**

**Mecánicas introducidas:**

**Mecánicas utilizadas:**

**Enemigos / obstáculos:**

**Recompensas:**

**Puntos de guardado:**

**Condición de entrada:**

**Condición de salida:**

**Eventos narrativos:**

**Mapa / diagrama:**

## Niveles del juego

### Nivel 1 — Las Entrañas del Reloj (tutorial)

**Objetivo principal:** Llegar al Pozo Celeste y obtener el primer fragmento de estrella.

**Objetivos secundarios:** Encontrar el poema escondido en la Galería de Engranajes.

**Duración estimada:** Entre 5 y 8 minutos para un jugador con experiencia en el género; para un jugador nuevo, unos 15 minutos.

**Dificultad:** Baja, como corresponde a un tutorial. Cada idea nueva se presenta primero en un espacio seguro y después se pone a prueba con riesgo. El Puente Roto es el primer gran desafío del gancho y el Pozo de Cadenas, el examen vertical de lo aprendido.

**Mecánicas introducidas:** moverse y saltar; agarrarse y escalar con cuerda limitada; plataformas (patrulla, zip, rejillas y losas que se rompen); gancho (balanceo y arrastre) y cristal de recarga; anclaje; la combinación de escalar, anclar y lanzarse.

**Mecánicas utilizadas:** las cuatro habilidades.

**Enemigos / obstáculos:** engranajes giratorios, sierras en las paredes, gas nebuloso y vacío letal.

**Recompensas:** primer fragmento de estrella; el Astrolabio brilla; el poema escondido.

**Puntos de guardado:** checkpoints en las salas largas. La demo todavía no guarda el progreso (ver [[04 - Guardado y Configuración]]).

**Condición de entrada:** despertar en el nicho XII.

**Condición de salida:** obtener el primer fragmento de estrella y tomar el elevador hacia el Eje Central.

**Eventos narrativos:** introducción de Efeméride, indicaciones en tres zonas, cierre en el Pozo Celeste con el cielo y sus huecos (ver [[04 - Diálogos y Narrativa]]).

**Zonas:**

| Zona                     | Qué se aprende                                                                                     | Salas                         | Peligros        |
| ------------------------ | -------------------------------------------------------------------------------------------------- | ----------------------------- | --------------- |
| La Sala de los Nichos    | Moverse y saltar; se presentan los nichos y habla Efeméride                                                | 1 sala                        | —               |
| La Galería de Engranajes | Saltar con hueco, agarrarse y escalar; la cuerda se agota; plataformas, rejillas y losas           | 9 salas (con un elevador de un solo sentido) | Engranajes y sierras |
| El Puente Roto           | Se entrega el gancho: arrastre, balanceo y faroles; cristal de recarga                             | 3 salas                       | Vacío, sierras y gas |
| El Pozo de Cadenas       | Examen vertical: escalar, lanzarse desde la pared y recargar al tocar suelo; sin anclaje           | 4 salas                       | Engranajes y sierras |
| El Pozo Celeste          | Se entrega el anclaje; escribir y usar la estrella sobre el vacío; primer fragmento | 1 sala y el elevador al Eje Central | Vacío     |

**Mapa / diagrama:** el reparto de las 18 salas por zonas es provisional; el mapa se incorporará cuando el equipo lo confirme.

### Nivel 2 — El Eje Central (cierre de la demo)

**Objetivo principal:** Llegar a la sala del Eje Central y cruzar las puertas de Géminis, con lo que termina la demo.

**Duración estimada:** Breve; no es un nivel de plataformas, sino la sala de llegada. En el juego completo será la sala desde la que el jugador elija el siguiente nivel.

**Mecánicas utilizadas:** ninguna nueva; el jugador camina.

**Enemigos / obstáculos:** ninguno.

**Condición de entrada:** subir en el elevador del Pozo Celeste.

**Condición de salida:** cruzar las puertas de Géminis (fin de la demo).

**Eventos narrativos:** llegada del elevador, vista del Gran Reloj con las doce Casas y Géminis señalada; el Almanaque mira las puertas una última vez y las cruza (ver [[01 - Premisa y Trama]]).

### Fuera de la demo

La Casa de Géminis, las demás Casas y el desenlace están previstos para el juego completo y no forman parte de esta entrega (ver [[01 - Alcance]]).

## Flujo del nivel

```text
Inicio → Zona A → Desafío → Zona B → Recompensa → Final
```

**Flujo de una Casa (juego completo):**

```text
Ascensor → Zona de presentación (segura) → Zonas de reto → Último tramo → Cámara (entrega de fragmentos) → Ascensor
```

## Criterios de calidad

- El objetivo es comprensible.
- Las reglas se pueden aprender.
- El desafío corresponde al nivel de progresión.
- Existe retroalimentación suficiente.
- El jugador entiende por qué tuvo éxito o fracaso.
- Cada sala presenta una idea nueva antes de ponerla a prueba con riesgo.
- Los saltos tienen una ventana de entrada justa (por ejemplo, un hueco de 3 unidades deja un margen cómodo y uno de 5 unidades en subida es injusto).
- Hay un checkpoint o una repisa cada 15 a 20 unidades en tramos verticales.
- Los límites de una sala no cortan un balanceo.

> **Navegación:** [[00 - Índice]] · ← [[01 - Estructura del Contenido]] · [[03 - Enemigos y NPC]] →
