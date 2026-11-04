# Data, at Scale

**A weekly research brief on one question:** does scaling training data always improve deep-learning model performance?

Read the [live GitHub Pages newsletter](https://tripathiswastik.github.io/Weekly-data-scaling-newsletter/).

## What the page includes

- A featured research story designed for a three-minute read
- A bulleted breakdown of practical takeaways
- Linked research, developer-community insights, and production lessons
- Short research quotes and an interactive multiple-choice reader question
- A weekly issue number, edition date, and next-issue date in Asia/Kolkata time

The feature story focuses on the quality-versus-quantity tradeoff in language-model pretraining. Findings are linked to their original sources, and practical recommendations are identified as inference where appropriate.

## Weekly publishing

The newsletter is scheduled for Mondays at 11:00 AM IST. The page calculates its issue number from the first edition date in `index.html` (currently November 2, 2026) and updates the issue and next-Monday labels in the browser.

GitHub Pages hosts the site and GitHub Actions deploys changes pushed to `main`. The scheduled newsletter and the website content are separate: a new weekly issue must be researched and added to `index.html`; GitHub Pages does not generate or replace article content on its own.

## Publish with GitHub Pages

1. Open the repository’s **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Save. The workflow at `.github/workflows/pages.yml` deploys on a push to `main` or a manual workflow run.

## Update an issue

1. Replace the featured story, source links, and bulleted breakdown in `index.html`.
2. Refresh the supporting stories, quotes, and reader quiz so they match that issue.
3. If the first-edition date changes, update the issue-number baseline in the page script.
4. Commit the change to `main`; GitHub Actions publishes the updated page.

## Files

- `index.html` — responsive single-page newsletter, styles, issue counter, and quiz interaction
- `.github/workflows/pages.yml` — GitHub Pages deployment workflow

There are no build dependencies; the page is plain HTML, CSS, and JavaScript.
