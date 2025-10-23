[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Maintainer's Operations Playbook

!!! Welcome
    Practical guidance for day‑to‑day repository and release operations.

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
- OWNERS/maintainers mapping per repo or directory
- README with quickstart + support links

## CI/CD Requirements

- Required checks (lint, tests, build, license scan)
- Reproducible builds where feasible
- Artifact storage with retention and immutability

## Release Taxonomy & Cadence

- **SemVer**: major=breaking, minor=features, patch=fixes
- Pre-release tags for RC/beta; document upgrade notes & migrations
- Maintain a **release checklist** (see Templates)

## Project Updates & Annual Review

- Publish periodic **project updates** (milestones, roadmap, risks, needs)
- Prepare **Annual Review**: governance/ops status, adoption metrics, roadmap proposals

## Checklists

- [ ] Repo structure aligned
- [ ] Required CI checks enforced
- [ ] Release checklist documented
- [ ] Update/Annual Review process linked

---

### Related

- [Security](security.md) · [Governance](governance.md) · [Templates](templates.md)
