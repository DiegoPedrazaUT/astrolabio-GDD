# Estructura del Contenido

## Descripción de la sección

Organiza el contenido del videojuego en unidades manejables: mundos, capítulos, zonas, niveles, misiones y desafíos.

## Estructura

```text
Juego
├── Las Entrañas del Reloj (tutorial, 5 zonas)
│   ├── La Sala de los Nichos
│   ├── La Galería de Engranajes
│   ├── El Puente Roto           (se entrega el gancho)
│   ├── El Pozo de Cadenas
│   └── El Pozo Celeste          (se entrega el anclaje; primer fragmento)
├── Casa de Géminis (5 zonas)
│   ├── El Atrio de los Gemelos
│   ├── La Galería de Espejos
│   ├── Los Puentes Paralelos
│   ├── La Torre Invertida
│   └── La Cámara de los Gemelos
└── Final 
    ├── El Observatorio de Ofiuco
    └── La Cámara Central
```

Entre una Casa y la siguiente se pasa por el Eje y se sube en un ascensor de engranajes, una transición breve que también sirve como pantalla de carga.

## Cantidad estimada

| Tipo                  |                                                                  Cantidad |
| --------------------- | ------------------------------------------------------------------------: |
| Mundos                |                               3 en la demo (Entrañas, Géminis y el final) |
| Zonas                 |                                                 12 en la demo (5 + 5 + 2) |
| Salas de las Entrañas |                                                                    Unas 8 |
| Salas de Géminis      |                                                Entre 8 y 12 (por definir) |
| Misiones              |                    1 principal (devolver las constelaciones) y 1 opcional |
| Enemigos              |                                                         0: no hay combate |
| Jefes                 |                                                                         0 |
| NPC                   |                      0 con los que se converse; Efeméride es la única voz |
| Objetos               | Fragmentos de estrella, poemas, cristal de recarga, checkpoints y faroles |
| Poemas                |                                1 oculto en las Entrañas; 3 o 4 en Géminis |

## Dependencias

¿Qué contenido debe existir antes de otro?

- Las Entrañas enseñan las cuatro habilidades y deben existir antes que cualquier Casa. El gancho se entrega en el Puente Roto y el anclaje en el Pozo Celeste.
- El primer fragmento de estrella (Pozo Celeste) abre el ascensor hacia las Casas.
- Cada Casa depende de que sus mecánicas propias estén diseñadas y probadas en salas de prueba antes de construir el nivel.


> **Navegación:** [[00 - Índice]] · ← [[04 - Diálogos y Narrativa]] · [[02 - Niveles]] →
