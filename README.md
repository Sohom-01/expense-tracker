# Spendly — Expense Tracker

A personal finance tracker built with Flask. Log expenses, understand your spending patterns, and take control of your finances — one transaction at a time.

> **Status:** Work in progress. The landing, login, and register pages are in place; authentication, the database layer, and expense management are being built step by step.

## Tech Stack

- **Backend:** Python, Flask
- **Database:** SQLite
- **Frontend:** Jinja2 templates, HTML, CSS, JavaScript
- **Testing:** pytest, pytest-flask

## Project Structure

```
expense-tracker/
├── app.py              # Flask app and routes
├── database/
│   └── db.py           # SQLite connection, schema, and seed data
├── static/
│   ├── css/style.css
│   └── js/main.js
├── templates/          # Jinja2 templates (base, landing, login, register)
└── requirements.txt
```

## Getting Started

### Prerequisites

- Python 3.9+

### Setup

```bash
git clone https://github.com/Sohom-01/expense-tracker.git
cd expense-tracker

python -m venv venv

# Windows (PowerShell)
venv\Scripts\Activate.ps1
# macOS / Linux / Git Bash
source venv/bin/activate        # Git Bash on Windows: source venv/Scripts/activate

pip install -r requirements.txt
```

### Run

```bash
python app.py
```

Then open [http://127.0.0.1:5001](http://127.0.0.1:5001).

### Test

```bash
pytest
```

## Roadmap

- [x] Landing, login, and register pages
- [ ] Database setup (schema + seed data)
- [ ] User registration and login
- [ ] Logout
- [ ] User profile page
- [ ] Add expenses
- [ ] Edit expenses
- [ ] Delete expenses
