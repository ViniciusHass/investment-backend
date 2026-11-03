# Backend agent instructions

The owner performs initial scaffolding. FastAPI, Python, uv, SQLAlchemy, Alembic and PostgreSQL are planned. Follow Factory specs and API contracts; write tests for all business rules. Keep market-data adapters behind interfaces, preserve source provenance, do not invent data. Never merge to main or modify the frontend repository. Request approval for major architectural changes.

Write code and configuration comments in English.
For each approved implementation, create a separate branch and worktree from `develop`; open a PR targeting `develop` after tests and review. The owner alone approves and performs merges.
