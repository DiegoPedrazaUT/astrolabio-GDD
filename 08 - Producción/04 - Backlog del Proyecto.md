# Backlog del Proyecto

## Descripción de la sección

El backlog contiene el trabajo necesario para convertir el diseño en un videojuego funcional.

El estado de cada tarea (pendiente, en progreso, bloqueada o terminada) se sigue en el tablero de tareas del equipo.

## Formato de tarea

### Tarea

**Descripción:**

**Responsable:**

**Prioridad:** Alta / Media / Baja

**Dependencias:**

**Criterio de aceptación:**

**Estado:** Pendiente / En progreso / Bloqueada / Terminada

## Backlog

### Núcleo del jugador

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Movimiento y salto de precisión                        | Diego Angel Ramirez Fernandez    | Alta      | Entrada                         | Salto variable con *coyote time* y memoria de pulsación; se siente justo y predecible |
| Agarre y escalada con cuerda limitada                  | Diego Angel Ramirez Fernandez    | Alta      | Movimiento                      | Se agarra solo a superficies rugosas; la cuerda se agota y se recarga al tocar suelo |
| Gancho (balanceo y arrastre)                           | Diego Angel Ramirez Fernandez    | Alta      | Movimiento, superficies         | Dos usos compartidos; conserva la velocidad al soltar; la cuerda choca con las esquinas |
| Anclaje de apoyo (estrella)                            | Diego Angel Ramirez Fernandez    | Alta      | Gancho                          | Se coloca en cualquier estado y el gancho puede engancharse a él                     |
| Salas, cámara, muerte y reaparición                    | Diego Angel Ramirez Fernandez    | Alta      | Movimiento                      | Reaparece en 0.4 s al inicio de la sala con todo recargado                          |
| Plataformas móviles, peligros y cristales de recarga   | Diego Angel Ramirez Fernandez    | Media     | Salas                           | Patrulla, zip, rejilla, losa y elevador; el jugador hereda su velocidad              |

### Contenido

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Las Entrañas del Reloj (5 zonas)                 | Diego Angel Ramirez Fernandez    | Alta      | Núcleo del jugador              | Cada sala presenta una idea antes de examinarla; se completa en 10 a 15 minutos     |
| Casa de Géminis                                        | Diego Angel Ramirez Fernandez    | Alta      | Entrañas, regla de Géminis      | Se completa; cada sala usa la regla propia                                           |
| Observatorio de Ofiuco y Cámara Central                | Diego Angel Ramirez Fernandez    | Media     | Casa de Géminis                 | Se leen la última nota y la carta de XI; la Cámara Central muestra el desenlace      |
| Regla de la Casa de Géminis (espejos)                   | Diego Angel Ramirez Fernandez    | Alta      | Gancho y anclaje                | Cada regla se prueba en una sala aislada antes de integrarse                         |
| Poemas y notas del Almanaque XI                        | Aleksander Rocha Baeza           | Baja      | Observatorios                   | Entre 4 y 5 poemas, las notas de las Dos Lentes y la carta de Ofiuco                     |

### Narrativa

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Diálogos de Efeméride por zona                         | Aleksander Rocha Baeza           | Alta      | Estructura de niveles           | Textos cortos al inicio y al final de cada zona                                      |
| Textos de hologramas, carteles y rótulos de zona       | Aleksander Rocha Baeza           | Media     | Diálogos                        | Coherentes con el tono de cada Casa                                                  |

### Arte

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Animaciones del Almanaque XII                          | Dalia Jimena Chim Uc             | Alta      | Arte del personaje              | Todas las animaciones de [[02 - Personajes y Animación]]                             |
| Tilesets de las Entrañas, Géminis y el final           | Dalia Jimena Chim Uc             | Alta      | Paleta SLSO8                    | Las seis superficies por zona, de 32×32 px, como *Rule Tiles*                     |
| Fondos de parallax y piezas de nivel                   | Victor Alexis Yah Alpuche        | Media     | Paleta SLSO8                    | Fondos más oscuros que el primer plano; piezas legibles                              |
| Efectos visuales (partículas y destellos)              | Victor Alexis Yah Alpuche        | Media     | Mecánicas                       | Cada acción importante tiene su señal visual                                         |

### Interfaz y sistemas

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| HUD (anillos y llave del Astrolabio)                   | Victor Alexis Yah Alpuche        | Alta      | Mecánicas                       | Muestra usos y cuerda sin tapar la acción                                            |
| Menús: principal, pausa, configuración y créditos      | Victor Alexis Yah Alpuche        | Alta      | Guardado                        | Navegables con teclado, ratón y mando                                                |
| Selector de Casa y ascensor                            | Diego Angel Ramirez Fernandez    | Media     | Estructura de niveles           | Carga la Casa elegida mientras habla Efeméride                                       |
| Guardado y configuración                               | Felipe Natanael Chan Uc          | Alta      | Menús                           | Guarda en observatorios mayores y al cambiar de Casa; recupera un archivo dañado     |
| Ayudas de entrada y de puntería                        | Diego Angel Ramirez Fernandez    | Alta      | Entrada, gancho                 | El jugador consigue lo que quiso hacer aunque se desvíe un poco                      |

### Audio

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Música por capas (Entrañas, Géminis y final)           | Felipe Natanael Chan Uc          | Media     | Estructura de niveles           | Las capas se suman sin romper el pulso                                               |
| Efectos de sonido de [[05 - Audio y Música]]           | Felipe Natanael Chan Uc          | Alta      | Mecánicas                       | Todos los eventos de la tabla tienen su sonido                                       |

### Calidad, publicación y marketing

| Tarea                                                  | Responsable                      | Prioridad | Dependencias                    | Criterio de aceptación                                                              |
| ------------------------------------------------------ | -------------------------------- | --------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| Pruebas con jugadores nuevos y ajuste de dificultad    | Todo el equipo                   | Alta      | Niveles                         | Un jugador nuevo termina el tutorial sin ayuda externa                               |
| Build de Windows y publicación en itch.io              | Diego Roman Pedraza Keb          | Alta      | Contenido cerrado               | Se descarga y se ejecuta en un equipo limpio                                         |
| Página de itch.io, donaciones y material del evento    | Diego Roman Pedraza Keb          | Media     | Build                           | Página publicada y material de presentación listo                                    |

## Priorización

Prioriza aquello que desbloquea otras tareas o valida primero las partes más riesgosas del proyecto.

1. El núcleo del jugador (gancho, anclaje y escalada), porque todo el diseño de niveles depende de él.
2. Las Entrañas del Reloj, porque enseñan las cuatro habilidades y son el vertical slice.
3. La Casa de Géminis completa antes de empezar el final.
4. Pulido, audio y contenido opcional al final, siguiendo los criterios de recorte de [[01 - Alcance]].


> **Navegación:** [[00 - Índice]] · ← [[03 - Roadmap]] · [[05 - Gestión de Cambios]] →
