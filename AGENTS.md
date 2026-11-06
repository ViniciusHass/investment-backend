# Backend agent instructions

The owner performs initial scaffolding. FastAPI, Python, uv, SQLAlchemy, Alembic and PostgreSQL are planned. Follow Factory specs and API contracts; write tests for all business rules. Keep market-data adapters behind interfaces, preserve source provenance, do not invent data. Never merge to main or modify the frontend repository. Request approval for major architectural changes.

Target Python 3.14 for new backend code, its container and CI, even when using Python 3.12-compatible syntax. The owner controls the initial `pyproject.toml` and lockfile.

Write code and configuration comments in English.
For each approved implementation, create a separate branch and worktree from `develop`; open a PR targeting `develop` after tests and review. The owner alone approves and performs merges.
Make subsequent commits atomic: one coherent change per commit, with a Conventional Commit subject. Agent-authored commits use `Codex <codex@users.noreply.github.com>` without changing the owner's global Git identity. Keep already published commits unchanged. Plan SemVer releases in a later approved card; do not create version tags automatically.
