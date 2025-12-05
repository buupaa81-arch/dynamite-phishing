# Changelog

All notable changes to this project will be documented in this file.  
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and adheres to [Semantic Versioning](https://semver.org/).

---

## [Unreleased]
- Work in progress features
- Planned improvements and experimental rules

---

## [0.1.0] - 2025-12-05
### Added
- Initial release of Dynamite Phishing.
- Core heuristics:
  - Punycode/IDN domain detection
  - Deep subdomain chain detection
  - Link mismatch detection
  - DOM signals (multiple password fields, seed/mnemonic inputs, script count)
- Banner UI with risk score and “Show reasons” breakdown.
- Developer installation instructions via `about:debugging`.

---

## [0.2.0] - Planned
### Added
- Adjustable scoring profiles (Cautious / Strict).
- Settings page for user customization.
- Expanded heuristics for certificate/TLS anomalies.

---

## [0.3.0] - Planned
### Added
- Offline ML model import (manual, signature‑verified).
- Extended DOM heuristics for urgency cues (timers, fake modals).
- Documentation updates in `docs/rules.md`.

---

## [1.0.0] - Planned
### Added
- Full audit reports and hardened build.
- Comprehensive test coverage and integration test pages.
- Security review and bounty program launch.

---

## Version List

- **0.1.0** — Core heuristics + banner UI (released)
- **0.2.0** — Adjustable scoring profiles + TLS checks (planned)
- **0.3.0** — Offline ML model import + extended DOM heuristics (planned)
- **1.0.0** — Hardened build + audit reports + full test coverage (planned)
