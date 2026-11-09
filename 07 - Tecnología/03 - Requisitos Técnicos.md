# Requisitos Técnicos

## Descripción de la sección

Define las condiciones técnicas necesarias para ejecutar y desarrollar el videojuego.

## Requisitos mínimos

Los valores son objetivos de diseño y se confirman al medir el rendimiento de la demo.

**Sistema operativo:** Windows 11 (64 bits)

**CPU:** Procesador de dos núcleos a 2.0 GHz o superior

**GPU:** Gráficos integrados compatibles con DirectX 11

**RAM:** 4 GB

**Almacenamiento:** 500 MB libres

**Resolución:** 1920×1080 (el juego se dibuja a 1280×720, es decir, 40 × 22,5 tiles de 32 px, y se escala con filtro de píxel); otras resoluciones 16:9 con bandas negras si hace falta

**Conexión:** No requerida

## Requisitos recomendados

**Sistema operativo:** Windows 11 (64 bits)

**CPU:** Procesador de cuatro núcleos a 2.5 GHz o superior

**GPU:** Tarjeta gráfica dedicada básica, o gráficos integrados recientes

**RAM:** 8 GB

**Almacenamiento:** 1 GB libre en una unidad SSD

## Objetivos de rendimiento

**FPS objetivo:** 60 estables (la física corre a 50 pasos por segundo con interpolación para que la cámara se vea suave).

**Tiempo de carga objetivo:** Menos de 5 s entre Casas; el ascensor funciona como pantalla de carga mientras habla Efeméride. El cambio de sala dentro de una Casa no carga nada: dura 0.5 s y no pausa el juego.

**Memoria máxima:** Menos de 1 GB de RAM.

## Restricciones

Documenta límites conocidos del proyecto.

- Solo Windows en la demo; no hay versión para consola ni móvil.
- Relación de aspecto 16:9; otras relaciones se resuelven con bandas negras.
- El pixel art exige filtro de píxel y tiles sin costuras para no deformar los píxeles; la escala es entera en 720p, 1440p y 2160p, y de ×1,5 en 1080p.
- Tres archivos de partida (tres ranuras).

> **Navegación:** [[00 - Índice]] · ← [[02 - Motor y Herramientas]] · [[04 - Datos y Persistencia]] →
