# Health Facility Locator (Google Maps Integration)

Outsourced feature build tracked for a Fiverr engagement. This repo is the
freelancer-facing source of truth: scope, tasks, branching rules, and PR
review process live here so progress is auditable outside of chat threads.

## What this feature does

Lets a user find the nearest health facilities (hospitals, clinics,
laboratories, pharmacies) from their current location or a searched address,
with filters for facility type and available services (e.g. immunization,
radiology). Built as a component/module inside the existing NaviHealth-style
web app, using the Google Maps JavaScript API + Places API.

See [`docs/BRIEF.md`](docs/BRIEF.md) for the full Fiverr project brief and
[`docs/PROJECT_BOARD.md`](docs/PROJECT_BOARD.md) for how work is tracked.

## Repo structure

```
health-facility-locator/
├── README.md
├── CONTRIBUTING.md
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── task.md
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/
│   ├── BRIEF.md              # Full Fiverr brief (scope, deliverables, budget)
│   └── PROJECT_BOARD.md      # Board columns, branching model, review flow
└── issues/                   # Placeholder tasks (mirrors GitHub Issues)
    ├── 01-project-setup.md
    ├── 02-maps-base-integration.md
    ├── 03-geolocation-and-search.md
    ├── 04-facility-data-and-filters.md
    ├── 05-facility-list-and-detail-view.md
    ├── 06-responsive-ui-polish.md
    └── 07-testing-and-handover.md
```

Each file under `issues/` is written as a ready-to-paste GitHub Issue
(title, description, acceptance criteria, estimate, dependency). When the
freelancer is confirmed, these get copy-pasted into the **Issues** tab so
they show up on the **Projects** board automatically.

## Branching model

- `main` — always deployable; freelancer never pushes directly here.
- `dev` — integration branch; freelancer's feature branches merge here via PR.
- `feature/<issue-number>-<short-slug>` — one branch per issue, e.g.
  `feature/03-geolocation-and-search`.

## Access given to the freelancer

- Write access to this repo only (not the main product monorepo).
- A sandbox Google Maps API key with a $0 daily spend cap and domain
  restriction to the staging URL.
- Read access to a sample (anonymized) facility dataset for local dev.
