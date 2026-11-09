# Público y plataforma

Astrolabio es un plataformas 2D de precisión para Windows y un solo jugador. Está dirigido a personas de 16 años en adelante que ya conocen el género y disfrutan una dificultad exigente pero justa: dominar el movimiento, superar cada sala y reintentar de inmediato tras cada error. Les atraen el pixel art, las atmósferas oscuras y una narrativa que se descubre mirando.

La dificultad se apoya en reglas legibles: cuántos usos del hilo quedan, qué superficie se agarra y qué mata se distingue sin texto. La demo gratuita sirve para aprender el ciclo completo (escalar, escribir un anclaje, lanzarse con el hilo) en el tutorial antes del cierre en el Eje Central.

## Plataforma

| Elemento | Decisión |
| --- | --- |
| Plataforma principal | PC (Windows) |
| Plataformas secundarias | Consola, por evaluar a futuro |
| Distribución | itch.io |
| Método de entrada | Teclado y ratón; mando, apuntando con el stick derecho |
| Resolución objetivo | 1920 × 1080; vista base de 1280 × 720 (40 × 22,5 tiles de 32 px), con escala ×1,5 a 1080p |
| Relación de aspecto | 16:9 |
| Rendimiento objetivo | 60 FPS estables |
| Conexión requerida | No |

## Restricciones

- **Controles:** el anclaje y el hilo dependen de apuntar; con mando se apunta con el stick derecho y el juego ofrece ayudas de puntería (ver [[04 - Controles]]).
- **Almacenamiento:** la demo **no guarda** el progreso: *Continuar* está bloqueado y la pausa avisa de ello. El guardado propuesto se describe en [[04 - Guardado y Configuración]].
- **Distribución:** la build de Windows se publicará en itch.io; el CI también compila WebGL hacia `main`, pero WebGL no está validada como plataforma de entrega.

## Sesión de juego

La demo dura entre 5 y 15 minutos según la habilidad del jugador. La cifra es una estimación del diseño: todavía no se ha medido con jugadores nuevos (ver [[02 - Pruebas]]).

## Modelo de distribución

Demo gratuita en itch.io, con donaciones voluntarias para apoyar una versión completa (ver [[01 - Alcance]]).

La plataforma, perspectiva y motor se centralizan en [[01 - Ficha del Proyecto]]. Las comprobaciones de accesibilidad se registran en [[03 - Accesibilidad]].


> **Navegación:** [[00 - Índice]] · ← [[02 - Visión del Juego]] · [[04 - Pilares de Diseño]] →
