# Echo — Field-Staff Issue Reporting Walkthrough

An interactive product walkthrough for **Echo** (Oro Px · field-staff issue reporting) —
one tap inside Oro Px replaces four WhatsApp groups with a contextual report that files a
tracked PSUP ticket in Linear and closes the loop with a push. *Report once; the answer echoes back.*

A self-contained static site: a big centered phone that steps through each screen with a
crossfade, per-screen trigger hints, a next-flow CTA, and confetti at each flow's end.

## Flows
- **Partners flow** — a field agent hits a blocker mid-visit, files a one-tap report (with draft-save), and tracks the PSUP ticket to resolution.
- **TL login flow** — a team lead reviews visits, files reports, and watches the team's tickets from the manager view.
- **Issue already exists** — reporting a loan that already has an open ticket.

## Run locally
```bash
python3 -m http.server 8137
# open http://localhost:8137
```

No build step. Screens live in `assets/screens/` (3× exports from Figma).

*Built from the Figma file `c-meal / admin` and the Echo engineering spec.*
