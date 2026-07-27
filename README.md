# PathFinder — Healthcare Project Management Dashboard

A single-file, zero-dependency interactive HTML demo for a healthcare IT project management platform. PathFinder provides two distinct views — a **PM Dashboard** and a **Team Member View** — built for Epic EHR integration and HIPAA-compliant software delivery projects.

Fully responsive: works on desktop, tablet, and mobile.

---

## Features

### PM Dashboard
- **Tasks at Hand** — filterable task table (All / In Progress / Pending / Completed) with click-to-detail modals
- **Project Progress** — live Gantt-style timeline with milestone tracking
- **Team Progress** — individual team member cards with completion stats and progress bars
- **Risk Register** — categorized risk tracking with severity indicators
- **Priorities** — ranked action items with owner and due date
- **AI Assistant** — project-aware chat interface

### Team Member View
- **Overview Tab** — personalized stat cards (My Tasks, Overdue, Completed This Week, Team Progress) that update live when tasks are checked off; activity chart
- **Tasks Tab** — full task list with click-to-detail drawer showing descriptions, requirements, acceptance criteria, and independent per-task comment threads
- **Meeting Notes Tab**
  - Most recent meeting: paragraph summary with **See more** to expand full notes; Decisions and Key Action Items always visible below
  - Past meetings: clickable cards that open a full notes modal with multi-paragraph notes, per-meeting comment thread, and download button
  - Top 5 Priorities from last meeting — each clickable for full task detail

---

## Mobile Support

PathFinder is fully responsive at all screen sizes:

| Breakpoint | Behaviour |
|---|---|
| ≤ 1200px | Single-column dashboard grid |
| ≤ 768px | Sidebar becomes a slide-in drawer; search hidden |
| ≤ 480px | 2-column stat cards; nav tabs scroll horizontally; modals slide up as bottom sheets; Gantt scrolls horizontally |

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
- **Chart.js 4.4** (CDN) — progress and activity charts
- **CSS custom properties** — theming via `--primary-color` and `--secondary-color`
- **CSS Grid + Flexbox** — fully responsive layout
- **Inter** (Google Fonts CDN) — typography

---

## Project Context

This demo simulates a real-world healthcare IT delivery project with three workstreams:

1. **Epic EHR Integration** — FHIR R4 API, OAuth 2.0 + PKCE authentication
2. **Patient Data Dashboard** — real-time clinical data visualization
3. **Consent Management Module** — digital signatures, versioning, audit trail (HIPAA-compliant)

**Go-live target:** August 28, 2026 (phased rollout)
**HIPAA compliance deadline:** August 31, 2026

---

## File Structure

```
Final_PathFinder/
├── index.html      # Complete application (single file, ~350 KB)
├── README.md       # This file
├── LICENSE         # MIT License
└── .gitignore      # Standard web project ignores
```

---

## License

MIT — see [LICENSE](LICENSE) for details.
