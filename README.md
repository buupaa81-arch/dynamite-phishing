# Dynamite Phishing

An open, Tor‑compatible browser extension that detects likely phishing pages without tracking the user. The goal is transparent, explainable, and community‑driven protection.

## Why This Project?
Phishing attacks exploit look‑alike domains, DOM tricks, and urgency cues. Dynamite Phishing scores risk signals locally and shows clear reasons for alerts.

## Privacy Principles
- **No telemetry:** No external HTTP requests, no exfiltration of browsing data.
- **Local analysis only:** All detection runs inside your browser.
- **Optional debug logs:** If enabled, logs remain local and can be deleted with one click.
- **Explainable UI:** The “Show reasons” button always reveals why a page was flagged.

## Features
- **Heuristics:** Detect punycode/IDN domains, deep subdomain chains, link mismatches, suspicious DOM forms.
- **Lightweight ML (optional, offline):** Pre‑packaged model, imported manually with signature verification.
- **Explainable alerts:** Banner at the top of the page with risk score and detailed breakdown.

## Installation (Developer Mode)
1. Clone this repository.
2. Open Tor Browser.
3. Navigate to `about:debugging` → `This Firefox` → `Load Temporary Add‑on`.
4. Select `manifest.json`.

## Contribution Guidelines
- Fork → feature branch → Pull Request with tests and rule explanations.
- Each new detection rule must include:
  - **Explanation:** Why the rule is needed.
  - **Tests:** Unit and DOM test cases.
  - **Documentation:** Update `docs/rules.md` and CHANGELOG.
- Respect privacy principles: no code that sends data externally without explicit opt‑in.

## Bug Bounty
We run a transparent bounty program to accelerate high‑quality development:
- Rewards for critical vulnerabilities, impactful detection rules, privacy improvements, and documentation quality.
- Details in [`BOUNTY.md`](./BOUNTY.md).

## Responsible Disclosure
- Report vulnerabilities privately as described in [`SECURITY.md`](./SECURITY.md).
- We acknowledge reports within 72 hours and aim to fix within 30 days.

## Roadmap
- **v0.1:** Core heuristics, banner alerts, basic UI.
- **v0.2:** Adjustable scoring profiles (cautious/strict).
- **v0.3:** Offline ML model import with signature verification.
- **v1.0:** Full audit reports, comprehensive test coverage, hardened build.

## License
MIT (or Apache‑2.0). Open, commercially compatible, but always aligned with privacy and ethical principles.
