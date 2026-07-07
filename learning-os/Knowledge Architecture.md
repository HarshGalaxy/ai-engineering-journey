# Knowledge Architecture

A map of the field I am entering — not a copy of my university's syllabus,
but a model of how the knowledge actually connects, and where I choose to
go beyond what UMOV teaches.

## How to read this document

The degree is organized into five pillars. Within each pillar there are
two layers:

- **Core** — what UMOV teaches. Guaranteed by the curriculum (plan 2024).
- **Edge** — what the industry uses that UMOV under-teaches or teaches
  late. Every Edge item must justify itself under **Rule #0**: nothing is
  added because it is new or popular, only because a real project or a
  real dependency requires it.

Core anchors me. Edge differentiates me. Neither is sufficient alone.

---

## Pillar 1 — Mathematical Foundations

**Why it exists:** Every model in data science and AI is mathematics in
disguise. This pillar is the language the rest of the field is written in.

**Core (UMOV):**
- Álgebra y Geometría Analítica, Cálculo Diferencial, Cálculo Integral
- Álgebra Lineal, Matemáticas Discretas, Ecuaciones Diferenciales
- Métodos Numéricos, Probabilidad y Estadística, Métodos Estadísticos
- Teoría de Gráficas, Geometría del Espacio, Lógica Clásica
- Probabilidad Aplicada y Simulación Estocástica
- Métodos Matemáticos Computacionales para Ciencia de Datos

**Internal dependency chain (what needs what):**

**Edge (justified additions):**
- **Computational linear algebra early (NumPy).** Reason: UMOV teaches
  linear algebra as pure theory; industry never does it by hand. Pairing
  each concept with its NumPy operation from day one prevents the common
  gap where a student "knows" matrices but can't use them in code.
- **Intuition-first supplements (visual math resources).** Reason: my own
  learning principle is intuition before formulas. The curriculum is
  formula-first; I compensate deliberately.

---

## Pillar 2 — Programming & Software Development

**Why it exists:** Ideas only become systems through code. This pillar is
how I turn understanding into working artifacts.

**Core (UMOV):**
- Principios de Programación, Algoritmos Computacionales
- Programación Estructurada, Lenguajes de Programación
- Estructura de Datos, Programación Orientada a Objetos
- Paradigmas y Programación para Ciencia de Datos
- Computación Distribuida, Computación Concurrente

**Internal dependency chain:**

**Edge (justified additions — the "assumed" skills):**
These are things the industry assumes you know but curricula teach late or
never. Each is justified because I need it NOW to run my own repository:

- **Git & version control.** Reason: already in use — this is how my
  learning repo exists. Non-negotiable in any job.
- **Command line / Linux basics.** Reason: servers run on Linux; the
  mayúsculas lesson (Linux is case-sensitive) already bit me.
- **Virtual environments (venv/conda).** Reason: needed the moment I
  install my second Python library without breaking the first.
- **Reading documentation.** Reason: the single most-used skill of a real
  engineer, and taught in no course.
- **Testing, linting, Docker, APIs.** Reason: required later, when the
  father-maintenance project needs to run somewhere other than my laptop.
  Placeholder so I see them coming.

---

## Pillar 3 — Applied Data Science

**Why it exists:** The bridge between raw data and decisions — the pillar
closest to my economics background.

**Core (UMOV):**
- Bases de Datos Relacionales, Bases de Datos, Bases de Datos Avanzadas
- Análisis de Datos Masivos, Visualización de Datos (cuatr. 08)
- Minería de Datos (cuatr. 08), Reconocimiento de Patrones
- Matemáticas Financieras, Tecnologías Financieras (cuatr. 09)

**Edge:** _To be detailed as I approach this pillar (≈ cuatrimestre 4+)._
Likely candidates under Rule #0: SQL beyond coursework, Pandas fluency,
real dashboarding tools. Deferred deliberately — detailing them now would
be mapping territory I won't walk for over a year.

---

## Pillar 4 — Artificial Intelligence & Machine Learning

**Why it exists:** The core of the degree's identity and my stated career
direction.

**Core (UMOV):**
- Introducción a la Ciencia de Datos y a la IA (already taken — LICD01)
- Aprendizaje de Máquinas (cuatr. 08), Introducción al Aprendizaje Automático
- Procesamiento del Lenguaje Natural (cuatr. 09)
- Inteligencia Artificial (cuatr. 08)
- Creatividad en los Negocios (IA para las Empresas)

**Depends on:** Pillars 1 and 2 almost entirely. I cannot meaningfully
learn ML before linear algebra, probability, and Python are in place.
This dependency is why rushing to ML now would create the exact knowledge
gaps my learning principles warn against.

**Edge:** _To be detailed as I approach this pillar (≈ cuatrimestre 6+)._
Deferred.

---

## Pillar 5 — Infrastructure, Systems & Emerging Technologies

**Why it exists:** Where systems actually run and scale. The pillar that
turns a project into a product.

**Core (UMOV):**
- Internet de las Cosas y Redes de Sensores (cuatr. 09)
- Computación Distribuida / Concurrente (shared with Pillar 2)

**Edge:** _To be detailed later._ This is where cloud, deployment, and
MLOps will live — the layer that makes the father-maintenance project
usable by someone other than me. Furthest from my current position;
detailed last.

---

## Cross-pillar dependency map

The single most important thing this document tells me — the order the
field actually requires, regardless of UMOV's scheduling:

Read: Math and Programming are the true prerequisites. Everything valuable
downstream (ML, data science, deployment) depends on them. This is why my
current focus — math intuition and programming fundamentals — is correct,
not impatience to reach the "exciting" AI parts.

---

## My current position

- **Cuatrimestre:** 1, first weeks.
- **Active pillars:** 1 (Mathematical Foundations) and 2 (Programming).
- **Everything else:** structurally mapped, intentionally not yet detailed.
  The map grows with me; it does not run ahead of me.