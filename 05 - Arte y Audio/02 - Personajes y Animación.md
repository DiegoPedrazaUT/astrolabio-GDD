# Personajes y Animación

## Descripción de la sección

Documenta cómo deben verse y comportarse visualmente los personajes.

## Requisitos por personaje

| Personaje                     | Modelo/Sprite                                                                   | Animaciones                                               | VFX                                           | Estado        |
| ----------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------- | ------------- |
| Almanaque XII (jugador)       | Sprite de 32×32 px, paleta SLSO8: autómata de latón con capa de mapas estelares | Movimiento, interacción, muerte y reaparición (ver abajo) | Polvo, chispas del hilo, destello del anclaje | Arte definido |
| Efeméride                     | Holograma dorado y blanco cálido con parpadeo                                   | Aparecer, hablar, parpadear al perder la calma, apagarse  | Brillo y líneas de proyección                 | Por producir  |
| Reflejo del jugador (Géminis) | Copia del Almanaque, boca abajo cuando el espejo está tumbado                   | Reutiliza las del Almanaque                               | Brillo del espejo                             | Por producir  |
| Almanaque XI                  | Cuerpo inmóvil sentado en el Observatorio de Ofiuco (versión completa)          | Ninguna                                                   | Ninguno                                       | Por producir  |

El diseño completo del Almanaque XII (cuerpo, cabeza, capa, llave de cuerda y Astrolabio) está en [[03 - Personajes]].

## Animaciones

### Movimiento

- Idle (quieto)
- Correr
- Saltar
- Caer
- Aterrizar (con aplastar y estirar, *squash & stretch*)
- Deslizar por la pared
- Colgar de la pared
- Escalar
- Balancearse con el hilo
- Ser arrastrado por el hilo

### Interacción

- Despertar y dormir (inicio del juego)
- Mirar hacia arriba (hologramas y telescopios)
- Inclinar la cabeza (ante un holograma)
- Sentarse y dar cuerda a la llave (observatorio)
- Recibir un objeto (poema o fragmento de estrella)

### Combate

No aplica: el juego no tiene combate.

### Daño

No aplica: no hay salud. Un toque de peligro destruye al personaje de inmediato.

### Muerte / derrota

Efecto breve de destrucción y de regreso al punto de reaparición (0.4 s). No hay pantalla de derrota.

### Capa

La capa es una línea que sigue al cuerpo con retraso: ondea al saltar y al balancearse y es el elemento más reconocible del personaje.

## Convenciones

- Sprites dibujados en Aseprite y exportados a PNG, sin compresión y con filtro de píxel (*Point*).
- Tamaño del personaje: 32×32 px; tiles: 16×16 px.
- El personaje se dibuja mirando a la derecha y se voltea para mirar a la izquierda.
- El pivote del sprite queda en los pies.
- La animación debe mostrar la velocidad propia del personaje, no la que le suma una plataforma o una corriente: sobre una cinta o plataforma se ve quieto, no «caminando».
- Nombres de archivo en minúsculas, sin espacios, con el nombre del personaje y de la animación (por ejemplo, `almanaque_run`).


> **Navegación:** [[00 - Índice]] · ← [[01 - Dirección de Arte]] · [[03 - Entornos]] →
