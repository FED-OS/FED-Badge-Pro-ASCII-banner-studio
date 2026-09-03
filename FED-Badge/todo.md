# FED-Badge v3.1 Upgrade — Master Plan

## Phase 1: Fix & Polish Core Files (DONE in v3.0)
- [x] Fix LICENSE contradiction
- [x] Remove placeholders, rewrite CONTRIBUTING/CHANGELOG/README
- [x] External styles.css
- [x] FED-ETCH ASCII Studio (Demo Mode, scanner, cascade animation, export)

## Phase 2: GitHub Community Files (v3.1)
- [x] Create .github/CODE_OF_CONDUCT.md
- [x] Create .github/ISSUE_TEMPLATE/bug_report.md
- [x] Create .github/ISSUE_TEMPLATE/feature_request.md
- [x] Create .github/PULL_REQUEST_TEMPLATE.md
- [x] Create .github/workflows/deploy.yml (GitHub Pages deploy)
- [x] Create social-preview.svg (1280x640 OG image)

## Phase 3: Upgrade FED-ETCH — Multiple Animation Styles (v3.1)
- [x] Add animation style selector (Cascade, Matrix, Typewriter, Reveal)
- [x] Implement Matrix rain style
- [x] Implement Typewriter style (line-by-line reveal)
- [x] Implement Reveal style (top-down wipe)
- [x] Rewrite animate() dispatcher
- [x] Add animStyleSel change handler + localStorage persistence

## Phase 4: WebM Video Export (v3.1)
- [x] Add "Record WebM" button using MediaRecorder + canvas.captureStream
- [x] Start/stop recording with button toggle
- [x] Download as .webm after stop
- [x] Enable recordBtn in loadTree()
- [x] Add recording pulse animation CSS

## Phase 5: Polish & Finalize
- [x] Browser-test all 4 animation styles
- [x] Update README + CHANGELOG for v3.1
- [x] Repackage zip
