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

## Notes

-


## AI-Assisted Creation & Provenance

Some parts of this repository were created or refined with the assistance of large language models (LLMs) at the author’s direction. The author reviewed and integrated the results.

The intent is to place this work as completely as possible into the public domain (see the License ).

If you believe any snippet inadvertently reproduces third-party copyrighted code in a way that conflicts with the license, please open an issue with details (file, lines, source link). We will promptly rewrite or remove the material.

Privacy note: Don’t paste sensitive or proprietary material into issues or pull requests; treat prompts/logs as public.

---

## License

Public domain under **The Unlicense** (see `LICENSE.md`).
