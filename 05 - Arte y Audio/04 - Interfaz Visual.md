# Interfaz visual

El HUD es mínimo: anillos del Astrolabio para los usos del gancho y de la estrella ancla, y una llave que gira para la cuerda de escalada. No hay vida, munición, mapa ni indicador de objetivo; este se cuenta con Efeméride y con el escenario. Los indicadores contextuales son un anillo sobre el farol o bloque al que se enganchará el gancho, la vista previa de la estrella ancla y los carteles de controles dentro del escenario.

| Estado        | Señal                                                                                                  |
| ------------- | ------------------------------------------------------------------------------------------------------ |
| Uso gastado   | El anillo se apaga                                                                                     |
| Advertencia   | La llave tiembla y suena un clic acelerado con la cuerda por agotarse; la cuerda del balanceo se pone roja en los últimos 2 s |
| Éxito         | Destello al escribir una estrella y brillo del Astrolabio al guardar un fragmento                      |
| Error         | La mira de la estrella ancla se pone roja si la posición no es válida                                  |
| Muerte        | Efecto breve de destrucción y reaparición; no hay pantalla de derrota                                  |
| Guardado      | Indicador pequeño «Guardando…» en el HUD mientras se escribe el registro                               |

La jerarquía visual es: el personaje y los peligros inmediatos, los objetivos enganchables y las superficies, los recursos y, al final, el texto de Efeméride, que no compite con la acción porque solo aparece en pausas.

La tipografía es una fuente de píxeles propia, legible a 1280×720 px: texto blanco cálido (`#ffecd6`) sobre un marco dorado tenue, con un color de apoyo por hablante. El texto aparece letra a letra, con etiquetas para pausas, ondas y temblor. Las teclas y botones se dibujan al estilo de los carteles pintados y cambian solos según el último dispositivo usado. La información jugable nunca depende solo del color. Las pantallas (menú principal, pausa, configuración, créditos y tarjeta final) se describen en [[02 - UI y Menús]].

> **Navegación:** [[00 - Índice]] · ← [[03 - Entornos]] · [[05 - Audio y Música]] →
