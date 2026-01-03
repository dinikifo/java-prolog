# MiniPrologProto Collection (Java)

This repository is a **collection of small subprojects** built around a compact Java-based Prolog-style resolution engine (unification + backtracking). Depending on the subproject, it adds:

- an embedded **column-oriented database** (two variants: *no joins* vs *join-capable*)
- an **HTN (Hierarchical Task Network) action planner**
- a **JSON-AIML dialect chatbot** plus a **dataset editor** (Swing)
- a **Toulmin argumentation expert system** (forward/backward reasoning) with a Swing UI

Each folder is intended to be runnable on its own via the included `build.sh` / `demo.sh` / `selftest.sh` scripts.

---

## Repo layout

- `gui.prolog.no.join/prolog_real_final/`
  - Prolog core + REPL
  - Column DB **without joins**
  - HTN planner

- `prolog_with_join/`
  - Prolog core + REPL
  - Column DB **with joins** (JSON join specification)
  - Join docs: `README_JSON_JOINS.md`
  - Extra documentation: `Manual_Tutorial.pdf`

- `aiml/`
  - JSON-AIML dialect chatbot + dataset editor (Swing)
  - Main UI entrypoint: `com.mycompany.prolog.JsonAimlStudioMain`

- `toulmin/`
  - Toulmin argument expert system with forward/backward reasoning
  - Swing UI entrypoint: `com.mycompany.prolog.ToulminExpertSystemUI`

---

## Requirements

- **Java 17+** recommended
- **Python 3.10+** only if you want the optional IDE front-end (where included)
- **PyQt6** only for `prolog_ide.py`


---

## License

Public domain under **The Unlicense** (see `LICENSE.md`).
