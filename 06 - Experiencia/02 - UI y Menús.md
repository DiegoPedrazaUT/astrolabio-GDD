# UI y Menús

## Descripción de la sección

Define la estructura funcional de las interfaces y menús.

## Mapa de navegación

```text
Menú principal
├── Nueva partida
├── Continuar                      (solo si existe una partida guardada)
├── Configuración
│   ├── Audio
│   ├── Idioma 
│   └── Controles
├── Créditos
└── Salir

Durante el juego
├── Pausa
│   ├── Continuar
│   ├── Configuración
│   └── Volver al menú principal
├── Selector de Casa (dial de reloj, en el Pozo Celeste)
└── Tarjeta final (al restaurar las Casas jugables)
```

Los menús se manejan con teclado, ratón o mando. Confirmar: Espacio o A.

## Pantallas

### Menú principal

**Propósito:** Entrada al juego.

**Elementos:** Título, fondo del Reloj con parallax y las opciones del mapa de navegación.

**Acciones disponibles:** Nueva partida, Continuar, Configuración, Créditos y Salir.

**Estados:** Con partida guardada (Continuar habilitado) y sin partida guardada (Continuar oculto o deshabilitado).

**Transiciones:** Nueva partida y Continuar llevan al juego con un fundido.

### Pausa

**Propósito:** Detener el juego sin perder el contexto.

**Elementos:** Lista de opciones sobre el juego atenuado.

**Acciones disponibles:** Continuar, Configuración y Volver al menú principal.

**Estados:** Se abre y se cierra con la misma tecla (TAB; Start en el mando). No se puede abrir durante una cinemática.

**Transiciones:** Continuar regresa de inmediato al punto exacto donde se pausó.

### Configuración

**Propósito:** Ajustar audio, video, controles y accesibilidad (ver [[04 - Guardado y Configuración]]).

**Elementos:** Pestañas por categoría y controles deslizantes e interruptores.

**Acciones disponibles:** Cambiar un valor, probarlo en el momento y restablecer la categoría.

**Estados:** Valores predeterminados y valores personalizados.

**Transiciones:** Regresa a la pantalla desde la que se abrió (menú o pausa).

### Selector de Casa

**Propósito:** Elegir a qué Casa subir después de las Entrañas.

**Elementos:** Un dial de reloj con las doce Casas; las que no se pueden visitar se muestran apagadas.

**Acciones disponibles:** Mover el dial (izquierda y derecha) y confirmar con salto.

**Estados:** Casa disponible, Casa restaurada y Casa no jugable.

**Transiciones:** Al confirmar, el ascensor sube mientras Efeméride habla y carga la Casa elegida.

### Tarjeta final

**Propósito:** Cerrar la demo mostrando el resultado de la partida.

**Elementos:** Casas restauradas, poemas y notas encontrados, muertes y tiempo de juego.

**Acciones disponibles:** Ver créditos o volver al menú principal.

**Estados:** Única.

**Transiciones:** Créditos o menú principal.

## Confirmaciones

Documenta acciones destructivas o irreversibles y cómo se confirman.

| Acción                                       | Confirmación                                                                                 |
| -------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Nueva partida con una partida guardada        | Pregunta si se desea reemplazar la partida actual                                            |
| Volver al menú principal desde la pausa       | Avisa que se pierde el progreso desde el último punto guardado                               |
| Salir del juego                               | Solo pide confirmación si hay progreso sin guardar                                           |
| Restablecer configuración                     | Pide confirmación para volver a los valores predeterminados                                  |
| Borrar la partida                             | Doble confirmación, separada del resto de las opciones                                       |


> **Navegación:** [[00 - Índice]] · ← [[01 - UX y Flujo del Jugador]] · [[03 - Accesibilidad]] →
