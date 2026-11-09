# Pilares de diseño

## Inmensidad silenciosa

Un mundo inmenso, antiguo y solitario, de ambientes oscuros con luz escasa y cálida. La atmósfera se construye con pixel art sobre un espacio profundo: engranajes del tamaño de edificios en capas de paralaje y un personaje diminuto. La legibilidad manda: el fondo es siempre más oscuro y menos saturado que el primer plano, las superficies escalables tienen textura rugosa y las que no se escalan son lisas.

## Movilidad fluida y castigo justo

El diseño de niveles exige saltos milimétricos y un uso inteligente del anclaje y del hilo. Un toque de peligro mata, no hay vidas y el jugador reaparece en la sala casi al instante (objetivo de diseño: menos de medio segundo). Si muere, debe saber que fue un error de cálculo propio. Las reglas son consistentes: los usos restantes, la superficie que se agarra y lo peligroso se ven sin texto. Los números del jugador viven en un único asset ajustable (`PlayerTuning`), de modo que la sensación se afina sin tocar código.

## Narrativa ambiental y poesía visual

La historia del Gran Reloj Cósmico y de los Almanaques anteriores no interrumpe la acción con textos largos: se cuenta con el arte de los escenarios, los poemas y la carta de despedida del Almanaque XI. Efeméride, la voz del Reloj, aparece con burbujas de texto cortas. Una caja de diálogo con texto letra a letra ya existe en el juego; el contenido narrativo final está en [[04 - Diálogos y Narrativa]].

## Crear el camino

El jugador no sigue una ruta fija: la construye. El anclaje lo escribe él y el hilo solo engancha en superficies y anclajes marcados como enganchables. Las salas admiten más de una solución, y el tutorial enseña esa libertad paso a paso. Ninguna mecánica nueva debe reemplazar esa creatividad.

## Reglas de decisión

Antes de incorporar una característica importante:

- ¿Refuerza uno de los pilares?
- ¿Mejora la experiencia principal?
- ¿Cabe en el alcance de la demo (ver [[01 - Alcance]])?
- ¿Complica innecesariamente otro sistema?


> **Navegación:** [[00 - Índice]] · ← [[03 - Público y Plataforma]] · [[01 - Jugabilidad]] →
