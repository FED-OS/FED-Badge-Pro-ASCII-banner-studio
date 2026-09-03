# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.1.0] – 2026-09-03

### Added
- **Four animation styles** for FED‑ETCH — choose between Cascade, Matrix Rain, Typewriter, and Reveal Wipe from the new Animation dropdown.
  - **Cascade** — lines rain down from the top and ease into their final positions (the original v3.0 style, now one of four).
  - **Matrix Rain** — individual characters fall in vertical columns with a trailing fade effect and bright white heads, evoking the classic Matrix digital rain.
  - **Typewriter** — lines are revealed character‑by‑character in sequence with a blinking blue cursor at the current position.
  - **Reveal Wipe** — a top‑down progressive curtain reveal with a glowing blue edge that sweeps downward to uncover the full tree.
- **WebM video export** — record the canvas animation directly to a `.webm` file using the MediaRecorder API and `canvas.captureStream()`. The Record button toggles between "Record WebM" and "Stop & Save", with a pulsing red indicator while recording is active.
- Animation style preference is now persisted to LocalStorage and restored on page reload.
- **GitHub community files**:
  - `CODE_OF_CONDUCT.md` — Contributor Covenant 2.1, adapted with FED‑OS enforcement contacts.
  - `ISSUE_TEMPLATE/bug_report.md` — structured bug report with environment fields.
  - `ISSUE_TEMPLATE/feature_request.md` — feature request with implementation willingness checkboxes.
  - `PULL_REQUEST_TEMPLATE.md` — PR template with type checklist, test steps, and a "no placeholder text" requirement.
  - `workflows/deploy.yml` — GitHub Pages deployment workflow using `actions/deploy-pages@v4`, triggered on push to `main`.
  - `social-preview.svg` — 1280×640 Open Graph image with gradient background, lightning icon, and feature bullets.

### Changed
- The animation engine is now a style dispatcher — `startAnimation()` reads the selected style and calls the appropriate init + animate functions.
- `loadTree()` now enables the Record WebM button alongside the other playback controls.
- `clearAll()` resets all style‑specific state (drops, matrix columns, typewriter position, reveal offset) and stops any active recording.
- The Record button has a pulsing red `@keyframes pulse-rec` animation while recording is active.

## [3.0.0] – 2026-09-02

### Added
- **FED‑ETCH ASCII Animation Studio** — a brand‑new tab that scans your local project folders and renders the file structure as animated ASCII art for README banners.
- Demo Mode with a built‑in mock repository so you can try the studio instantly, no folder upload required.
- Folder scanner using the modern `showDirectoryPicker()` API (Chrome / Edge) with a `webkitdirectory` fallback for Firefox and Safari.
- ASCII tree renderer using proper Unicode box‑drawing characters (├──, └──, │).
- Canvas‑based cascade animation engine with Play / Pause / Restart controls and an adjustable speed slider.
- Static ASCII export — copy the rendered tree to the clipboard or download it as a `.txt` file.
- Live progress bar and file counter during folder scans.
- Configurable scan limits (max files, max depth, max file size) to keep rendering fast and safe.
- LocalStorage persistence for animation speed and theme preferences.
- External stylesheet (`styles.css`) now properly linked instead of duplicated inline.

### Changed
- Restructured `index.html` to load `styles.css` externally for a cleaner, smaller markup.
- Expanded the navigation header to four tabs: Generator, Presets, ASCII Studio, Docs.
- README completely rewritten with the ASCII Studio section, real links, and no placeholders.
- CONTRIBUTING expanded with branch naming, commit conventions, and contribution areas.

### Fixed
- **License contradiction resolved** — `LICENSE` now contains the full MIT text (it previously held CC0), matching the MIT badge and `LICENSE.md`.
- Removed every remaining `YOUR_USERNAME` placeholder from presets — all preset links now point to the real FED‑OS / Fedpromptly URLs.
- CHANGELOG no longer contains malformed markdown fences or duplicated headers.
- CONTRIBUTING no longer truncated — the full workflow is now documented.

## [2.0.0] – 2026-08-23

### Added
- Full GitHub‑style UI with tabs (Generator, Presets, Docs).
- Support for all badge services: Shields.io, Badgen.net, Badges.ws, BadgeWind, Raw SVG, GitHub Actions.
- One‑click copy for HTML, Markdown, and raw output.
- Copy All (HTML and Markdown) buttons.
- Preset library with 12+ common badges.
- Built‑in documentation tab.
- Responsive design — works on all screen sizes.

### Changed
- Complete rewrite of the UI — now uses Primer‑inspired dark theme.
- Output now includes both HTML and Markdown formats for every badge.

### Fixed
- Raw SVG now correctly previews and copies the complete SVG code.
- GitHub Actions badge now generates the exact URL format that works.

## [1.0.0] – 2026-08-20

### Added
- Initial release with Shields.io and Badgen support.
- Basic input form and live preview.
- Copy‑to‑clipboard functionality.
