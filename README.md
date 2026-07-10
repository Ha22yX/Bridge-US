<div align="center">
  <h1>Bridge US</h1>
  <p>An early Flask community prototype for international students sharing practical U.S. arrival knowledge.</p>

  <p>
    <a href="README.zh-CN.md">Chinese</a>
    &middot;
    <a href="https://github.com/Ha22yX/Bridge-US-V2">Bridge-US V2</a>
    &middot;
    <a href="#quickstart">Quickstart</a>
    &middot;
    <a href="#features">Features</a>
    &middot;
    <a href="#tech-stack">Tech Stack</a>
  </p>

  <p>
    <img alt="Python: Flask" src="https://img.shields.io/badge/Python-Flask-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img alt="Community: prototype" src="https://img.shields.io/badge/Community-prototype-287866?style=for-the-badge" />
    <img alt="Version: v1" src="https://img.shields.io/badge/Version-v1-6b7f73?style=for-the-badge" />
  </p>
</div>

<p align="center">
  <img src=".github/assets/readme-hero.svg" alt="Bridge US overview image" width="100%" />
</p>

<p align="center">
  <img src="docs/pic/image.png" alt="Bridge US prototype screenshot" width="100%" />
</p>

## Overview

Bridge US v1 is the first practical prototype of the international-student community idea.

It is intentionally simple: server-rendered pages, a SQLite-backed content flow, and a review queue for approved public posts.

## Features

- Section-based practical posts for arrival, housing, transit, food, life admin, and safety topics.
- Registration/login flow, post submission, and admin review queue.
- Approved-only public content for a basic trust workflow.
- Product-planning docs and screenshot retained in `docs/`.
- Clear relationship to Bridge-US-V2 as the more complete independent rebuild.

## How It Works

1. Users browse practical posts by category.
2. Registered users submit posts from their own experience.
3. Admins review new submissions before publication.
4. The repo documents the early product direction before the V2 rewrite.

## Quickstart

Run the project locally with the commands below.

```bash
git clone https://github.com/Ha22yX/Bridge-US.git
cd Bridge-US
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Open `http://127.0.0.1:5000`. Use this repo as the v1 prototype; use V2 for the fuller product architecture.

## Configuration

| Item | Purpose |
| --- | --- |
| `SECRET_KEY` | Set for Flask sessions before deployment. |
| SQLite database | Local prototype storage; back it up before real use. |
| Admin review | Use the review queue to keep public content controlled. |
| V2 migration | Treat new feature work as a reason to inspect Bridge-US-V2 first. |

## Tech Stack

| Layer | Technology | Role |
| --- | --- | --- |
| Backend | Flask | Routes, templates, and sessions. |
| Data | SQLite | Prototype database. |
| Frontend | Jinja, CSS | Server-rendered community pages. |
| Docs | Markdown | Product planning and roadmap notes. |

## Project Layout

```text
app.py                  Flask application
db.py                   database helpers
templates/              community and admin pages
static/                 CSS and static assets
docs/                   planning notes and screenshot
```

## Status

Early prototype. Bridge-US and Bridge-US-V2 target the same product idea but are independent projects; V2 is more complete.

## Related Projects

- [Bridge-US V2](https://github.com/Ha22yX/Bridge-US-V2) - companion/version reference.

## License

No project-wide open-source license has been declared yet.
