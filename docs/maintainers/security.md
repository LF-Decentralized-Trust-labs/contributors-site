[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Security Playbook

!!! Welcome
    Ship verifiably secure releases and respond quickly to vulnerabilities. This page covers policy, release integrity, CI, and response.

## Security Policy (SECURITY.md)

  Private contact, PGP key, embargo flow, supported versions, backport policy.

- **Contact:** security@… and PGP key (optional)
- **Embargo:** intake → triage → coordinated fix → disclosure
- **Support:** list supported versions and backport windows

## Release Integrity

  SemVer, signed artifacts (cosign/GPG), provenance (SLSA), and SBOM per release.

- **SemVer** with clear pre-releases (alpha/beta/rc)
- **Signing** (cosign/GPG) for all artifacts; publish **provenance** (SLSA-aligned)
- **SBOM** per release attached to artifacts

## CI / Protections

  Branch protection, required checks, Scorecards in CI, dependency update policy.

- Branch protection: required reviews & checks; consider signed commits
- **OpenSSF Scorecard** in CI; track checks like token permissions & pinned deps
- Regular dependency updates; avoid unreviewed auto-merges

## Vulnerability Response

  Triage in 48h; fix/mitigation in 7–14 days; private coordination; advisories.

- Triage within **48 hours**; guidance/fix within **7–14 days** by severity
- Coordinate with downstreams prior to disclosure
- Publish advisories and changelog entries

## Supply-Chain Hygiene

- Pin build deps; aim for reproducible builds
- Restrict GitHub Actions tokens & use trusted, reusable workflows
- Avoid fetching unpinned scripts/binaries at build time

## Checklists

- [ ] SECURITY.md with contact + embargo
- [ ] Signed releases + provenance + SBOM
- [ ] Scorecard CI in place
- [ ] Vulnerability response runbook documented

---

### Related

- [Operations](operations.md) · [Templates](templates.md) · [SLSA Guidelines](https://lf-decentralized-trust.github.io/governance/guidelines/slsa-guidelines/)
