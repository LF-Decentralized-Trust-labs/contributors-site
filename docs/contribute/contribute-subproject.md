[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Contribute a New Subproject to an Existing LFDT Top-Level Project

This guide explains how to propose and integrate a **new subproject** under an existing LFDT **Top-Level Project (TLP)**. It combines LFDT-wide governance expectations with project-specific practices so your subproject can mature, align with the parent TLP, and deliver value to the ecosystem.

!!! tip "New here?"
    If your idea is early-stage, consider starting in **LFDT Labs** for a lightweight, low-friction launch. Labs lets you build community, harden the codebase, and validate scope before a formal proposal to a TLP.

---

## Recommended Entry Path: **Labs First**

**Why start in Labs?**  
For subprojects without maintainer diversity, open-source history, or a stable community, **LFDT Labs** is the ideal first step. Labs offers a low-barrier space for community exploration and development before formal lifecycle entry.

**Benefits of the Labs approach**
- **Community building:** time to attract contributors and diversify maintainers.  
- **Experience development:** learn LFDT processes and open source governance norms.  
- **Risk mitigation:** address common rejection factors before a formal TLP proposal.

---

## Core Requirements for Subproject Integration

### Essential prerequisites

**Legal compliance**
- Apache-2.0 license compatibility.  
- Trademark clearance for naming.  
- DCO sign-off enforcement on all commits.

**Maintainer diversity**
- Multiple maintainers from **at least two organizations**.  
- Demonstrable long-term contribution commitments.  
- Evidence of production or POC usage where possible.

**Community foundation**
- More than one sponsor across different organizations.  
- Public technical discussions and a community engagement plan (e.g., Discord, mailing lists, regular calls).  
- Willingness to meet LFDT reporting expectations.

### Technical standards

**Repository structure & docs**
- Follow the LFDT common repository structure.  
- Include `SECURITY.md` with reporting process, plus user/dev/app-dev docs.  

**Quality assurance**
- CI configured (build, tests, scans).  
- Unit/integration test coverage with documented status.  
- OpenSSF Scorecard enabled for security signals.

---

## Integration Process

### 1) Pre-integration assessment

**Evaluate alignment**
- Avoid significant overlap with existing TLP components.  
- Clearly state the distinct advantage your subproject brings.  
- Show architectural compatibility with the TLP.

**Community preparation**
- Discuss the idea in TLP channels and public forums.  
- Engage TLP maintainers and stakeholders early.  
- Ensure all proposal materials are publicly accessible.

### 2) Formal proposal

**Submit for review**
- Use the official proposal template referenced by the TLP/TAC.  
- Include purpose, scope, committed resources, and initial maintainers.  
- Demonstrate vendor-neutral governance and community support.

**Evaluation signals**
- Lifecycle criteria across legal, diversity, security, releases, testing/QA, structure, maintenance, production, documentation.  
- OpenSSF Scorecard & LFX Insights, plus manual repo inspection.  
- Community feedback and discussion period.

### 3) Post-approval integration

**Repository & governance setup**
- Create or migrate under the LFDT GitHub org within the TLP namespace.  
- Add required files (`LICENSE`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `CONTRIBUTING`, `MAINTAINERS`, `README`).  
- Connect to TLP automation (CI, release process, issue labels) and community channels.

**Ongoing compliance**
- Provide quarterly/annual updates as required.  
- Participate in TLP and TAC review cycles.  
- Maintain diversity and engagement standards as the subproject grows.

---

## TLP-Specific Considerations

**Each TLP may add local requirements**, such as:
- Technical architecture reviews for compatibility with the TLP roadmap.  
- Participation in project-specific governance bodies or working groups.  
- Release coordination (versioning, cadence, artifact signing).  
- Documentation standards (site structure, style guides).

**Best practices**
- Engage early and often with TLP maintainers.  
- Join community calls and design discussions; contribute to existing modules to demonstrate commitment.  
- Articulate unique value, provide adoption signals, and align your roadmap with TLP strategy.

---

## Success Factors & Common Pitfalls

**Critical success factors**
- Maintainer diversity (avoid single-maintainer proposals).  
- Visible community readiness (public design, roadmap, regular meetings).  
- Clean legal posture (license, DCO, trademarks).

**Common pitfalls**
- Overlap with existing components without clear differentiation.  
- Weak organizational backing or unclear resourcing.  
- Copyleft/GPL or patent encumbrances blocking Apache-2.0 compatibility.

---

## Submission checklist

- [ ] Apache-2.0-compatible codebase with DCO enforced  
- [ ] `LICENSE`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `CONTRIBUTING`, `MAINTAINERS`, `README`  
- [ ] Multiple maintainers from **≥ 2** orgs; sponsors identified  
- [ ] CI + tests + basic security scans; OpenSSF Scorecard enabled  
- [ ] Public roadmap & engagement plan; discussion with TLP maintainers  
- [ ] Clear differentiation from existing TLP scope and architecture  
- [ ] Proposal doc ready (purpose, scope, resourcing, governance)

---

## Notes

LFDT governance provides the baseline expectations for any addition to the ecosystem, while each TLP can tailor integration details to fit its architecture and release machinery. Labs is a great on-ramp if your subproject needs time to grow community and operational maturity before formal integration.
