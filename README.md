# CodeStart FIEC — Prototipo de interfaz

Mockup navegable de la plataforma **CodeStart FIEC**, de apoyo al Curso Propedéutico de la
Facultad de Informática, Electrónica y Comunicación (FIEC) — Universidad de Panamá.

> **Avance 2 — Diseño Instruccional y de Interfaz**
> Documentación de diseño + prototipo navegable, en un solo archivo estático.

**Ver en vivo:** <https://zobercito.github.io/codestart-fiec-mockup/>

---

## Qué hay aquí

Un único archivo (`index.html`) con dos cosas a la vez:

**1. El prototipo** — 4 pantallas navegables de la plataforma:

| | Pantalla | Requisitos |
|---|---|---|
| **A** | Dashboard del estudiante — progreso, ruta de 8 módulos, tareas asignadas, medallas | RF02, RF05, RF06, RF13 |
| **B** | Lección interactiva — modo clase, video, animación del recorrido de una instrucción, simulador de memoria, anatomía del código línea por línea | RF03, RF09, RF16 |
| **C** | Editor de retos — editor con casos de prueba, pistas progresivas, salida aislada, diagnóstico de error | RF04, RF10, RF11 |
| **D** | Panel docente — grupos, KPIs, seguimiento por estudiante, análisis de errores frecuentes | RF07, RF13, RF14, RF15 |

**2. La documentación de diseño del A2**, embebida en el mismo archivo:

| | Sección | Qué documenta |
|---|---|---|
| ▣ | **Guía de estilo** | Tokens de color con contraste medido (WCAG 2.1), tipografía, espaciado, componentes base, microinteracciones del editor y reglas de accesibilidad |
| ▤ | **Storyboard** | Las 4 pantallas con sus objetivos, datos, interacciones, microcopy y estados alternos — **anotadas sobre el prototipo real**, no dibujadas aparte |
| ⌘ | **Mapa de navegación** | Flujos de estudiante, docente y administrador, con guardas de acceso y equivalencia mapa ↔ requisito |
| ✓ | **Validación con usuarios** | Protocolo de la prueba de usabilidad, instrumentos y criterios de aceptación |

---

## Cómo navegar

La barra superior tiene dos grupos: **Prototipo** (las pantallas) y **Diseño** (la documentación).
La barra también permite cambiar entre pantallas; en la sección *Storyboard* cada ficha
tiene un botón **«Abrir pantalla anotada»** que salta a la pantalla real y activa los
marcadores numerados sobre ella.

---

## Identidad visual

| Token | Valor | Uso |
|---|---|---|
| FIEC | `#0B62A4` | Color institucional: navegación, enlaces, acciones primarias |
| UP | `#F5B014` | Color de la universidad: progreso, racha, insignias, advertencias |
| Éxito | `#10B981` | Aciertos, módulos completados, casos de prueba aprobados |
| Error | `#EF4444` | Errores de compilación, fallos de validación |
| Texto | `#0F172A` → `#475569` | Jerarquía de texto (7 niveles medidos contra WCAG AA) |
| Tipografía | Inter + JetBrains Mono | Texto e interfaz / código |
| Fondo | `#F8FAFC` · `#FFFFFF` | Canvas de la app y de las tarjetas |

Los pares de color permitidos y los prohibidos, con su razón de contraste medida,
están en la **Guía de estilo**.

---

## Notas técnicas

- **Un solo archivo, sin build.** Tailwind por CDN, JS vanilla. Se abre con doble clic
  o se sirve tal cual desde GitHub Pages.
- **Peso:** ~430 KB (los logos están en `assets/`, no embebidos en base64).
- **Accesibilidad:** contraste AA verificado, foco visible, interacción de código
  funciona con ratón, teclado y táctil (`hover` + `focus-visible` + clic).
- **Responsive:** verificado a 390 px (móvil), 768 px (tableta) y 1500 px (escritorio).

---

## Documentación relacionada

El **Avance 1 — Análisis y Planificación** (21 secciones, 18 RF, 9 RNF) y la
documentación de la asignatura se versionan por separado, en el repositorio de
documentación del proyecto.

---

**Materia:** Informática Educativa · 2do Semestre 2026 · Prof. Alvin Blanco
**Equipo:** Francisco Gonzalez · Eira Arrocha · Yasari Ortiz · Domingo de León
