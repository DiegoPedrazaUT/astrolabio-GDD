# Arquitectura técnica

```text
Entrada (un único lector de entrada)
  ↓
Controlador del jugador (orquestador)
  ↓
Mecánicas del jugador (movimiento, salto, pared, escalada, gancho, estrella ancla)
  ↓
Sistemas del mundo (plataformas, salas y cámara, peligros, reaparición)
  ↓
Presentación (animación, efectos, sonido, interfaz y diálogos)
```

La presentación **solo escucha eventos**: cambiar el arte, el sonido o la interfaz nunca altera la jugabilidad.

| Componente               | Responsabilidad                                                                               |
| ------------------------ | --------------------------------------------------------------------------------------------- |
| Lector de entrada        | Único punto que habla con el Input System; entrega direcciones y pulsaciones ya interpretadas |
| Controlador del jugador  | Orquesta el paso de física y decide qué mecánica controla el cuerpo                           |
| Sensores                 | Detectan suelo, pared y aplastamiento                                                         |
| Mecánicas del jugador    | Un componente por mecánica: movimiento, salto, pared, escalada, gancho y estrella ancla       |
| Plataformas y recogibles | Plataformas móviles, cristales de recarga y piezas del nivel                                  |
| Salas y cámara           | Dividen el nivel en pantallas con Cinemachine y fijan el punto de reaparición                 |
| Reaparición              | Muerte, reaparición y reinicio del nivel                                                      |
| Cinemáticas y diálogos   | Secuencias de pasos, burbujas de texto y holograma de Efeméride                               |
| Presentación             | Animación, efectos visuales, sonido, HUD y menús                                              |

Las mecánicas avisan de lo que ocurre (saltó, aterrizó, enganchó, soltó, murió, reapareció, obtuvo un fragmento) mediante eventos, y un evento de reinicio devuelve plataformas, cristales, losas y estrellas a su estado inicial cuando el jugador reaparece. Solo el controlador del jugador ejecuta la física en cada paso fijo, así nunca hay dos mecánicas escribiendo la velocidad a la vez y cada una se puede probar por separado. Las capas de física (suelo liso, suelo rugoso, metal estelar enganchable, rejilla y peligros) deciden qué se puede pisar, agarrar o enganchar, sin etiquetas ni scripts en cada tile. Los valores ajustables viven en el Inspector, no en el código.

> **Navegación:** [[00 - Índice]] · ← [[04 - Guardado y Configuración]] · [[02 - Motor y Herramientas]] →
