# RINGFORGE // NEXUS v3

Mission-control HUD that showcases RINGFORGE as the **truth layer** on top
of verified Ring Developer capabilities. It embeds contract facts only —
Capability Matrix v1, Scope / Endpoint / Device registries v1 — and never
invents Ring APIs.

## Truth model (shown in the app)

- **RING DOCUMENTATION FACT** — from the embedded matrix, last verified
  2026-09-10.
- **RING SOURCE FACT (runtime)** — UNAVAILABLE until Partner OAuth is
  linked. The app does not pretend to have live data.
- **RINGFORGE DERIVED** — correlation computed from the embedded facts.
- **AI INTERPRETATION** — labeled as interpretation, not fact.
- **MOCK ADAPTER** — live-looking telemetry is explicitly mock.

## Live probe (opt-in only)

The default mode is MOCK: the app makes no network calls at all. The
Source Gate panel can probe a local sidecar (`http://127.0.0.1:8787`) or,
in DIRECT mode with a token the user pastes in, the Ring Partner API.
Nothing is fetched unless the user switches modes and provides a token.
The token is kept in sessionStorage only.

## Panels

1. Property topology (force graph of device families)
2. Capability matrix explorer
3. Event bus + temporal/graph correlation
4. Scope / OAuth + private-app limit conflict
5. Endpoint registry
6. Truth HUD / HIRE readout

## Keyboard

`/` search · `Esc` close inspector/search · `1`–`6` switch panels ·
`Space` pause/resume event bus.

## Why v3

Three RingForge files were found in the archive: v1.0.0 (`RINGFORGE.html`,
also shipped in `RINGFORGE-nexus-module-v1.0.0.zip`), v1.0.1 HUD
(CSS layout fixes only), and v3 (this file — restyled shell, boot screen,
Source Gate probe panel, data version 3.0.0). v3 is the newest and most
complete build, so it is the one staged here. The module zip's own icon
(`icon.svg`, the hex/ring mark) is kept as `icons/nexus-sigil.svg`.

## Files

- `index.html` — the v3 app, single file (Google Fonts loaded from CDN)
- `manifest.webmanifest` / `manifest.json` — PWA manifest (page links
  the `.webmanifest`)
- `icons/` — custom icon set plus the original hex/ring `nexus-sigil.svg`
