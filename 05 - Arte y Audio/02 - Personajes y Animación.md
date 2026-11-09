# Personajes y Animación

## Requisitos por personaje

| Personaje                     | Modelo/Sprite                                                                   | Animaciones                                               | VFX                                           | Estado        |
| ----------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------- | ------------- |
| Almanaque XII (jugador)       | Sprite de 32×32 px, paleta SLSO8: autómata de latón con capa de mapas estelares | Movimiento, interacción, muerte y reaparición (ver abajo) | Polvo, chispas del gancho, destello de la estrella ancla | Arte integrado en el juego |
| Efeméride                     | Holograma dorado y blanco cálido con parpadeo                                   | Aparecer, hablar, parpadear al perder la calma, apagarse  | Brillo y líneas de proyección                 | Sprites de reposo y habla dibujados; sin integrar en el juego |

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
- Balancearse con el gancho
- Ser arrastrado por el gancho

### Interacción

- Despertar y dormir (inicio del juego)
- Mirar hacia arriba (el cielo del Pozo Celeste)
- Dar cuerda a la llave (al estar quieto)
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
- Tamaño del personaje: 32×32 px, mostrado al doble de tamaño (unos 2 tiles de alto); tiles: 32×32 px, pintados con *Rule Tiles*.
- El personaje se dibuja mirando a la derecha y se voltea para mirar a la izquierda.
- El pivote del sprite queda en los pies.
- La animación debe mostrar la velocidad propia del personaje, no la que le suma una plataforma: sobre una cinta o plataforma se ve quieto, no «caminando».
- Nombres de archivo en minúsculas, sin espacios, con el nombre del personaje y de la animación (por ejemplo, `almanaque_run`).

> **Navegación:** [[00 - Índice]] · ← [[01 - Dirección de Arte]] · [[03 - Entornos]] →
