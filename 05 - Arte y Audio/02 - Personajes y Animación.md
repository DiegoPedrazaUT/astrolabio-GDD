# Personajes y animación

| Personaje               | Sprite                                                                           | Animaciones                                               | VFX                                                      | Estado                                                 |
| ----------------------- | -------------------------------------------------------------------------------- | --------------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------ |
| Almanaque XII (jugador) | 32×32 px, paleta SLSO8: autómata de latón con capa de mapas estelares            | Movimiento, interacción, muerte y reaparición (ver abajo) | Polvo, chispas del gancho, destello de la estrella ancla | Arte integrado en el juego                             |
| Efeméride               | Holograma dorado y blanco cálido con parpadeo                                    | Aparecer, hablar, parpadear al perder la calma, apagarse  | Brillo y líneas de proyección                            | Sprites de reposo y habla dibujados; sin integrar      |

El diseño completo del Almanaque XII está en [[03 - Personajes]].

**Animaciones del Almanaque:**
- *Movimiento:* quieto, correr, saltar, caer, aterrizar (con aplastar y estirar), deslizar por la pared, colgar, escalar, balancearse con el gancho y ser arrastrado por el gancho.
- *Interacción:* despertar y dormir (inicio del juego), mirar hacia arriba (el cielo del Pozo Celeste), dar cuerda a la llave al estar quieto y recibir un objeto (poema o fragmento de estrella).
- *Muerte:* efecto breve de destrucción y regreso al punto de reaparición (0,4 s); no hay pantalla de derrota.
- *Capa:* una línea que sigue al cuerpo con retraso; ondea al saltar y al balancearse y es el elemento más reconocible.

**Convenciones:** sprites dibujados en Aseprite y exportados a PNG, sin compresión y con filtro de píxel (*Point*). El personaje mide 32×32 px y se muestra al doble (unos 2 tiles de alto); se dibuja mirando a la derecha y se voltea, con el pivote en los pies. La animación muestra la velocidad propia del personaje, no la que le suma una plataforma. Los archivos van en minúsculas, sin espacios, con el nombre del personaje y de la animación (por ejemplo, `almanaque_run`).

> **Navegación:** [[00 - Índice]] · ← [[01 - Dirección de Arte]] · [[03 - Entornos]] →
