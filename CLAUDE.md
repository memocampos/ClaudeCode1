# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Environment

- Python 3.11 via `.venv/` (created by PyCharm)
- Activate: `source .venv/bin/activate`

## Projects

### findme_jobs/

Flask landing page for findme.jobs.

```bash
cd findme_jobs
pip install -r requirements.txt
python app.py          # runs on http://localhost:8080
```

**Note:** macOS AirPlay Receiver occupies port 5000 — the app is configured to use 8080.

Structure:
- `app.py` — single `GET /` route rendering `templates/index.html`
- `templates/index.html` — full landing page (10 sections, Jinja2)
- `static/css/style.css` — all styles, CSS custom properties, responsive
- `static/js/main.js` — nav scroll class toggle + Intersection Observer for entrance animations
