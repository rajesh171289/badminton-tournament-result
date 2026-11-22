# Project memory

## Product intent & audience

- Single-page static website presenting tournament data with division-based navigation.
- Intended for public sharing via a hosted link.

## Brand personality & voice

- Not yet inferred beyond straightforward, informational presentation of tournament content.

## Visual design & UX direction

- Existing design is treated as canonical; preserve as-is.
- Self-contained single `index.html`: all CSS, data, and interactivity are inline.
- Includes responsive behavior for mobile and print layouts; must remain unchanged.
- Division navigation pattern is part of the current UX and should not be altered.

## Decisions, constraints & rationale

- Site must run as a static site with `index.html` as the entry point; no build-step-dependent app logic inside the HTML.
- Minimal Vite config + package file added solely so the preview and Bolt can serve/publish the static site; not meant to change the page itself.
- Production build confirmed clean with everything intact.
- Deployment target: default Bolt-hosted `bolt.host` URL; no custom domain configuration.
- Core constraints from user: keep current design, tournament data, navigation, and responsive behavior unchanged.

## Open questions & assumptions

- Assumption: no backend or dynamic data is needed; tournament data is static and lives in `index.html`.
- Assumption: future edits should still avoid breaking the self-contained single-file structure unless explicitly requested.
- Open: brand/voice guidance not provided; revisit if styling or copy changes are requested.