# GlobalDrive 2026/27 – Internet of Logistics

Project website of the GlobalDrive 2026/27 student research project (TUM, KTH and industry partners).

The whole website is one file: `index.html` (HTML, CSS and JavaScript in one place, no build step).

## View the website

- **Live:** once GitHub Pages is enabled, the site is at https://thomaswallner99.github.io/globaldrive-2026/
- **Locally:** download or clone the repo and open `index.html` in your browser.

## How we work together

`main` is the version everyone sees. Nobody edits `main` directly – every change goes through a branch and a pull request.

1. **Create a branch** for your change, named after what you do, e.g. `theses/thomas-abstract` or `ecosystem/interfaces`.
   - On github.com: branch dropdown → type a new name → *Create branch*.
   - With git: `git checkout -b theses/thomas-abstract`
2. **Make your change** in `index.html` (on github.com: open the file → pencil icon; or locally in any editor, or with Claude).
3. **Commit** with a short message saying what changed, e.g. `Add abstract for shared dispatch platform`.
4. **Open a pull request** into `main` and add one teammate as reviewer.
5. The reviewer checks it (open the file from the branch or download it and look at it in the browser) and **merges** it.
6. GitHub Pages updates the live site automatically after the merge (takes about a minute).

### Rules of thumb

- Keep pull requests small and focused – one topic per PR. Small PRs rarely collide.
- Before you start, pull the latest `main` (`git pull`) or create your branch fresh from `main`.
- If two people need to change the same section, agree in the team chat who does it.
- Bigger design ideas: make a separate branch (e.g. `design/new-ecosystem-layout`) so everyone can compare before merging.
- Every version is kept in the history – nothing is lost, and any change can be reverted.

## Where to edit what

All content lives in `index.html`:

| Section | What to change | Where in the file |
|---|---|---|
| Research Gap, Learnings, Project & People | Text | HTML sections `id="research-gap"`, `id="learnings"`, `id="people"` |
| Layer model (L1–L6) | Layer names, descriptions, bullet lists | JavaScript `const LAYERS=[…]` |
| How the layers interact | Cards, flows between layers, regulatory arrows | JavaScript block `// ---- layer interaction map` (`const L=[…]`, `const F={…}`) |
| Theses | Title, description, method, layers | JavaScript `const THESES=[…]` |
| Team | Names | JavaScript `const PEOPLE=[…]` |
