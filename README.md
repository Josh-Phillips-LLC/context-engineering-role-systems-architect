# context-engineering-role-systems-architect

Role-specific agent workspace for **Systems Architect**.

This repository is generated from templates and role definitions in `Context-Engineering`.

## Purpose

- Provide a role-scoped default repo for IDE agents and role-based workstation containers.
- Keep role instructions self-contained for tools that read repo-root instruction files.

## Managed Files

These files are generated artifacts and should not be manually edited:

- `AGENTS.md`
- `.github/copilot-instructions.md`
- `.vscode/settings.json`

Instruction model:

- `AGENTS.md` is the canonical compiled role instruction set.
- `.github/copilot-instructions.md` is an adapter that points to `AGENTS.md`.

## Source of Truth

Canonical role definitions and governance live in `Context-Engineering`:

- `10-templates/job-description-spec/global.json`
- `10-templates/job-description-spec/roles/systems-architect.json`
- `10-templates/agent-instructions/base.md`
- `10-templates/agent-instructions/roles/systems-architect.md`
- `00-os/role-charters/systems-architect.md`
- `governance.md`

For `compliance-officer`, generated instructions also embed:

- `10-templates/compliance-officer-pr-review-brief.md`

## Regeneration

Regenerate this repository from `Context-Engineering` using:

```bash
10-templates/repo-starters/role-repo-template/scripts/render-role-repo-template.sh \
  --role-slug systems-architect \
  --repo-name context-engineering-role-systems-architect \
  --output-dir <path-to-role-repo>
```

## Generation Metadata

- Source ref: `bea1f47`
- Generated at (UTC): `2026-02-13T18:07:03Z`
