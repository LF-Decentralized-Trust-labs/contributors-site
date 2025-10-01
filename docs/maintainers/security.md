[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Security Playbook

Ship verifiably secure releases and respond quickly to vulnerabilities.

## Security Policy (SECURITY.md)

- Provide a **private contact** (security@…) and PGP key if available.
- Define an **embargo process**, acknowledgement timeline, and disclosure expectations.
- State supported versions and how fixes are backported.

## Release Integrity

- Use **SemVer** with clear pre‑releases.
- Sign artifacts (e.g., **cosign**, GPG) and publish **provenance** (SLSA‑aligned).
- Generate **SBOM** per release and store with artifacts.

## CI / Protections

- Branch protection: required reviews, status checks, and signed commits if used.
- Run **OpenSSF Scorecard** in CI; track key checks (pinned dependencies, token permissions).
- Regular dependency updates; avoid unreviewed auto‑merges.

## Vulnerability Response

- Triage within **48 hours**, fix or mitigation guidance within **7–14 days** depending on severity.
- Coordinate with downstreams before public disclosure.
- Publish advisories (e.g., GitHub Security Advisories) and changelog entries.

## Supply‑Chain Hygiene

- Pin versions for build deps; prefer reproducible builds.
- Restrict GitHub Actions tokens to least privilege; use reusable, trusted workflows.
- Avoid downloading binaries/scripts at build time from unpinned URLs.

## Checklists

- [ ] SECURITY.md with contact + embargo
- [ ] Signed releases + provenance + SBOM
- [ ] Scorecard CI in place
- [ ] Vulnerability response runbook documented
