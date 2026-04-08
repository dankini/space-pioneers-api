# Claude Code Guidelines

## Project Overview

This is the Space Pioneers API - a Django-based API for tracking human spaceflight data including missions, astronauts, agencies, and EVAs.

## Git Conventions

Follow the standards in [CONTRIBUTING.md](CONTRIBUTING.md) for branch naming, commit messages, and PR process.

- **Before committing**: Always ask whether to commit to main or create a branch, and include a recommendation based on the change type

## Tech Stack

- Python / Django
- Docker for containerization
- PostgreSQL database

## Code Standards

- PEP 8 style guide
- 4 spaces indentation (Python)
- 88 character line length (Black formatter)
- 2 spaces indentation (HTML templates)
- Prefer class-based views over function-based views

## Django Guidelines

- Always include migrations in the same commit as model changes
- Never run `migrate` automatically — flag migrations for the user to review first
- Ask before adding new dependencies

## Testing

Run tests before committing: `docker-compose exec web python manage.py test`
