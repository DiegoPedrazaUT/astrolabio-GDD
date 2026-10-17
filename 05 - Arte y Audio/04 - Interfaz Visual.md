# Interfaz Visual

## Descripción de la sección

Documenta la información que el juego muestra al jugador y las reglas visuales de la interfaz.

## HUD

El HUD es mínimo y forma parte del mundo: se apoya en el propio Astrolabio del personaje.

Elementos:

- **Vida:** no aplica (no hay salud).
- **Energía / Recursos:** anillos del Astrolabio para los usos del gancho y del anclaje; una llave que gira para la cuerda de escalada.
- **Munición:** no aplica.
- **Objetivo:** no hay indicador en pantalla; el objetivo se cuenta con Efeméride y con el escenario.
- **Mapa:** no hay; cada sala se ve completa con su cámara.
- **Indicadores contextuales:** anillo sobre el farol o bloque al que se enganchará el hilo, vista previa del anclaje y carteles de controles dentro del escenario.

El HUD se oculta cuando el jugador no tiene el control (conversaciones y cinemáticas).

## Jerarquía visual

¿Qué información debe verse primero, segundo y tercero?

1. El personaje y los peligros inmediatos.
2. Los objetivos enganchables, las superficies y el camino.
3. Los recursos (anillos y llave del Astrolabio).
4. El texto de Efeméride, que no compite con la acción porque solo aparece en pausas.

## Estados

- **Normal:** anillos encendidos según los usos disponibles.
- **Uso gastado:** el anillo se apaga.
- **Advertencia:** la llave tiembla y suena un clic acelerado cuando la cuerda está por agotarse; la cuerda del balanceo se pone roja en los últimos 2 s.
- **Éxito:** destello al escribir una estrella y brillo del Astrolabio al guardar un fragmento.
- **Error:** la mira del anclaje se pone roja si la posición no es válida.
- **Bloqueo:** durante una conversación o cinemática no hay control y el HUD se oculta.
- **Muerte:** efecto breve de destrucción y reaparición; no hay pantalla de derrota.

## Convenciones

**Tipografía:**
Fuente de píxeles propia, legible a 640×360 px. Texto blanco cálido (`#ffecd6`) sobre un marco dorado tenue; cada hablante tiene su propio color de apoyo.

**Iconografía:**
Las teclas y los botones se dibujan al estilo de los carteles pintados en el escenario. Los iconos cambian solos según el último dispositivo usado (teclado o mando); si dos teclas hacen lo mismo en el mando, se dibuja una sola.

**Tamaños mínimos:**
El texto debe leerse a la resolución base (640×360 px, escala ×3 en 1080p).

**Contraste:**
Texto claro sobre fondo oscuro; la información jugable nunca se apoya solo en el color.

**Animaciones:**
El texto aparece letra a letra, con etiquetas para pausas, ondas y temblor. Las transiciones usan fundidos breves.

## Pantallas

- Menú principal
- Pausa
- Configuración
- Selector de Casa (un dial de reloj en el Pozo Celeste, con las doce Casas)
- Créditos
- Tarjeta final (estadísticas de la partida)

No existen Inventario, Mapa, Victoria ni Derrota.

El flujo y la estructura de las pantallas se detallan en [[02 - UI y Menús]].


> **Navegación:** [[00 - Índice]] · ← [[03 - Entornos]] · [[05 - Audio y Música]] →
