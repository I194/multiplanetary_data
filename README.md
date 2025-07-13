# Multiplanetary Data

Open-source knowledge base for **multiplanetary life** — agriculture, engineering, habitat design, space medicine, psychology and every other discipline required to settle new worlds.
All articles feed directly into the content pipeline for **[multiplanetarization.com](https://www.multiplanetarization.com/)**, an independent project tracking humanity’s progress toward living on multiple planets.

Every contribution is a standalone article stored as Markdown plus local media inside the `articles/` directory.

## Repository Layout

```text
articles/
  my-article-slug/
    article.md
    cover.jpg|png|webp
    optional-media.*
```

## Writing an Article

1. Create a new folder inside `articles/` named after your topic in *kebab-case* (lowercase words separated by hyphens).
2. Add an `article.md` file that follows the front-matter schema below.
3. Place a `cover` image in the same folder and reference it from the front matter (`cover: cover.jpg`).
4. Commit, push, and open a Pull Request (PR) against `main`.

### Front Matter Schema

```yaml
---
title: Your Article Title               # Required
date: YYYY-MM-DD                        # ISO-8601, UTC
description: One-sentence abstract      # ≤120 characters
importance: 1–10                        # Subjective priority
cover: cover.jpg                        # File present in folder
---
```

### Front Matter Fields Explained

| Field      | Purpose |
|------------|---------|
| `title`    | Article headline shown on multiplanetarization.com |
| `date`     | Publication date (ISO-8601) used for sorting |
| `description` | Concise abstract for previews/meta tags |
| `importance` | Editorial priority **1 (low) – 10 (top)**; higher numbers surface sooner on the homepage |
| `cover`    | Local image file displayed as the article banner |

### Recommended Markdown Skeleton

```markdown
# <Title – Optional Subtitle>

<!-- Optional: replace the list below with your own key points -->
## Why <Topic> (optional)

- Point 1  <!-- example placeholder -->
- Point 2
- Point 3

---

## Key Section Heading

Your content here. Use additional sections (`##`, `###`, …) as needed.

---

## References

- List sources, links, spreadsheets, videos, etc.
```

### Style Guide

* Plain Markdown only; avoid raw HTML except the occasional `<br>` if you really need a line break.
* Use local images (`![alt](image.png)`) rather than external links so that the repo stays self-contained.
* Keep each image **≤ 1 MB** — this is mandatory both for quick page loads on multiplanetarization.com and for a lightweight repository.
* Prefer tables for numeric data or comparisons.
* Keep line length ≤120 characters to ease diff reviews.
* Cite your sources – science is better with references.
* To embed a full-width **YouTube** video, put the URL on its own line with no Markdown formatting (e.g. `https://www.youtube.com/watch?v=dQw4w9WgXcQ`). Most Markdown engines will auto-embed it.

## Contributing Workflow

1. Fork this repository and create a topic branch:
   ```bash
   git checkout -b my-new-article
   ```
2. Add your article and commit your changes.
3. Push the branch and open a Pull Request to `main`.

I ([@i194wisp](https://x.com/i194wisp)) review every PR live and leave feedback.
During review you will receive one of three labels:

| Label            | Meaning                                                      |
|------------------|--------------------------------------------------------------|
| 🟢 **Accepted**     | Looks great – will be merged as-is.                          |
| 🟡 **Needs Changes**| Please address the review comments and push an update.       |
| 🔴 **Rejected**     | Topic is out of scope or has major issues; no merge planned. |

I aim to review every submission within **72 hours**.

## License (CC-BY-4.0)

This repository uses the **Creative Commons Attribution 4.0 International** license.
In short, you can **share** and **adapt** the material—even commercially—**as long as** you give proper credit.

Key points:

* **Share** — copy and redistribute the material in any medium or format.
* **Adapt** — remix, transform and build upon the material for any purpose, including commercial.
* **Attribution required** — you must give appropriate credit, link to the license and indicate if changes were made.
* **No additional restrictions** — you may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

There are **no warranties**. Use the information at your own risk.

Full legal text: <https://creativecommons.org/licenses/by/4.0/>

By submitting a Pull Request you agree to license your contribution under these same CC-BY-4.0 terms so that the entire knowledge base stays compatible.