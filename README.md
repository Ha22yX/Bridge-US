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

## Why This Exists

New international students often rely on scattered chats and social posts for housing, transportation, safety, and first-week logistics. Bridge US v1 is a small moderated prototype for organizing that advice into searchable sections.

## Workflow

- Students browse practical posts by section.
- Registered users submit experience-based posts.
- New submissions enter a review queue before becoming public.
- Approved posts form a simple trust-oriented knowledge base.
- The project acts as the early product prototype before the V2 rebuild.

## Features

- Section-based feed for first-week, housing, food, transit, life admin, and safety posts.
- Registration, login, post submission, and admin review queue.
- Approved-only public content for basic moderation.
- Chinese/English direction for international-student scenarios.

## Quickstart

```bash
git clone https://github.com/Ha22yX/Bridge-US.git
cd Bridge-US
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Open `http://127.0.0.1:5000`. This v1 repo is intentionally simpler than V2.

## Tech Stack

| Layer | Technology | Role |
| --- | --- | --- |
| Backend | Flask | Routes, templates, and sessions. |
| Data | SQLite | Local app database for prototype content. |
| i18n | Flask-Babel | Bilingual UI direction. |
| Frontend | Jinja, CSS | Server-rendered community pages. |

## Project Map

```text
app.py                  Flask application
db.py                   database helpers
templates/              community and admin pages
static/                 CSS and static assets
docs/                   product planning notes and screenshot
```

## Notes

[Bridge-US](https://github.com/Ha22yX/Bridge-US) and [Bridge-US-V2](https://github.com/Ha22yX/Bridge-US-V2) target the same product idea but are independent projects. V1 is the early/simple Flask prototype; V2 is the fuller React/FastAPI rebuild.
