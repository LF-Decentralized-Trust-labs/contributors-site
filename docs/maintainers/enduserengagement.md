[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Engage End Users → Grow Contributors → Develop Future Maintainers

**Keep it simple.** Reaching out to end users doesn’t have to be daunting. Start with a short, friendly invite, give them clear first steps, and celebrate every bit of feedback. This page offers a lightweight playbook to **identify end users**, **invite them into the open**, and **help them grow** from users → contributors → (eventually) maintainers.

!!! tip "Why this matters"
    Projects with active end-user participation ship more relevant features, catch bugs earlier, attract sponsors, and build long-term maintainer pipelines.

---

## Find your end users

Start by mapping where your users already are:

- Support channels: Discord/Matrix/Slack, forums, mailing lists
- GitHub: issue authors, discussions participants, stargazers, orgs filing bugs across repos
- Events: demos, webinars, town halls, conference talks that mention your project
- Social: blog posts, case studies, LinkedIn/Twitter posts referencing your project

**Action:** create a simple list (e.g., `community/end-users.csv`) with org, point of contact, GitHub IDs, and how they use the project.

---

## Invite them into the open

Make the “front door” obvious and repeat it often.

- **Town halls & community calls:** personally invite identified users. Add a standing “End-User Update” segment.
- **Office hours:** short, predictable, and recorded.
- **Design reviews / roadmap sessions:** ask end users for a 10-minute lightning talk on their use case.
- **GitHub first:** encourage users to use their **GitHub IDs** to open issues/discussions and upvote with 👍.

**Message template (PM or email)**

```text
Subject: Invitation to share your use case + join <Project> community calls

Hi <Name>,

We saw <Org> using <Project> for <use case>. We’d love your feedback and to feature your lessons learned.
Could you:
1) Create issues with your GitHub ID for any gaps or requests (link: <issues url>)
2) Add <Org> to our ADOPTERS.md (instructions below)
3) Join our next town hall on <date/time> (<meeting link>)

Even 10 minutes of your perspective helps steer the roadmap. Thanks!
— <Maintainer>, <Project>
```

---

## Capture adoption (ADOPTERS.md)

Ask organizations to **add themselves to your project’s `ADOPTERS.md`** with a short blurb and contact. This both proves real-world usage and helps future contributors find peers.

- If your project **already has** `ADOPTERS.md`: link it prominently in `README`, issue templates, and your website.
- If your project **does not** have `ADOPTERS.md`: see LFDT guidance → **[Defining Adopters](https://github.com/LF-Decentralized-Trust/governance/blob/e85ba94202a629a83148934330183de2ee995a9a/tac/governing-documents/defining-adopters.md)**.

**Suggested `ADOPTERS.md` entry**

```markdown
## Organization: ExampleCorp
- Contact(s): @octocat (GitHub)
- Workloads: Payments ledger, tokenization service
- Scale: ~150 TPS, 20 nodes, 3 regions
- Version: v1.7.x
- Notes: Contributing connector XYZ and schema ABC in 2025Q4
```

---

## Lower the bar to first contributions

Give end users crisp, safe places to start—beyond code.

- **Issue labels:** `good first issue`, `help wanted`, `docs-needed`, `use-case / RFC`  
- **Response norm:** acknowledge new issues within 72 hours.  
- **Contribution menu:** docs fixes, tutorials, sample apps, SDK examples, benchmarks.

**Use-case RFC issue template (snippet)**

```yaml
name: Use-case RFC
body:
  - type: textarea
    attributes:
      label: Summary
      description: What you’re trying to achieve, why it matters
  - type: input
    attributes:
      label: SLO/SLI targets
      placeholder: e.g., p99 < 200ms, RPO=0, RTO < 5m
  - type: textarea
    attributes:
      label: Gaps / blockers
  - type: textarea
    attributes:
      label: Proposed contribution (code/docs/tests)
```

---

## Grow contributors → maintainers

Define an **onramp**, then a **ladder**—kept small and friendly.

- **Buddy mentoring:** pair each new end-user contributor with a maintainer for their first PR.
- **Reviewer shadowing:** invite proven contributors to shadow reviews for 2–4 weeks.
- **Module ownership:** carve out small components (docs site, SDK bindings, connectors) with clear ownership criteria.
- **Public criteria:** link to your project’s **maintainer expectations** and **promotion process** in `CONTRIBUTING.md`.

**Example growth path**

1. Add org to `ADOPTERS.md`; open issues with GitHub ID  
2. First docs/tutorial PR → first feature/bugfix PR  
3. Regular reviews; become **Reviewer** (triage+review)  
4. Own a module; become **Maintainer** (merge rights)  

---

## Measure what matters (keep it light)

Pick 2–3 indicators and publish them quarterly:

- # orgs in `ADOPTERS.md` (new vs. total)  
- # first-time PRs from end-user orgs; acceptance rate  
- Time to first maintainer response (issue/PR)

A short note in `community/quarterly-report.md` is enough—no heavy dashboards required.

---

## Quick, copy-paste block for your README

Add this snippet so end users always know the first steps:

```markdown
**Are you using <Project> in your org? Start here:**
1) Open issues with your **GitHub ID** for bugs/requests: <issues URL>  
2) Add your org to **ADOPTERS.md** (template inside): <ADOPTERS.md URL>  
3) Join our **monthly town hall**: <calendar link> (agenda & notes inside)
```

---

_Questions or improvements to this page? Open an issue/PR in the contributors-site repo and tag the maintainers of the **Maintain** section._
