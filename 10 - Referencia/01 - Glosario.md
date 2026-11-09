# Glosario

## Descripción de la sección

Define los términos del juego, del equipo y del código que aparecen en el GDD, para que todos hablen de lo mismo.

## Mundo y personajes

| Término | Definición |
| --- | --- |
| **Almanaque XII** | El protagonista: un autómata, el duodécimo de su linaje. Ver [[03 - Personajes]] |
| **Efeméride** | Personaje que acompaña a los Almanaques y les da órdenes. Ver [[03 - Personajes]] |
| **Gran Reloj Cósmico** | La máquina que fijó el destino de todos y por la que asciende el Almanaque |
| **Entrañas del Reloj** | Zona del tutorial (18 salas), en la base del Reloj |
| **Pozo Celeste** | Última sala del tutorial: el elevador al aire libre hacia el cielo |
| **Eje Central** | Zona a la que llega el elevador; cierra la demo |
| **Casa** | Cada una de las regiones zodiacales del juego completo (Géminis, entre ellas) |
| **Constelaciones rotas** | Lo que el Almanaque debe devolver a su órbita |

## Mecánicas y piezas

| Término | Definición |
| --- | --- |
| **Hilo** | Hilo de luz que el jugador dispara para engancharse, balancearse o arrastrarse. Tiene 2 usos |
| **Estrella-anclaje** | Punto de apoyo que el jugador escribe en el vacío (tecla E) y al que puede enganchar el hilo |
| **Cuerda (de escalada)** | Resistencia para agarrarse a superficies rugosas: 100 puntos, se rellena al pisar suelo |
| **Farol** | Punto de enganche fijo para el hilo |
| **Cristal / estrella recargable** | Pieza que devuelve los usos del hilo |
| **Checkpoint** | Punto donde reaparece el jugador tras morir |
| **Compuerta** | Puerta que se abre al acercarse y se cierra detrás |
| **Sala** | Unidad del nivel: tiene su cámara y sus puntos de reaparición. Su nombre es su identificador |
| **Gas nebuloso** | Peligro estático que mata al tocarlo y corta el hilo |
| **Engranaje / sierra** | Peligros letales; los engranajes giran y las sierras están hundidas en el muro |
| **Metal estelar** | Superficie enganchable que responde al hilo con una onda de luz |
| **Plataforma de patrulla, zip, losa, rejilla** | Plataformas que recorren un camino, se lanzan al llegar, se caen al pisarlas o se atraviesan desde abajo |
| **Elevador de solo ida** | Elevador que no se puede volver a usar; añade un punto de reaparición arriba |

## Arte

| Término | Definición |
| --- | --- |
| **SLSO8** | Paleta base de 8 colores del proyecto |
| **Tile** | Cuadro de 32 × 32 px, equivalente a 1 unidad del juego |
| **Rule Tile** | Tile que elige solo su sprite según los vecinos, para evitar costuras |
| **Hoja de fotogramas** | Imagen con todos los cuadros de una animación en fila |
| **Graybox** | Nivel hecho con piezas grises para probar el diseño antes de poner arte |

## Tecnología y proceso

| Término | Definición |
| --- | --- |
| **URP 2D** | Pipeline de render 2D de Unity |
| **Input System** | Paquete de Unity para controles; el archivo de controles es `AstrolabioControls.inputactions` |
| **PlayerTuning** | Asset con los números del jugador (correr, salto, pared, escalada) |
| **EditMode / PlayMode** | Dos tipos de prueba automática de Unity: sin ejecutar el juego y ejecutándolo |
| **Análisis estático** | Revisión automática del código sin ejecutarlo (Roslyn) |
| **CI** | Integración continua: GitHub ejecuta pruebas y compilaciones en cada PR |
| **Gitflow** | Flujo de ramas del equipo: `feature/*` → `develop` → `main` |
| **UI Toolkit** | Sistema de interfaz de Unity con el que se hacen menús y HUD |
| **HUD** | Información en pantalla durante el juego (usos, zona) |
| **Demo** | Versión recortada que se presenta; ver [[01 - Alcance]] |
| **Vertical slice** | Un tramo del juego terminado con calidad final |


> **Navegación:** [[00 - Índice]] · ← [[04 - Criterios de Aceptación]] · [[02 - Referencias e Inspiración]] →
