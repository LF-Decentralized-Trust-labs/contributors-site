[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Propose a New Top-Level Project (TLP) to LFDT

Launching a new **Top-Level Project (TLP)** at LFDT gives your community a neutral home, clear governance, and a well-defined path from **Incubation → Graduation**. This page summarizes what the Technical Advisory Council (TAC) looks for, how to prepare a proposal, and how projects are evaluated. Detailed criteria and procedures live in the governance repository and lifecycle docs. Projects may start in **LFDT Labs** and later propose for **Incubation**. The **TAC** meets regularly to review proposals and reports; decisions are recorded in public minutes and GitHub PRs.

**Important:** For any official LFDT project, entry to the formal lifecycle is only through the **Incubation** stage. The governance doc states that projects accepted by LFDT “enter the lifecycle only through the *Incubation* state,” including new proposals, Labs projects moving up, and reactivated archived projects.   That said, **[LFDT Labs](https://lf-decentralized-trust.github.io/governance/governing-documents/project-lifecycle/](https://www.lfdecentralizedtrust.org/projects/labs))** is outside the formal lifecycle —it’s a lightweight place to start work first. If/when a Lab is promoted to an official LFDT project, it then enters **Incubation**.

 
!!! tip "New here?"
    Read the **[LFDT Project Lifecycle](https://lf-decentralized-trust.github.io/governance/governing-documents/project-lifecycle/)** for the authoritative policy on stages and criteria. It also clarifies how projects can become **Dormant** or **Archived** if activity ceases.

---

## Project Proposal Requirements

Submit your proposal to the TAC using the official **Proposal Template**. 

Include [3](#2-2):

- **Clear description** of the project's purpose and goals  
- **Well-defined scope** that does not overlap existing LFDT projects  
- **Committed development resources** from multiple organizations  
- **Initial maintainers** representing diverse organizations  
- **Vendor-neutral approach** ensuring no single company controls the project

---

## Entry Criteria for Incubation

Minimum requirements to begin the lifecycle [4](#2-3):

1. **Legal Compliance** — Apache-2.0 license with proper attribution  
2. **Maintainer Diversity** — At least **2** organizations represented among maintainers  
3. **Security Standards** — Basic security policies and practices in place

---

## Technical & Community Readiness

Projects should demonstrate [5](#2-4):

- **Open source codebase** with **DCO** sign-off enforcement  
- **Multiple maintainers** from different organizations  
- **Production usage** examples or proof-of-concept implementations  
- **Community engagement plan** (public forums, regular meetings, documented process)

---

## Evaluation Process

The TAC evaluates proposals across **Legal, Diversity, Security, Releases, Testing/QA, Structure, Maintenance, Production,** and **Documentation** [6](#2-5). Inputs include **OpenSSF Scorecard** signals, **LFX Insights** activity, and **manual repository inspection**.

---

## Submission Process (TL;DR)

1. **Prepare your proposal** using the official template in the proposals repository.  
2. **Engage the community** — discuss in Discord, mailing lists, and TAC meetings.  
3. **Submit to TAC** for formal review and vote.  
4. **Meet ongoing requirements** — quarterly reports and annual reviews after acceptance.

!!! note "Best practices"
    Several successful LFDT projects (e.g., **Cacti**, **FireFly**) proved out in **LFDT Labs** before proposing for Incubation. If your idea is early-stage or experimental, consider starting in Labs to build momentum and validate scope [8](#2-7).

---

## Notes



---

## Citations

**File:** tac/governing-documents/project-lifecycle.md (L43-48)
```markdown
Projects are in one of four possible states:

- [_Incubation_](#incubation)
- [_Graduated_](#graduated)
- [_Dormant_](#dormant)
- [_Archived_](#archived)
```

**File:** tac/governing-documents/project-lifecycle.md (L60-66)
```markdown
A Proposal must:

- Have a clear description
- Have a well-defined scope
- Identify committed development resources
- Identify initial maintainers
- Be vendor neutral
```

**File:** tac/governing-documents/project-lifecycle.md (L150-159)
```markdown
The following criteria MUST be considered for each project when making one of the aforementioned decisions:
- Legal
- Diversity
- Releases
- Testing and Q/A
- Security
- Structure
- Maintenance
- Production
- Documentation
```

**File:** tac/governing-documents/project-lifecycle.md (L183-184)
```markdown
  * To be a *Graduated* project, the number of organizations from which maintainers are drawn must be at least 3, and the OpenSSF Score SHOULD be 10.
  * To be an *Incubated* project, the number of organizations from which maintainers are drawn must be at least 2.
```

**File:** tac/governing-documents/project-lifecycle.md (L242-245)
```markdown
A project accepted by the LFDT can enter the lifecycle only through the *Incubation* state. This applies to:
- New projects presented to the TAC
- Projects that were formerly *Archived* and wish to resume development activity
- LFDT Labs projects
```

**File:** tac/governing-documents/project-lifecycle.md (L247-250)
```markdown
Therefore, the qualification for a project to be accepted by the LFDT TAC and to begin its official lifecycle is the set of criteria marked (6) in the above diagram, namely:
1. Legal
2. Diversity (>=2 maintaining organizations)
3. Security
```

**File:** tac/guidelines/project-incubation-entry-considerations.md (L12-19)
```markdown
### Codebase
* Code should exist as open source software in some form. Previous accepted projects have come up through labs (e.g., Cacti, FireFly); while others previously had stand alone governance prior to joining (e.g., Besu).
* DCO sign off should be enforced in the code repository as it transitions to LFDT. Historical commits that existed in the repository before a decision to transition the project to LFDT was made do not need to be squashed, in order to preserve metadata.

### Maintainers
* The project should have multiple maintainers. These maintainers need not be from different companies; however, having maintainers from different companies is seen as a positive sign. Proposals with only one maintainer have been rejected by prior TACs.
* The project should have demonstrable examples of POC/production uses publicly available.
* The project should have the backing of more than one organization/individuals (i.e., the project proposers should be able to demonstrate significant, long term contribution in codebase).
```
