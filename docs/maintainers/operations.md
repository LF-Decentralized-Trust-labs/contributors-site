[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Maintainer's Operations Playbook

!!! Welcome
    Practical guidance for day‑to‑day repository and release operations.

<div class="grid cards" markdown>

- :material-folder-cog:{ .lg .middle } __Common Repository Structure__

  ---

  `docs/`, `security/`, `governance/`, `.github/` templates, OWNERS/maintainers mapping.

- :material-robot-confused:{ .lg .middle } __CI/CD Requirements__

  ---

  Required checks (lint, test, build), reproducible builds, artifact storage and retention.

- :material-tag:{ .lg .middle } __Release Taxonomy & Cadence__

  ---

  SemVer, pre-releases, migration notes, LTS decisions, checklists.

- :material-chart-timeline-variant:{ .lg .middle } __Project Updates & Annual Review__

  ---

  What to report to the TAC, metrics, deadlines, and exemplars.

</div>

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
