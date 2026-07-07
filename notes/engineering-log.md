# Engineering Log

A running record of what I learn, what I struggle with, and the
decisions I make while building my skills as an engineer.

Format per entry: Date → What I worked on → Where I got stuck →
Key insight or decision → Next step. Kept short on purpose so the
habit survives.

---

## 2026-07-07 — Defined what this repository is (and is not)

**Worked on:** Scoping this repository and settling its architecture
before writing any real content.

**Where I got stuck:** I kept conflating two goals — using the repo as
personal memory vs. using it to impress recruiters. That single
confusion made the whole project feel directionless.

**Key decisions:**
1. This repo serves my memory. My *projects* serve recruiters. They are
   different artifacts optimizing for opposite things: the notebook wins
   by recording everything (including mistakes); a portfolio wins by
   hiding the noise and showing only polished work. One repo cannot do
   both, so I stopped trying.
2. Therefore this repo (`ai-engineering-journey`) is my notebook. Inside
   it, `projects/` is a workshop where projects are born and cooked raw.
   When a project matures (e.g. `father-maintenance-ai`), it moves to its
   own dedicated public repo — clean, documented, recruiter-facing. A
   project earns its own repo only once it exists and works, never before.

**Why this matters:** It resolves the tension that had me stuck, and it
matches how the industry actually works — recruiters browse independent
project repos, not a folder of study notes.

**Next step:** Write `learning-os/Knowledge Architecture.md` — a map of
the five pillars of my degree — so every future entry has somewhere to
connect to.

## 2026-07-07 — Built my first isolated development environment

**Worked on:** Setting up a real Python development environment from
zero: VS Code + the Python extension, a dedicated conda environment,
and running my first script inside it.

**Where I got stuck (five real obstacles, in order):**
1. `git add` silently did nothing — I had a filename case mismatch
   (`Engineering-log.md` vs `engineering-log.md`). Linux is
   case-sensitive; Windows hid the problem.
2. First commit captured an *empty* file (0 bytes). Git records
   whatever state exists — it does not validate content. Precision is
   my responsibility, not the tool's.
3. `conda activate` did nothing — conda was not hooked into PowerShell.
   Fixed once with `conda init powershell`.
4. After the hook, PowerShell blocked the conda profile script:
   execution policy disabled. Fixed with
   `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned`.
5. Editor vs terminal used different interpreters — terminal was in
   `ai-journey`, VS Code was still pointing at `base`.

**Key decisions and why:**
- **Isolated env, not `base`.** Experiments in `base` can break the
  whole Anaconda install. A dedicated env (`ai-journey`) is a sandbox:
  break it without consequences elsewhere.
- **Python 3.11, not 3.13.** In data science, "newest" ≠ "most stable".
  Libraries lag behind new Python releases. 3.11 is mature and widely
  supported. Stability over recency.
- **`RemoteSigned` + `CurrentUser` scope.** Least privilege: allow my
  own local scripts, still block unsigned scripts from the internet,
  and change policy only for my user — no admin rights, no system-wide
  change. Open only what the problem requires.
- **Env lives on `D:`** (`D:\conda_envs\ai-journey`) because `C:` is
  nearly full. Data science envs are multi-GB; disk planning matters.

**Recurring lesson:** The machine is literal. Four of five obstacles
were tools doing exactly what I said, not what I meant — and staying
silent about it. Verify against evidence; never assume. My first
program proves this: it prints its own interpreter path to *demonstrate*
which env it runs in rather than trusting it.

**Next step:** Begin Cisco Python Essentials 1 (Week 1 of the roadmap):
variables, data types, input/output. Build something tiny that runs.