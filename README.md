# Cash CI Gallery

Visual test gallery for UI and E2E test recordings from Cash iOS Buildkite builds.

→ [View Gallery](https://priip.github.io/cash-ci-gallery)

## ✨ Features

- Search and filter by name, module, team, type, or status ([ownership mapping](https://docs.google.com/spreadsheets/d/1u3hNvS6JQiBt9_ORCuZaR8IdUxvO-5-AV9utG_cyD9Y/edit?gid=457260210#gid=457260210))
- View test cards with GIF previews, failure analysis, and navigation between recordings

## 🧪 Current Process (Experimental)

This is a **proof of concept** to validate whether a visual test gallery is useful. The workflow is intentionally simple and mostly manual. The goal is to gather feedback.

**How it works:**
1. Buildkite on-demand job records GIFs for UI/E2E tests
2. Local extraction script downloads artifacts and generates test data JSON
3. Static HTML gallery displays GIFs with search and filtering

## 🤔 Open Questions

- How to automate the extraction and publishing pipeline? (possible integration with [#actionable-ci-results](https://www.notion.so/square-seller/Actionable-CI-Results-Home-go-actionable-ci-docs-27d70293beed80919ca8ccc7b897d739))
- Where to store GIFs (500MB+ per build) and how long to retain them?
- When to run: nightly, per release, or on-demand?
- How to optimize: smaller GIFs, MP4s, or frame-by-frame screenshots?