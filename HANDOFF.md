# Project Continuity & Working State: Infomity Studio Website (`infomity.github.io`)

## Project Overview
- **Domain & Repository**: `https://infomity.github.io/` hosted at `E:\hissain\github\infomity.github.io` (branch `main`).
- **Purpose**: Official corporate studio and product showcase website for Infomity. Features live flagship Google Play applications, privacy policies, open-source AI tooling, scientific libraries, and threat intelligence systems.
- **Brand Identity**: Obsidian dark aesthetic, zero telemetry, edge-native compute, complete user sovereignty, zero ads/trackers.

## Current Status
- **Bengal Keyboard**: Live on Google Play (`com.infomity.banglakeyboard`, v1.0.49+).
  - Play Store URL: `https://play.google.com/store/apps/details?id=com.infomity.banglakeyboard`
  - Showcase: `https://infomity.github.io/bangla-keyboard/`
  - Privacy Policy: `https://infomity.github.io/bangla-keyboard/privacy/`
- **Remogent**: Live on Google Play (`io.github.infomity.remogent`, v0.1.70 Production; v0.1.91+ in Play Store review / Internal Testing, Companion `0.2.26`).
  - Play Store URL: `https://play.google.com/store/apps/details?id=io.github.infomity.remogent`
  - Showcase: `https://infomity.github.io/remogent/`
  - Privacy Policy: `https://infomity.github.io/remogent/privacy/`
- **Deployment State**: Live on GitHub Pages (`origin/main` commit `eaff896`, `status: "built"`).

## In-Flight / Active Tasks
- None.

## Important Decisions & Constraints
- **Alignment & Visual Harmony**: All pages (`index.html`, `bangla-keyboard/index.html`, `remogent/index.html`) follow 1:1 centered hero layouts (`max-width: 860px; margin: 2rem auto; text-align: center;`), centered status pills, centered CTAs, centered section headers (`max-width: 680px; margin: 0 auto 3rem auto;`), and centered card headers/icons-above-titles and descriptions (`.feature-card-header`, `.feature-card-icon`, `.feature-card-desc`, `.app-header-block`, `.metric-card`, setup & FAQ cards).
- **Direct Play Store Links**: Both showcase pages (`bangla-keyboard/index.html` and `remogent/index.html`) feature direct "Get it on Google Play" glow buttons with official SVG play icons pointing to verified app package IDs.
- **Cross-App Navigation**: Unified top navbar and footer links cross-reference between Home, Apps Catalog, Bangla Keyboard, and Remogent across all pages.
- **Compliance & Store URLs**: Both product pages serve as the official Play Console Support / App Website URLs and contain direct links to their dedicated, compliant privacy policies.
- **Static & Dependency-Free**: Pure HTML5/CSS3/Vanilla JS with zero external tracking SDKs. Theme preference saved in `localStorage`.

## Technical Context & Code Map
- `index.html`: Studio hub page with interactive software catalog, hero showcase buttons, and telemetry metrics.
- `bangla-keyboard/index.html`: Bengali phonetic keyboard product showcase with interactive simulated QWERTY input and Google Play link.
- `bangla-keyboard/privacy/index.html` & `privacy.txt`: Standalone privacy policy satisfying Google Play requirements.
- `remogent/index.html`: AI terminal agent client showcase with 3-step setup guide and Google Play link.
- `remogent/privacy/index.html` & `privacy.txt`: Standalone privacy policy detailing zero telemetry, direct P2P connection, and push notifications.
- `privacy/index.html`: Studio-wide privacy charter linking to both application-specific disclosures.
- `assets/css/style.css`: Unified ZeBeyond / Obsidian dark theme styling.

## Validation
- Verified HTML markup integrity across `index.html`, `remogent/index.html`, and `bangla-keyboard/index.html` with Python `HTMLParser` after final edits.
- Verified live GitHub Pages deployment (`commit eaff896`, `status: "built"`) and `HTTP 200` responses for `/`, `/remogent/`, `/bangla-keyboard/`, and `/assets/css/style.css`.

## Next Actions / Open Items
1. **Post-Approval Privacy Policy & Showcase Update (Remogent)**:
   - Once Google Play approves the pending Remogent version (`v0.1.91+`), review `remogent/privacy/index.html` and `remogent/privacy/privacy.txt` for any updates required by the new features (e.g., Antigravity CLI `agy`, local `/proxy/:port/*` web preview, workspace file browser, notification biometric overlay, 8 MB session cap) and proceed accordingly.
   - Update `remogent/index.html` to promote the `#coming-soon` items to live features once approved on Production.
