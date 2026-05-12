# AGENTS.md - madfaker

## Purpose

`madfaker` is a tiny fake-data repo used for testing against legacy MAD-shaped REST data without hitting the real system.

## Role in micro-dkp

- Provides a lightweight mock data source for local or experimental development.
- Supports testing and prototyping around the legacy MAD domain.
- Is a support utility, not a source of truth for production business rules.

## Key layout

- `db.json` is the main mock data store.

## Working agreement

- Keep the data small, explicit, and disposable.
- Prefer representative fixtures over trying to mirror the full production schema here.
- If a test fixture starts encoding real business logic, move that logic back to the owning service or a more intentional test harness.
