# Roadmap — Weeks 01 to 12

## Purpose

UMOV does not gate my progress: no assignments, no projects, only videos
and multiple-choice exams. Therefore **this roadmap is my forcing
function.** The structure that a normal school imposes from outside, I
impose on myself from here. If this document is ignored, nothing external
will catch the failure — so it will not be ignored.

## Planning principle: rolling-wave

Near weeks are detailed; far weeks are directional. What I do in week 8
depends on how weeks 1–3 went. This plan is re-elaborated as I learn, not
written once and obeyed blindly.

## Time budget (honest)

- **Target:** ~20–25 h/week (weekdays, replacing former gaming downtime).
- **Floor (bad week):** ~10 h/week — enough to keep momentum alive.
- **Weekends:** rest by default. Study only to recover a short week.
  Rest is scheduled, not stolen. Sustainable pace requires it.
- **Micro-gaps at work (3–5 min):** review channel only — re-reading
  notes, spaced repetition. Not for new programming or math.

## Definition of "done" per week (non-negotiable)

Every week must produce:
1. At least one commit to this repo.
2. At least one `engineering-log.md` entry.

This is the accountability UMOV does not provide. Weeks without both did
not happen.

---

## Phase 1 — Weeks 1–3: Python foundations + solidify tooling (DETAILED)

**Anchor resource:** Cisco Python Essentials 1 (free via UMOV/NetAcad,
gives a certificate → also feeds `career/`). This answers my earlier
question about whether to use the Cisco courses: yes, as the spine here.

Active pillars: 2 (Programming), with 1 (Math) as a light parallel track.

### Week 1 — Environment + first steps
- Confirm Python is installed; install VS Code Python extension.
- Create and activate a virtual environment (`venv`) — first real use of
  an Edge skill. Commit a `hello.py`.
- Cisco PE1: intro, variables, data types, basic input/output.
- Output: one small script committed. One log entry.

### Week 2 — Control flow + first useful program
- Cisco PE1: conditionals and loops.
- Build one tiny program that takes input and produces output (e.g. a
  unit converter). Commit it.
- Output: working script committed. One log entry.

### Week 3 — Functions + basic data structures
- Cisco PE1: functions, lists, tuples, dictionaries.
- Refactor the week-2 script to use functions. Goal: feel *why* functions
  exist — reusable tools, not repeated code. (Connects to my "build tools
  to reuse" mindset.)
- Output: refactored script committed. One log entry.

---

## Phase 2 — Weeks 4–6: Python for real data (DIRECTIONAL)

- Reading and writing files; working with structured data (CSV first,
  then Excel via a library like openpyxl/pandas — introduced when needed,
  not before).
- Problem decomposition: breaking a task into small solvable pieces.
- First contact with the *shape* of my father's data (what columns, what
  calculation is done by hand today).
- Re-detail these weeks at the end of week 3.

## Phase 3 — Weeks 7–9: Father project — vertical slice v0.1 (DIRECTIONAL)

- Build the **smallest possible thing that does one real thing**: read one
  Excel sheet, automate the ONE calculation currently done manually.
- Not a full app. A vertical slice — the engineering discipline of proving
  one end-to-end path before broadening. Crude is fine; working is the bar.

## Phase 4 — Weeks 10–12: Harden + reassess (DIRECTIONAL)

- Handle a second case; add basic structure; write a README for the slice.
- Re-plan the *next* 12 weeks based on what actually happened.

---

## Parallel light track — Math (all 12 weeks)

~2–3 short sessions/week (not daily), supporting UMOV's Cálculo /Álgebra,
intuition-first. Log only when something clicks or blocks. Heavy math
(linear algebra for ML) deepens later, per the dependency map — not forced
now.

## Current sprint

**Weeks 1–3.** Everything past week 3 is intentionally coarse and will be
elaborated as I go.