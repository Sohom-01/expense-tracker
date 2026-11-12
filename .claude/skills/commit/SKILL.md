---
name: commit
description: Stage the current change and commit it to main using this repo's `area: description` message style.
disable-model-invocation: true
---

Commit the current working-tree changes following this repo's conventions.

1. Run `git status` and `git diff` to see what changed. Check `git log --oneline -5` for the message style.
2. Keep it to one logical change per commit. If the diff mixes unrelated changes, stage and commit them separately.
3. Stage files by name. Never stage `venv/`, `*.db`, `.env` or `__pycache__/`.
4. Write a one-line message in the form `area: description`, all lowercase, imperative (e.g. `landing: add privacy policy page and route`, `db: add get_db helper`). Use the page or module as the area.
5. Commit directly to `main`. Do not push unless asked.
