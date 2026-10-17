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
├── Casa de Géminis (6 zonas)
│   ├── El Atrio de los Gemelos
│   ├── La Galería de Espejos
│   ├── Los Puentes Paralelos
│   ├── El Observatorio de las Dos Lentes
│   ├── La Torre Invertida
│   └── La Cámara de los Gemelos
├── Casa de Acuario (6 zonas)
│   ├── Las Fuentes Rotas
│   ├── Los Acueductos
│   ├── Las Esclusas
│   ├── El Remolino
│   ├── El Observatorio del Cauce
│   └── La Cámara del Portador
└── Final 
    ├── El Observatorio de Ofiuco
    └── La Cámara Central
```

Entre una zona y la siguiente se pasa por el Eje y se sube en un ascensor de engranajes, una transición breve que también sirve como pantalla de carga.

## Cantidad estimada

| Tipo                       |                                                                                     Cantidad |
| -------------------------- | -------------------------------------------------------------------------------------------: |
| Mundos                     |                                   4  en la demo (Entrañas, Géminis, Acuario, Cámara Central) |
| Niveles (zonas)            |                                                                    19 en la demo (5 + 6 + 6) |
| Salas de las Entrañas      |                                                                                       Unas 5 |
| Salas de Géminis y Acuario |                                                          Entre 8 y 12 por Casa (por definir) |
| Misiones                   |                                             1 principal (restaurar cada Casa) y 2 opcionales |
| Enemigos                   |                                                                            0: no hay combate |
| Jefes                      |                                                                                            0 |
| NPC                        |                                         0 con los que se converse; Efeméride es la única voz |
| Objetos                    | Fragmentos de estrella, poemas, notas de XI, cristal de recarga, checkpoints y observatorios |
| Observatorios              |                                    3 mayores: Dos Lentes (Géminis), Cauce (Acuario) y Ofiuco |
| Poemas                     |                                 1 oculto en las Entrañas; 3 o 4 en Géminis; 4 o 5 en Acuario |

## Dependencias

¿Qué contenido debe existir antes de otro?

- Las Entrañas enseñan las cuatro habilidades y deben existir antes que cualquier Casa. El gancho se entrega en el Puente Roto y el anclaje en el Pozo Celeste.
- El primer fragmento de estrella (Pozo Celeste) abre el ascensor hacia las Casas.
- Los observatorios dependen del sistema de guardado y de la tecla de interactuar.
- Las notas de XI dependen de los observatorios mayores.
- Cada Casa depende de que sus mecánicas propias estén diseñadas y probadas en salas de prueba antes de construir el nivel.
- Por decidir: si Acuario exige haber restaurado Géminis o si el jugador puede elegir la Casa en el dial del Pozo Celeste.


> **Navegación:** [[00 - Índice]] · ← [[04 - Diálogos y Narrativa]] · [[02 - Niveles]] →
