# Echo — Issue Reporting Walkthrough

An interactive, mobile-first product walkthrough for **Echo** (Oro Px · field-staff issue
reporting): one tap on the orange flag files a tracked PSUP ticket with the visit attached,
and the status loop closes in the app. *Report once; the answer echoes back.*

Self-contained static site — `index.html` plus 2x PNG screens exported from Figma
(`px--app-echo`). No build step, no dependencies.

## Flows
| Flow | Screens |
|---|---|
| From a visit — blocker → report → ticket → resolved | 21 |
| From home (TL) — report without a visit open | 21 |
| Sales visit trigger (double agent) | 3 |
| Reports list — partner view | 3 |
| Reports list — manager view | 2 |
| Filter by raised-by | 2 |
| Search (incl. no results) | 3 |
| Cancel a report | 3 |
| Edge cases (empty sheet, shimmer) | 4 |
| Master-view list states | 3 |

Screens whose export has not landed yet are skipped automatically, so the site is never
broken mid-export.

## Run locally
```bash
python3 -m http.server 8139
# open http://localhost:8139
```
