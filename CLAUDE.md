# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Spendly: a Flask + SQLite expense tracker with Jinja2 templates, plain CSS and vanilla JS. It is built step by step from a tutorial.

## Commands

- Setup: `python -m venv venv`, activate it (PowerShell `venv\Scripts\Activate.ps1`, Git Bash `source venv/Scripts/activate`), then `pip install -r requirements.txt`.
- Run: `python app.py` (debug on, port **5001**, not Flask's default 5000).
- Test: `pytest` (pytest and pytest-flask are installed, but no tests exist yet).
- No linter, formatter or CI is configured.

## Rules

- Vanilla JS only. No JS libraries, frameworks or new dependencies.
- Keep edits minimal. Do not modify unrelated parts of a page or file.
- Database: raw `sqlite3` only, no ORM. `database/db.py` provides `get_db()` (sets `row_factory`, enables foreign keys), `init_db()` (`CREATE TABLE IF NOT EXISTS`) and `seed_db()`. The DB file is `expense_tracker.db` (gitignored).
- Stub routes in `app.py` (`/logout`, `/profile`, `/expenses/add`, `/expenses/<id>/edit`, `/expenses/<id>/delete`) are future tutorial steps. Implement only the step requested and leave other stubs untouched.

## Gotchas

- `landing.html` uses `static/css/landing.css`. The other pages extend `base.html` and use `static/css/style.css`.
- `file.txt` is a log of prompts and commit messages, not project code.

## Git

- Commit directly to `main`, one change per commit, message format `area: description` in lowercase (e.g. `landing: add privacy policy page and route`).
