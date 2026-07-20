# Contributing

Thanks for your interest in contributing to oleander skills.

## Who can contribute

Contributions from external contributors are welcome.

## How to contribute

1. Fork the repository.
2. Create a branch for your change.
3. Add or update skills under `skills/<skill-name>/`.
4. Open a pull request with:
   - what changed
   - why it changed
   - any usage examples

## Skill layout

Each skill lives in its own directory:

```
skills/<skill-name>/
├── SKILL.md         # Required — frontmatter + instructions
└── metadata.json    # Required — name + semver version
```

Optional: `scripts/`, `references/`, or `assets/` for progressive disclosure.

### `SKILL.md` frontmatter

Required fields:

| Field | Rules |
| --- | --- |
| `name` | Lowercase letters, numbers, hyphens; must match the directory name |
| `description` | Third person; include **what** the skill does and **when** to use it (trigger terms) |

Example:

```yaml
---
name: lake-query
description: >-
  Routes lake SQL by scanned data size. Use when querying oleander lake
  tables or choosing between DuckDB and Spark SQL.
---
```

### `metadata.json`

Keep in sync with the skill name and bump the version when behavior changes:

```json
{
  "name": "lake-query",
  "version": "0.1.0"
}
```

## Validate before opening a PR

```bash
npx skills-ref validate skills/<skill-name>
```

## Review and approval policy

- All contributions require review.
- A contribution is considered approved and official only after an oleander employee approves and merges the pull request.

## Style guidance

- Keep `oleander` lowercase.
- Keep instructions concrete and reproducible.
- Prefer concise, testable guidance over broad theory.
- Keep `SKILL.md` under 500 lines; move detail into `references/` when needed.
- Do not reference files that are not committed in this repository.
