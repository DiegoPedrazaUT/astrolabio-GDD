# Arquitectura Técnica

## Arquitectura

```text
Entrada (un único lector de entrada)
  ↓
Controlador del jugador (orquestador)
  ↓
Mecánicas del jugador (movimiento, salto, salto de pared|, escalada, gancho, estrella ancla)
  ↓
Sistemas del mundo (plataformas, salas y cámara, peligros, reaparición)
  ↓
Datos / Persistencia (progreso, configuración)
  ↓
Presentación (animación, efectos, sonido, interfaz y diálogos)
```

La presentación **solo escucha eventos**: cambiar el arte, el sonido o la interfaz nunca altera la jugabilidad.

## Componentes principales

| Componente                  | Responsabilidad                                                                               | Dependencias                    |
| --------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------- |
| Lector de entrada           | Único punto que habla con el Input System; entrega direcciones y pulsaciones ya interpretadas | Input System                    |
| Controlador del jugador     | Orquesta el paso de física y decide qué mecánica controla el cuerpo                           | Lector de entrada, mecánicas    |
| Sensores                    | Detectan suelo, pared y aplastamiento                                                         | Física 2D, capas                |
| Mecánicas del jugador       | Cada una es un componente propio: movimiento, salto, pared, escalada, gancho, estrella ancla         | Sensores                        |
| Plataformas y recogibles    | Plataformas móviles, cristales de recarga y piezas del nivel                                  | Física 2D, evento de reinicio   |
| Salas y cámara              | Dividen el nivel en pantallas, cambian de cámara y fijan el punto de reaparición              | Cinemachine                     |
| Reaparición                 | Muerte, reaparición  y reinicio del nivel                                                     | Salas, peligros                 |
| Cinemáticas y diálogos      | Secuencias de pasos, burbujas de texto y holograma de Efeméride                              | Lector de entrada, presentación |
| Progreso y guardado         | Estado de la partida (fragmentos, poemas) y su archivo                                 | Datos y persistencia            |
| Presentación                | Animación, efectos visuales, sonido, HUD y menús                                              | Eventos de las mecánicas        |

## Comunicación

- **Eventos.** Las mecánicas avisan de lo que ocurre (saltó, aterrizó, enganchó, soltó, murió, reapareció, obtuvo un fragmento) y la presentación se suscribe a esos eventos.
- **Evento de reinicio del nivel.** Cuando el jugador reaparece, todo lo que se suscribe (plataformas, cristales, losas, estrellas) vuelve a su estado inicial.
- **Un único orquestador.** Solo el controlador del jugador ejecuta la física en cada paso fijo; así nunca hay dos mecánicas escribiendo la velocidad a la vez y cada una se puede probar por separado.
- **Capas de física.** Las capas (suelo liso, suelo rugoso, metal estelar enganchable, rejilla y peligros) deciden qué se puede pisar, agarrar o enganchar, sin necesidad de etiquetas ni scripts en cada tile.

## Principios técnicos

- Bajo acoplamiento cuando sea razonable.
- Responsabilidades claras: un componente por responsabilidad.
- Código mantenible.
- Datos separados de lógica cuando corresponda (valores ajustables en el Inspector, no escritos en el código).
- Evitar dependencias innecesarias.

> **Navegación:** [[00 - Índice]] · ← [[04 - Guardado y Configuración]] · [[02 - Motor y Herramientas]] →
