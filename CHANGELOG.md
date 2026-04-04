# Changelog — Auracelle Orion · Public Use Demo

All notable changes to this simulation are documented here.  
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [0.4.0] - 2026-04-04

### Added
- **Nuclear Cybersecurity domain** — three new scenarios with full 5-turn lifecycle each:
  - `SAFEGUARD ZERO` (IAEA Safeguards-class) — cyberattack on nuclear facility safeguards monitoring disabling IAEA verification data feeds; w_IFD=0.60 · λ=0.25
  - `FISSION GATE` (Stuxnet-class) — centrifuge control system compromise via grey-market USB and PLC ladder logic modification at uranium enrichment facility; w_IFD=0.50 · λ=0.20
  - `YELLOWCAKE RUN` (Supply-chain mineral attack) — cyber-enabled falsification of nuclear material transport authentication via shared rare earth logistics platform; w_IFD=0.35 · λ=0.18
- **Nuclear-specific stressors** — `NUC-VERIFY`, `NUC-CTRL`, `SC-PROVENANCE`, `IAEA-ITDB`, `OT-ENRICH`, `CHAIN-AUTH`
- **Nuclear governance frameworks** — IAEA CSA Article 77, Additional Protocol, CPPNM, NPT normative provisions modelled across scenario options
- **Domain-coloured scenario navigation** — AI scenarios accent in amber (`#e8a444`); Nuclear scenarios accent in red (`#e05555`); section labels, prefix spans, and button left-border accents all domain-coded
- **Domain section dividers** in left nav — "AI Cybersecurity" and "Nuclear Cybersecurity" group headers with coloured section borders
- **Scenario prefix labels** — `AI ·` and `NUCLEAR ·` tags above each scenario name in the navigation panel

### Fixed
- **Tooltip portal system** — replaced CSS-only `position:absolute` tooltip approach with a JavaScript portal that teleports tooltip content to `document.body` on `mouseenter`; resolves clipping caused by `overflow:hidden` and `overflow-y:auto` on `.lnav`, `.rpanel`, and `.gboard` containers
- **Tooltip direction** — portal auto-detects available viewport space and opens left or right accordingly; right-panel tooltips always open leftward; left-nav domain health tooltips open rightward with full z-index clearance
- **`MutationObserver`** re-attaches tooltip listeners after each scenario or turn load so tooltips remain functional throughout the full game lifecycle
- **JavaScript syntax errors** in nuclear scenario turn data — six unescaped apostrophes (`engineer's`, `operator's`, `adversary's`, `platform's`, `facility's`) corrected to `\'`

### Changed
- **Scenario navigation** expanded from 4 to 7 scenarios
- `FRACTURE PT.` renamed to `FRACTURE POINT` for consistency with SC object definition
- `_config.yml` removed — not required for single-file GitHub Pages deployments

---

## [0.3.0] - 2026-04-03

### Added
- **Tooltip hover system** — 23 interactive tooltip triggers across left nav and right panel:
  - Left nav: g-GCC master score, IFD / SWD / SCTL / GOV domain health boxes, three intel token types (Technical Observable, Adversarial Signal, Governance Quality), four threat metrics (SBOM-VIS, SC-CONC/HHI, SC-GREY, PATCH-VEL)
  - Right panel: five Governance Confidence tracks, four Regulatory Obligations (EO 14028, NIS2, CISA KEV, EU CRA), Cultural Acceptance, Misinformation Pressure, Allied Coordination Quality
- **Tooltip CSS system** — `.tt-wrap`, `.tt`, `.tt-title`, `.tt-body`, `.tt-thresh` classes; `.tt-left` flip modifier for left-opening variants

---

## [0.2.0] - 2026-03-15

### Added
- **E-AGPO-HT v2.0 scoring engine** — full Ψ_v2 composite scoring function across six Q-dimensions (Q_timing, Q_coord, Q_norm, Q_sctl, Q_acc, Q_domain_sep)
- **g-GCC master score** with nonlinear λ cross-domain coupling term (IFD × SWD amplification)
- **Four AI cybersecurity scenarios** — MIRAGE CHAIN, IRONCLAD SIEGE, FRACTURE POINT, PHANTOM CIRCUIT — each with 5 turns, 4 options per turn, full propagation chain, intel reveals, cascade alerts, and After-Action Review
- **Intel token system** — 3 tokens per turn; Technical Observable, Adversarial Signal, Governance Quality reveal types
- **Governance Artifact upload** — accepts `.txt`, `.md`, `.pdf`, `.docx` for stress-testing against E-AGPO-HT framework
- **Regulatory Obligations panel** — live compliance tracking for EO 14028, NIS2, CISA KEV, EU CRA
- **Governance Confidence tracks** — Technical Resilience, Regulatory Compliance, Diplomatic Coordination, Public/Sector Trust, Supply Chain Trust (τ̄)
- **Policy Stress indicators** — Cultural Acceptance, Misinformation Pressure, Allied Coordination Quality
- **Endgame overlay** — win/loss state with final Ψ_v2 score, grade, and replay option
- **Game log** — timestamped event log across all turns
- **Source Serif 4 / JetBrains Mono / DM Sans** typography stack
- **DOE / National Lab colour palette** — institutional design register

### Changed
- Migrated from prototype to full simulation architecture with turn management, state machine, and dynamic rendering

---

## [0.1.0] - 2026-03-02

### Added
- Initial public demo HTML prototype (`index.html`)
- GitHub Pages deployment workflow (`.github/workflows/deploy.yml`)
- Repository governance files (`README.md`, `.gitignore`)
