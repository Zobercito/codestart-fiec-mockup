# CodeStart FIEC — Diseño instruccional e interfaz

Prototipo navegable de **CodeStart FIEC**, plataforma de apoyo al Curso Propedéutico de la
Facultad de Informática, Electrónica y Comunicación (FIEC) — Universidad de Panamá.

> **Avance 2 — Diseño Instruccional y de Interfaz**
> El prototipo y su documentación de diseño, en un solo archivo estático.

**Ver en vivo:** <https://zobercito.github.io/codestart-fiec-mockup/>

---

## Qué hay aquí

Un único archivo (`index.html`) con dos cosas a la vez.

### 1 · El prototipo

Cuatro pantallas navegables de la plataforma:

| | Pantalla | Requisitos |
|---|---|---|
| **A** | **Dashboard del estudiante** — progreso, ruta de 8 módulos, tareas asignadas, medallas | RF02, RF05, RF06, RF13 |
| **B** | **Lección interactiva** — modo clase, video, animación del recorrido de una instrucción, simulador de memoria, anatomía del código línea por línea | RF03, RF09, RF16 |
| **C** | **Editor de retos** — editor con casos de prueba, pistas progresivas, salida aislada en el navegador, diagnóstico del error | RF04, RF10, RF11 |
| **D** | **Panel docente** — grupos, indicadores del grupo, seguimiento por estudiante, errores frecuentes, próxima acción | RF07, RF13, RF14, RF15 |

### 2 · La documentación de diseño

En las pestañas **«Diseño»** de la barra superior:

| Sección | Qué documenta |
|---|---|
| **▣ Guía de estilo** | Tokens de color con el contraste medido, tablas de combinaciones permitidas y prohibidas, escala tipográfica, componentes base con sus estados, microinteracciones del editor y reglas de accesibilidad |
| **▤ Storyboard** | Las 4 pantallas con objetivo, actor, precondición, datos, interacciones y estados alternos — **anotadas sobre el prototipo real**, no dibujadas aparte |
| **⌘ Mapa de navegación** | Flujos de estudiante, docente y administrador, guardas de acceso por rol y cobertura de requisitos |
| **✓ Validación** | Protocolo de la prueba de usabilidad: participantes, tareas, instrumento, criterios de aceptación y bitácora de hallazgos |

---

## Cómo navegar

La barra superior tiene dos grupos: **Prototipo** (las pantallas) y **Diseño** (la documentación).

En la sección *Storyboard*, cada ficha tiene un botón **«Abrir pantalla anotada»** que salta a la
pantalla real y activa los marcadores de letra sobre ella. Al pulsar un marcador se abre su
anotación en un panel lateral. Se sale con `Esc`.

---

## Identidad visual

| Token | Valor | Uso |
|---|---|---|
| FIEC | `#0B62A4` | Institucional: navegación, enlaces, acciones primarias |
| UP | `#F5B014` | Universidad: progreso, racha, insignias, advertencias |
| Éxito | `#10B981` | Aciertos, módulos completados |
| Error | `#DC2626` | Fallos de validación, errores de compilación |
| Texto | `#0F172A` → `#64748B` | Jerarquía de texto (7 niveles medidos contra WCAG AA) |
| Tipografía | Inter + JetBrains Mono | Texto e interfaz / código |
| Fondo | `#F8FAFC` · `#FFFFFF` · `#0F172A` | Canvas, tarjetas, editor |

Los pares de color permitidos y prohibidos, con su razón de contraste medida, están en la
**Guía de estilo**.

---

## Notas técnicas

- **Un solo archivo, sin build.** Tailwind por CDN, JS vanilla. Se abre con doble clic o se sirve
  tal cual desde GitHub Pages.
- **Peso:** ~200 KB en total (los logos están en `assets/`, no embebidos en base64).
- **Accesibilidad:** contraste AA verificado sobre el DOM renderizado (0 pares por debajo del
  mínimo), foco visible, e interacción de código que funciona con ratón, teclado y táctil.
- **Responsive:** verificado a 390 px (móvil), 768 px (tableta) y 1500 px (escritorio).

---

## Documentación relacionada

El **Avance 1 — Análisis y Planificación** (21 secciones, 18 RF, 9 RNF) y el material de la
asignatura se versionan por separado, en el repositorio de documentación del proyecto.

---

**Materia:** Informática Educativa · 2do Semestre 2026 · Prof. Alvin Blanco
**Equipo:** Francisco Gonzalez · Eira Arrocha · Yasari Ortiz · Domingo de León
