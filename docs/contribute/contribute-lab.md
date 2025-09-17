[//]: # (SPDX-License-Identifier: CC-BY-4.0)

## Why Propose a New Project as an LFDT Lab

LFDT Labs is the fastest way to start and grow an open-source idea under vendor-neutral stewardship. By proposing a Lab, you get a lightweight home for your code—public repo, basic governance, and community visibility—without the overhead of a full top-level project. Labs invite early adopters and maintainers to test, give feedback, and co-develop roadmaps, while you benefit from standard practices (Apache-2.0, DCO) and shared community infrastructure. As your project matures, the Labs path provides a clear runway toward the formal LFDT lifecycle (Incubation → Graduation). If you want momentum, mentorship, and a credible neutral umbrella from day one, proposing a Lab is the right move.

## How to Contribute a New Project as an LFDT Lab

### Understanding LFDT Labs
LFDT Labs serves as an experimental space for new projects before they potentially enter the formal LFDT project lifecycle [1](#1-0) . Previous successful projects like Cacti and FireFly have come through labs before becoming official LFDT projects [2](#1-1) .

### Key Requirements for Labs Projects
LFDT Labs keeps barriers low, but proposals still need a few essentials so collaborators can engage from day one. Below are the baseline requirements reviewers look for to confirm the project is legally clean, minimally documented, and has committed maintainers with a clear scope.<br>
 
 Your project should have:
   - Open source codebase with clear licensing
   - Basic documentation
   - Initial maintainer commitment
   - Defined scope and objectives

### Transition Path to Full LFDT Projects
Labs projects that mature can transition to the formal LFDT lifecycle through the Incubation state [4](#1-3) . To qualify for this transition, projects must meet entry criteria including:

- Legal compliance (Apache 2 licensing) [5](#1-4) 
- Maintainer diversity (≥2 organizations) [6](#1-5) 
- Basic security practices [7](#1-6) 

### Next Steps
1. Prepare your project proposal with clear description, scope, and committed resources
2. Engage with the LFDT community through Discord or mailing lists
3. Submit your proposal for TAC review
4. Work toward meeting the criteria for eventual transition to Incubation if desired

<cite />

---

## Official LFDT Labs Proposal Process (from LFDT Labs README)

Follow these steps to propose a **new Lab** using the LFDT Labs website repository:

1. **Fork** the `lf-decentralized-trust-labs.github.io` repository.
2. **Fill out the Proposal Template** and save it under the `labs/` subdirectory as `<your-lab-name>.md` (e.g., `mynewlab.md`). Your **lab repository is expected to use the same name**, so choose carefully.  
   - **Naming rule:** A Lab **cannot** be named after a product, network, or any existing entity. Open source code should have a distinct identity separate from any product or service. If you pick a product/service name now, you will need to change it later.
3. **(Optional) Find a sponsor** to help connect your proposal to the broader LFDT community and validate novelty/scope.  
   Ways to find sponsors:  
   - Ask maintainers of related projects via your existing connections.  
   - Pitch to related working groups or projects in their channels/mailing lists.  
   - Use the `MAINTAINERS` file in repos to find contacts and/or post to the Maintainers list.  
4. **Commit with DCO sign-off.** Include a line like:  
   `Signed-off-by: Your Name <you@example.com>`  
   Use `git commit -s` to add it automatically (or `git commit --amend -s`).
5. **Open a Pull Request.**
6. **Wait for Labs stewards review.** Stewards check that proposals are **cogent and novel**. Stewards and sponsors are not obligated to maintain your Lab code; their review role is limited to proposal evaluation.

### Bringing in an existing repository
- By default, stewards create a **new repository** for your Lab.  
- If you want to **reuse an existing GitHub repository**, you may request that option **only if every commit is DCO-signed**.  
- If not all commits are signed, **squash** history into a single initial commit in the new Lab repo **with your sign-off**.

### License requirement
All LFDT software (including Labs) must use the **Apache 2.0** license. License all incoming and new code accordingly and ensure **all commits are DCO-signed**.

### Code of Conduct
All LFDT community members must follow the **Code of Conduct**.

---

## Notes

The governance repository contains extensive documentation about the formal project lifecycle but lacks specific Labs contribution processes. The TAC meeting minutes indicate recent changes to Labs approval processes, but detailed procedures would likely be found in Labs-specific repositories or documentation that I don't have access to.

Wiki pages you might want to explore:
- [Project Management (LF-Decentralized-Trust/governance)](/wiki/LF-Decentralized-Trust/governance#3)
- [Meeting Archive (LF-Decentralized-Trust/governance)](/wiki/LF-Decentralized-Trust/governance#6.2)

### Citations

**File:** tac/governing-documents/project-lifecycle.md (L242-246)
```markdown
A project accepted by the LFDT can enter the lifecycle only through the *Incubation* state. This applies to:
- New projects presented to the TAC
- Projects that were formerly *Archived* and wish to resume development activity
- LFDT Labs projects

```

**File:** tac/governing-documents/project-lifecycle.md (L247-251)
```markdown
Therefore, the qualification for a project to be accepted by the LFDT TAC and to begin its official lifecycle is the set of criteria marked (6) in the above diagram, namely:
1. Legal
2. Diversity (>=2 maintaining organizations)
3. Security

```

**File:** tac/guidelines/project-incubation-entry-considerations.md (L13-13)
```markdown
* Code should exist as open source software in some form. Previous accepted projects have come up through labs (e.g., Cacti, FireFly); while others previously had stand alone governance prior to joining (e.g., Besu).
```

**File:** tac/meeting-minutes/2025/2025-08-28.md (L13-13)
```markdown
- [TAC members can approve lab proposals vote has passed](https://lists.lfdecentralizedtrust.org/g/tac/topic/114818893#msg4140).
```
