[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Operations Playbook

Day‑to‑day repository and release operations.

## Common Repository Structure

```
/docs
/security
/governance
/.github
  ├─ ISSUE_TEMPLATE/
  ├─ PULL_REQUEST_TEMPLATE.md
  └─ workflows/
/cmd or /src
```
- OWNERS/maintainers mapping per repo or directory.
- Clear README with quickstart and support links.

## CI/CD Requirements

- Required checks (lint, tests, build, license scan).
- Reproducible builds where feasible.
- Artifact storage with retention and immutability.

## Release Taxonomy & Cadence

- **SemVer**: major for breaking changes, minor for features, patch for fixes.
- Pre‑release tags for RC/beta; document upgrade notes and migration steps.
- Maintain a **release checklist** (see Templates).

## Project Updates & Annual Review

- Publish periodic **project updates** (milestones, roadmap, risks, needs).
- Prepare an **Annual Review** with governance/ops status, adoption metrics, and roadmap proposals.

## Checklists

- [ ] Repo structure aligned
- [ ] Required CI checks enforced
- [ ] Release checklist documented
- [ ] Update/Annual Review process linked
