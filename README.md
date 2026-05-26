# FairLend-Audit
FairLend-Audit
# FairLend Audit Demo Assets

## Recommended live demo

Open:

- `index.html`

This is the new mobile-friendly interactive prototype. It supports:

- case selection for A1024, A1026, and A1027
- fairness threshold adjustment
- proxy-variable scan
- applicant explanation preview
- human review actions
- regulatory audit-log updates
- responsive desktop and phone layouts
- independent state per case, so scanning or explaining A1024 does not incorrectly carry over to A1026 or A1027
- tablet-width navigation support, so the bottom navigation appears as soon as the desktop sidebar is hidden

The older entry `index.html` now redirects to the interactive demo so the wrong prototype is not opened during presentation.

## Figma workflow

Use the existing Figma file as the visual source, then update it with the new interaction model:

1. Keep the current six-screen flow as your baseline:
   - `01-login.svg`
   - `02-dashboard.svg`
   - `03-case-detail.svg`
   - `04-proxy-scan.svg`
   - `05-explanation-report.svg`
   - `06-human-review-log.svg`
2. Import or redraw the new interactive-demo states in Figma:
   - dashboard with threshold slider
   - flagged case cards
   - proxy scan complete state
   - applicant explanation preview
   - review action and audit-log saved state
3. Add mobile frames around 390 x 844 and connect them using Prototype mode.
4. Use Smart Animate for:
   - Dashboard -> Case
   - Case -> Proxy Scan
   - Proxy Scan -> Explanation
   - Explanation -> Review
5. Use the HTML demo as the working backup if Figma internet access fails.

## Research mapping

The demo is built around the paper's core argument: AI mortgage systems should be fair, explainable, and accountable, not only accurate.

Feature mapping:

- Fairness risk: rejection-rate disparity dashboard and adjustable alert threshold.
- Proxy risk: postcode, employment type, credit history, savings record, and loan-to-value scan.
- Explainability: plain-language applicant report with correctable factors.
- Human oversight: high-risk AI rejections cannot become final automatically.
- Accountability: audit log records original AI decision, risk level, reviewer action, and outcome.
