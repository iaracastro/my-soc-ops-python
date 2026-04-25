# Soc Ops - Social Bingo Game

## Development Checklist
Before committing or deploying:
- [ ] **Lint**: `uv run ruff check .` (Fix any style issues)
- [ ] **Test**: `uv run pytest` (Ensure all tests pass)
- [ ] **Run**: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000` (Verify app starts)

## Code Style
- Python 3.13+ with type hints
- Ruff for linting (E, F, I, N, W rules)
- Line length: 88 chars
- Use `uv` for dependency management

## Architecture
- **Backend**: FastAPI with session-based game state
- **Frontend**: HTMX for dynamic interactions, Jinja2 templates
- **Game Logic**: Bingo mechanics in `game_logic.py`, sessions in `game_service.py`
- **Models**: Pydantic models in `models.py`

## Build and Test
- Install: `uv sync`
- Test: `uv run pytest`
- Lint: `uv run ruff check .`
- Run dev server: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`

## Conventions
- HTMX requires full browser (not VS Code Simple Browser) for functionality
- Session middleware for game persistence
- Static files served from `/static/`

See `workshop/` for detailed lab guides and `docs/` for documentation.