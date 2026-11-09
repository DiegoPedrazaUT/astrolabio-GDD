# Interfaz Visual

## HUD

El HUD es mínimo.

> [!info] Estado en el juego
> El HUD implementado (UI Toolkit, panel de 1280 × 720) muestra el gancho y la estrella ancla con sus usos y su botón, **solo cuando el jugador ya tiene la habilidad**; el nombre de la zona durante 3 s al entrar en una zona nueva; y las pistas de Pausa y Saltar. Se oculta en la pausa y bajo el velo del elevador. El diseño de anillos y llave del Astrolabio de abajo es la propuesta original: la cuerda de escalada aún no tiene indicador en el HUD.

Elementos:

- **Vida:** no aplica (no hay salud).
- **Energía / Recursos:** anillos del Astrolabio para los usos del gancho y de la estrella ancla; una llave que gira para la cuerda de escalada.
- **Munición:** no aplica.
- **Objetivo:** no hay indicador en pantalla; el objetivo se cuenta con Efeméride y con el escenario.
- **Mapa:** no hay; cada sala se ve completa con su cámara.
- **Indicadores contextuales:** anillo sobre el farol o bloque al que se enganchará el gancho, vista previa de la estrella ancla y carteles de controles dentro del escenario.

El HUD se oculta cuando el jugador no tiene el control (conversaciones y cinemáticas).

## Jerarquía visual

1. El personaje y los peligros inmediatos.
2. Los objetivos enganchables, las superficies y el camino.
3. Los recursos (anillos y llave del Astrolabio).
4. El texto de Efeméride, que no compite con la acción porque solo aparece en pausas.

## Estados

- **Normal:** anillos encendidos según los usos disponibles.
- **Uso gastado:** el anillo se apaga.
- **Advertencia:** la llave tiembla y suena un clic acelerado cuando la cuerda está por agotarse; la cuerda del balanceo se pone roja en los últimos 2 s.
- **Éxito:** destello al escribir una estrella y brillo del Astrolabio al guardar un fragmento.
- **Error:** la mira de la estrella ancla se pone roja si la posición no es válida.
- **Bloqueo:** durante una conversación o cinemática no hay control y el HUD se oculta.
- **Muerte:** efecto breve de destrucción y reaparición; no hay pantalla de derrota.

## Convenciones

**Tipografía:**
Fuente de píxeles propia, legible a 1280×720 px. Texto blanco cálido (`#ffecd6`) sobre un marco dorado tenue; cada hablante tiene su propio color de apoyo.

**Iconografía:**
Las teclas y los botones se dibujan al estilo de los carteles pintados en el escenario. Los iconos cambian solos según el último dispositivo usado (teclado o mando); si dos teclas hacen lo mismo en el mando, se dibuja una sola.

**Tamaños mínimos:**
El texto debe leerse a la resolución base (1280×720 px, escalada con filtro de píxel en 1080p).

**Contraste:**
Texto claro sobre fondo oscuro; la información jugable nunca se apoya solo en el color.

**Animaciones:**
El texto aparece letra a letra, con etiquetas para pausas, ondas y temblor. Las transiciones usan fundidos breves.

## Pantallas

- Menú principal
- Pausa
- Configuración
- Créditos
- Tarjeta final (estadísticas de la partida)

No existen Inventario, Mapa, Victoria ni Derrota.

El flujo y la estructura de las pantallas se detallan en [[02 - UI y Menús]].

> **Navegación:** [[00 - Índice]] · ← [[03 - Entornos]] · [[05 - Audio y Música]] →
