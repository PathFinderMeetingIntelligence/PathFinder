# PathFinder — Healthcare Project Management Dashboard

A single-file interactive HTML demo for a healthcare IT project management platform. PathFinder provides two distinct views — a **PM Dashboard** and a **Team Member View** — designed for use on Epic EHR integration and HIPAA-compliant software delivery projects.

---

## Features

### PM Dashboard
- **Tasks at Hand** — filterable task table (All / In Progress / Pending / Completed) with click-to-detail modals
- **Project Progress** — live Gantt-style timeline with milestone tracking
- **Team Progress** — individual team member cards with completion stats and progress bars
- **Risk Register** — categorized risk tracking with severity indicators
- **AI Assistant** — project-aware chat interface

### Team Member View
- **Overview Tab** — personalized stat cards (My Tasks, Overdue, Completed This Week, Team Progress) that update live when tasks are checked off
- **Tasks Tab** — full task list with click-to-detail side drawer showing descriptions, requirements, acceptance criteria, and per-task comment threads
- **Meeting Notes Tab**
  - Most recent meeting: Summary (with **See more** to expand full notes), Decisions, and Key Action Items always visible
  - Past meetings: clickable cards that open a full notes modal with comments and download
  - Top 5 Priorities from last meeting — each clickable for full task detail

---

## Team

| Name | Role |
|---|---|
| Emily Watson | Technical Consultant |
| Mike Rodriguez | UI/UX Designer |
| Jennifer Park | QA Lead |
| Erin Hardy | Package Consultant |
| David Kim | Backend Engineer |
| Sarah Chen | Frontend Engineer |
| Thomas Wright | Business Analyst |

---

## Getting Started

No build step required. This is a fully self-contained single-file application.

```bash
# Clone the repo
git clone https://github.com/your-org/pathfinder.git
cd pathfinder

# Open directly in your browser
open index.html

# Or serve locally
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

## Tech Stack

- **HTML5 / CSS3 / Vanilla JavaScript** — zero dependencies, no frameworks
- **Chart.js** (CDN) — progress and activity charts
- **CSS custom properties** — theming via `--primary-color` and `--secondary-color`

---

## Project Context

This demo simulates a real-world healthcare IT delivery project with the following workstreams:

1. **Epic EHR Integration** — FHIR R4 API, OAuth 2.0 + PKCE authentication
2. **Patient Data Dashboard** — real-time clinical data visualization
3. **Consent Management Module** — digital signatures, versioning, audit trail (HIPAA-compliant)

**Go-live target:** August 28, 2026 (phased rollout)  
**HIPAA compliance deadline:** August 31, 2026

---

## File Structure

```
Final_PathFinder/
├── index.html      # Complete application (single file)
├── README.md       # This file
├── LICENSE         # MIT License
└── .gitignore      # Standard web project ignores
```

---

## License

MIT — see [LICENSE](LICENSE) for details.
