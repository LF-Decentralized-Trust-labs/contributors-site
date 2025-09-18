[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Contributor Site Contribution Guide

This contributor website lives in **LF-Decentralized-Trust-labs/contributors-site** and is published via GitHub Pages. You can edit pages directly on GitHub or work locally with MkDocs (Material theme).

- Repo: `https://github.com/LF-Decentralized-Trust-labs/contributors-site`
- Published site: `https://lf-decentralized-trust-labs.github.io/contributors-site/`
- License: **CC BY 4.0** (see `LICENSE`)

---

## Quick Start (edit in GitHub)

!!! tip "Fastest path"
    1. Open the page under `docs/` you want to change and click **Edit** (✏️) on GitHub.  
    2. Make your Markdown edits, write a clear commit message, and open a **Pull Request (PR)**.  
    3. After review, merging the PR republishes the site to GitHub Pages.

If you’re **adding a new page**, see **Add a New Page** and **Update the Sidebar Navigation** below.

---

## Full Workflow (local preview)

1. **Clone the repo**
   ```bash
   git clone https://github.com/LF-Decentralized-Trust-labs/contributors-site.git
   cd contributors-site
   ```

2. **Create a branch**
   ```bash
   git checkout -b docs/your-change
   ```

3. **Install docs tooling** (uses repo’s pinned dependencies)
   ```bash
   pip install -r requirements.txt
   ```

4. **Run a local server**
   ```bash
   mkdocs serve
   ```
   Preview at **http://127.0.0.1:8000** with live reload.

5. **Commit & push**
   ```bash
   git add .
   git commit -m "docs: update site content"
   git push -u origin docs/your-change
   ```

6. **Open a Pull Request** on GitHub for review.

---

## Repository Layout (what to expect)

```
contributors-site/
├─ docs/
│  ├─ index.md
│  ├─ about.md
│  ├─ projects.md
│  ├─ contribute/
│  │  ├─ index.md
│  │  ├─ end-users.md
│  │  └─ guide.md      ← (this file, if you place it here)
│  ├─ maintain/
│  │  └─ index.md
│  └─ mentorship/
│     └─ index.md
├─ mkdocs.yml
├─ requirements.txt
└─ .github/
   └─ workflows/
```

- All content must live under `docs/`.
- Images: put in `docs/assets/images/` and link relatively.
- Downloads/templates: `docs/assets/downloads/`.

---

## Add a New Page

1. **Create the file** under `docs/`, e.g.:
   ```
   docs/contribute/how-to-add-pages.md
   ```

2. **Add a title** at the top:
   ```markdown
   # How to Add Pages
   ```

3. **Wire it into the sidebar** (next section).

---

## Update the Sidebar Navigation

MkDocs shows only pages listed under `nav:` in `mkdocs.yml`. Edit `mkdocs.yml` and add your page where it fits:

```yaml
site_name: LF Decentralized Trust

nav:
  - Home: index.md
  - About: about.md
  - Contribute:
      - Overview: contribute/index.md
      - End Users: contribute/end-users.md
      - Website Guide: contribute/guide.md     # ← add your page here
  - Maintain:
      - Overview: maintain/index.md
  - Mentorship:
      - Overview: mentorship/index.md
  - Projects: projects.md
```

**Path tips**
- Paths in `nav:` are **relative to `docs/`**.
- `about.md` and `about/index.md` are both valid (the latter renders at `/about/`).
- After editing `mkdocs.yml`, restart `mkdocs serve`.

---

## Linking Between Pages (relative links)

With `use_directory_urls: true` (default), `projects.md` renders at `/projects/`.  
- From `docs/projects.md` to `docs/end-users.md` (sibling): `../contribute/end-users/`  
- From `docs/contribute/index.md` to `docs/about.md`: `../about/`  
- Same folder: `./another-page/` or `another-page.md`

**Examples**
```markdown
See the [End Users](../contribute/end-users/) guide.
Read more [About](../about/).
```

---

## Components & Patterns (Material)

Admonitions:
```markdown
!!! tip "Helpful Tip"
    Short, actionable guidance for the reader.
```

Buttons:
```markdown
[Open an Issue](https://github.com/LF-Decentralized-Trust-labs/contributors-site/issues/new){ .md-button .md-button--primary }
```

Cards grid:
```markdown
<div class="grid cards" markdown>

- :octicons-project-symlink-16:{ .lg .middle } __[Contribute](./index.md)__
- :fontawesome-solid-circle-info:{ .lg .middle } __[About](../about.md)__

</div>
```

Images & downloads:
```markdown
![Alt text](../assets/images/example.png)
[Download template](../assets/downloads/template.docx)
```

---

## Style & Content Guidelines

- Be **task-focused** and concise; use headings and lists.
- Use **sentence case** for headings (except proper nouns).
- Link to **source repos**, specs, or further reading.
- Prefer **examples** and short code blocks over long prose.
- Keep relative links so previews and subpath hosting work.

---

## PR Checklist

- [ ] Builds locally with `mkdocs serve` (no 404s, no console errors).
- [ ] `mkdocs.yml` updated if you added a page.
- [ ] Relative links verified (hover in local preview).
- [ ] Images live under `docs/assets/images/` and are referenced relatively.
- [ ] Clear commit message and PR description.

---

## Troubleshooting

**My page doesn’t show in the sidebar**  
- Add it under `nav:` in `mkdocs.yml` and restart `mkdocs serve`.

**A link points to the wrong place**  
- From a subpage, `./end-users.md` resolves under the current folder.  
- Go up one: `../end-users/` (or `../end-users.md`).

**Local preview shows 404**  
- Check filename and `nav:` path.  
- Ensure the file is under `docs/`.  
- Restart `mkdocs serve` after editing `mkdocs.yml`.

---

## Optional mkdocs.yml Enhancements

Add repository and “Edit this page” links:

```yaml
repo_name: LFDT Contributors Site
repo_url: https://github.com/LF-Decentralized-Trust-labs/contributors-site
edit_uri: edit/main/docs/
theme:
  name: material
  features:
    - content.action.edit
    - navigation.sections
    - navigation.path
```

---

## Reference

- Official MkDocs documentation: **https://www.mkdocs.org/**
