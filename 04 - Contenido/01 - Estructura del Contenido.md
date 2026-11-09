# Estructura del Contenido

## Descripción de la sección

Organiza el contenido del videojuego en unidades manejables: mundos, capítulos, zonas, niveles, misiones y desafíos.

## Estructura

```text
Demo
├── Las Entrañas del Reloj (tutorial, 5 zonas, 18 salas)
│   ├── La Sala de los Nichos
│   ├── La Galería de Engranajes   (incluye un elevador de un solo sentido)
│   ├── El Puente Roto             (se entrega el gancho)
│   ├── El Pozo de Cadenas
│   └── El Pozo Celeste            (se entrega el anclaje; primer fragmento)
└── El Eje Central (sala de llegada; fin de la demo)
```

El elevador del Pozo Celeste sube hasta el Eje Central en un ascenso exterior: un cielo que se oscurece, el Gran Reloj al fondo y Géminis señalada. En el juego completo, del Eje Central se llegará a cada Casa por elevador.

**Fuera de la demo:** la Casa de Géminis, las demás Casas y el desenlace están previstos para el juego completo y no forman parte de esta entrega (ver [[01 - Alcance]]).

## Cantidad estimada

| Tipo                  |                                                                  Cantidad |
| --------------------- | ------------------------------------------------------------------------: |
| Mundos                |                                    2 en la demo (Entrañas y Eje Central) |
| Zonas                 |                          6 en la demo (5 de las Entrañas y el Eje Central) |
| Salas de las Entrañas |                          18 (el reparto por zonas es provisional) |
| Salas del Eje Central |                                                                         1 |
| Misiones              |            1 principal (llegar al Eje Central) y 1 opcional (el poema oculto) |
| Enemigos              |                                                         0: no hay combate |
| Jefes                 |                                                                         0 |
| NPC                   |                      0 con los que se converse; Efeméride es la única voz |
| Objetos               | Fragmento de estrella, poema, cristal de recarga, checkpoints y faroles |
| Poemas                |         1 oculto en las Entrañas; hay 5 textos propuestos (ver [[04 - Diálogos y Narrativa]]) |

## Dependencias

- Las Entrañas enseñan las cuatro habilidades y deben existir antes que cualquier Casa. El gancho se entrega en el Puente Roto y el anclaje en el Pozo Celeste.
- El primer fragmento de estrella (Pozo Celeste) abre el elevador hacia el Eje Central.
- Cada Casa del juego completo depende de que sus mecánicas propias estén diseñadas y probadas en salas de prueba antes de construir el nivel.


> **Navegación:** [[00 - Índice]] · ← [[04  Diálogos y Narrativa]] · [[02 - Niveles]] →
