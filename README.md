# Abrupt vs Gradual Shifts: Rate Factors (Innovation Summit 2025)

This repository hosts the public website, shared code, and collaboration notes for **Innovation Summit 2025 — Group 3**. Our sprint focuses on comparing ecosystem rate factors that drive **abrupt** versus **gradual** changes, with the goal of producing rapid visualizations, a concise brief, and reusable workflows that decision makers can explore after the event.

The project site is published with MkDocs at **https://cu-esiil.github.io/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/**. Every commit to the `docs/` folder rebuilds the site automatically via GitHub Actions.

---

## Repository layout

| Path | Purpose |
| --- | --- |
| `code/` | Analysis scripts, notebooks, and supporting utilities developed during the sprint. |
| `docs/` | Source files for the public website, including the homepage, updates, and resource guides. |
| `documentation/` | Internal planning notes and extended write-ups that do not belong on the public site. |
| `containers/` | Definitions for reproducible container images that support repeatable analyses. |
| `workflows/` | Automation and CI/CD configuration, including the MkDocs deployment workflow. |

Large datasets should live in the team’s CyVerse folder instead of this repo. Link to them from `docs/data.md` or relevant analysis notes.

---

## Getting started

### Update the website

1. Open the [`docs/`](docs/) directory and choose the page you want to edit (for example [`docs/index.md`](docs/index.md)).
2. Click the ✏️ icon in GitHub or edit locally, then describe your change in a short commit message.
3. Commit directly to `main`. The MkDocs workflow rebuilds the site automatically—refresh the public link after a minute.

Helpful pages to customize early:
- **Homepage:** [`docs/index.md`](docs/index.md) — add your current questions, visuals, and call to action.
- **Project template:** [`docs/project_template.md`](docs/project_template.md) — adjust the front-matter fields to match Group 3.
- **Persistent storage guide:** [`docs/instructions/save-to-persistent-storage.md`](docs/instructions/save-to-persistent-storage.md) — confirm the CyVerse path matches your team.

### Share and run code

- Store runnable scripts and notebooks in [`code/`](code/). Add brief headers describing inputs, outputs, and how to execute each workflow.
- Reference important files from [`docs/code.md`](docs/code.md) once analyses begin.
- Use the [`containers/`](containers/) and [`requirements.txt`](requirements.txt) scaffolding if you need reproducible environments.

### Connect with shared storage

Group 3’s CyVerse community folder lives at:
```
https://de.cyverse.org/data/ds/iplant/home/shared/esiil/Innovation_summit/Group_3/
```
Use the GoCommands workflow in [`docs/instructions/save-to-persistent-storage.md`](docs/instructions/save-to-persistent-storage.md) for uploads and downloads.

---

## GitHub Pages deployment

1. Pages is configured to deploy with the **Deploy site (MkDocs)** workflow in `.github/workflows/deploy.yaml`.
2. If workflows are disabled, enable them from the **Actions** tab.
3. To trigger a rebuild manually, visit **Actions → Deploy site (MkDocs) → Run workflow** targeting `main`.

---

## Contributing

- Work on small, frequent commits so the team can track progress easily.
- When editing in the browser, keep notes concise and emphasize visuals that tell the day’s story.
- Use issues or the project Slack channel to coordinate changes before demo time.

---

## Citation

If you reuse the materials here, cite the project using [`CITATION.cff`](CITATION.cff) or the preferred format for your publication.
