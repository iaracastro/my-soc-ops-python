🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops — Social Bingo for Real-Life Mixers

Turn awkward small talk into a game. Soc Ops helps groups break the ice with a fast, playful Social Bingo: find people who match prompts, complete a row, and spark real conversations.

Why it matters

- Fast onboarding for in-person events, meetups, and team socials
- Lightweight, session-backed gameplay — no accounts required
- Built with FastAPI, HTMX, and Jinja2 for snappy, server-driven UX

Highlights

- Polished Bingo mechanics with session-based game state
- Designer-friendly frontend (Jinja2 + HTMX) for progressive enhancement
- Extensible quiz/agent system used in the workshop labs

Quickstart

1. Install dependencies and sync the environment:

```bash
uv sync
```

2. Lint and run tests (recommended before changing code):

```bash
uv run ruff check .
uv run pytest
```

3. Start the development server and open your browser at http://localhost:8000:

```bash
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

Workshop & Labs

The repository is also a hands-on lab. Follow the guided parts to explore architecture and multi-agent examples:

| Part | Title |
|------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

Development Checklist

- Lint: `uv run ruff check .`
- Test: `uv run pytest`
- Run locally: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`

Contributing

Contributions, bug reports, and suggestions are welcome — see CONTRIBUTING.md for details.

License

This project is licensed under the terms in the LICENSE file.

---

> 📝 Offline lab guides are available in the `workshop/` folder.

