# ZEN Credential Card Style Vault

This repository stores **HTML-only prototypes** of ZEN credential cards—visual shells for the badges, levels, and achievements used across the ZEN ecosystem:

- **ZEN AI Pioneer Program** (youth AI literacy, 1st in U.S. history)
- **ZEN Vanguard** (professional / adult track)
- **AI Homeschool Kit**
- **Blockchain Literacy tracks**
- Future **ZEN Card**–based credentials and collectible badges

Each `.html` file is a fully self-contained, displayable card layout. These are **front-end style experiments**, not live credential data. Later, real program data (name, level, XP, wallet, etc.) will be injected into these shells by ZEN’s credentialing pipeline.

---

## What’s in here now

- `*.html` files, each representing a **single ZEN Card layout**.
- Every file:
  - Is a **complete HTML document** (`<html>`, `<head>`, `<body>`).
  - Includes **all CSS inline** (usually via `<style>` in the `<head>`).
  - Centers one tall “card” UI on screen (desktop-friendly).
  - Uses placeholder values like `ALEX PIONEER`, levels, stats, etc.

> **Important:** These HTML files are treated as **design artifacts / reference styles**, not production components. They will inform the final credential renderer and blockchain-minted ZEN Card designs.

---

## How to view a card

1. Clone the repo.
2. Open any `*.html` file in a browser (double-click or `Open With → Browser`).
3. Inspect / tweak styles locally as needed.

No build step, no bundler—each card is standalone.

---

## How to add a new card (human workflow)

1. Create a **new** HTML file (do not overwrite an existing one).
2. Use a descriptive filename, for example:

   - `zen-bio-labs-level-5.html`
   - `zen-technomancer-class-x.html`
   - `zen-neural-runner-class-s.html`

3. Ensure the file is:
   - A **complete, valid HTML document**.
   - Visually centered, with a single vertical card.
   - Using **only inline CSS** (no external frameworks, fonts, or scripts).
4. Commit the new file:

   ```bash
   git add your-new-file.html
   git commit -m "Add new ZEN card style: <short description>"
