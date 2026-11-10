# Requisitos técnicos

Los valores son objetivos de diseño y se confirman al medir el rendimiento de la demo.

| Requisito       | Mínimo                                                    | Recomendado                                           |
| --------------- | --------------------------------------------------------- | ----------------------------------------------------- |
| Sistema         | Windows 11 (64 bits)                                      | Windows 11 (64 bits)                                  |
| CPU             | Dos núcleos a 2,0 GHz                                     | Cuatro núcleos a 2,5 GHz                              |
| GPU             | Gráficos integrados compatibles con DirectX 11            | Tarjeta dedicada básica o integrada reciente          |
| RAM             | 4 GB                                                      | 8 GB                                                  |
| Almacenamiento  | 500 MB libres                                             | 1 GB libre en SSD                                     |
| Conexión        | No requerida                                              | No requerida                                          |

El juego se dibuja a 1280×720 (40 × 22,5 tiles de 32 px) y se escala con filtro de píxel a 1920×1080 (×1,5); la escala es entera en 720p, 1440p y 2160p, y otras resoluciones 16:9 usan bandas negras si hace falta. El objetivo es 60 FPS estables (la física corre a 50 pasos por segundo con interpolación), menos de 1 GB de RAM y menos de 5 s de carga al pasar de las Entrañas al Eje Central, donde el elevador funciona como pantalla de carga. La demo es solo para Windows.

> **Navegación:** [[00 - Índice]] · ← [[02 - Motor y Herramientas]] · [[04 - Datos y Persistencia]] →
