# PathFinder — Meeting Intelligence System

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.1.0-brightgreen.svg)](CHANGELOG.md)
[![HIPAA Aware](https://img.shields.io/badge/HIPAA-Aware-red.svg)](#security)
[![No Build Tools](https://img.shields.io/badge/build-none%20required-lightgrey.svg)](#getting-started)

> A single-page healthcare project management dashboard that transforms meeting transcripts into structured intelligence — surfacing priorities, tracking deliverables, and keeping distributed clinical IT teams aligned.

---

## 📸 Screenshot

<!-- Replace with an actual screenshot once deployed -->
![PathFinder Dashboard Screenshot](docs/screenshot.png)

---

## ✨ Features

### 🗂 Role-Based Views
- **PM View** — Full project oversight: budget, timeline, risks, team utilization, and executive summaries.
- **Team Member View** — Personalized task lists, individual deliverables, and meeting action items filtered to each role.
- Supported roles: PM, Technical Consultant, Lead Software Engineer, Senior Quality Consultant, Solutions Architect, UX/UI Designer, DevOps Engineer, Data Analyst, Security Engineer, Technical Writer, Project Coordinator, Business Analyst.

### 📋 Meeting Intelligence
- Upload or paste meeting transcripts for automatic processing.
- AI-generated meeting notes with structured summaries, decisions, and action items.
- Searchable meeting history with participant tracking.

### ✅ Task & Deliverable Management
- **Tasks at Hand** — Click-to-detail modal for each task with status, owner, priority, and due date.
- Priority matrix (Critical / High / Medium / Low) with visual indicators.
- Deliverables tracker with completion percentages and milestone mapping.
- Team progress dashboard with per-role utilization charts (Chart.js).

### 🤖 AI Priority Assistant
- Inline assistant for reprioritizing tasks based on project context.
- Suggests blockers and dependency chains from transcript data.

### 🔗 Integrations
| Platform | Capability |
|---|---|
| **Microsoft Teams** | Meeting transcript import, notification webhooks |
| **Outlook** | Calendar sync, meeting invite parsing |
| **Slack** | Action-item notifications, daily digest |
| **Box** | Document storage, deliverable file linking |
| **Epic EHR** | FHIR R4 resource references, workflow context |

### 🏥 Healthcare & Compliance
- HIPAA-aware data handling patterns (no PHI stored client-side by default).
- FHIR R4 integration hooks for Epic EHR environments.
- Audit-trail-ready action logging.

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 (semantic) |
| Styling | CSS3 with custom properties (CSS variables) |
| Logic | Vanilla JavaScript (ES6+) |
| Charts | [Chart.js](https://www.chartjs.org/) v4 |
| Fonts | [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts |
| Build | **None** — open `index.html` directly |

No npm, no bundler, no framework. Works offline after first load.

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome 90+, Firefox 88+, Edge 90+, Safari 14+).
- No server, no Node.js, no dependencies to install.

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-org/pathfinder.git

# 2. Enter the project directory
cd pathfinder

# 3. Open the app
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Or simply drag `index.html` into your browser.

### Optional: Local HTTP Server
Some browser security policies restrict local file access. If features behave unexpectedly, serve the file over HTTP:

```bash
# Python 3
python -m http.server 8080

# Node (npx)
npx serve .
```

Then visit `http://localhost:8080`.

---

## 📁 Project Structure

```
pathfinder/
├── index.html              # Single-page application entry point
├── css/
│   └── styles.css          # All styles (CSS variables, layout, components)
├── js/
│   ├── app.js              # Bootstrap, routing, role switching
│   ├── meetings.js         # Transcript parsing & meeting intelligence
│   ├── tasks.js            # Task management & modal logic
│   ├── charts.js           # Chart.js wrappers for progress visuals
│   ├── integrations.js     # Box / Teams / Outlook / Slack connectors
│   └── ai-assistant.js     # Priority assistant logic
├── data/
│   └── sample-data.json    # Demo data (no real PHI)
├── docs/
│   └── screenshot.png      # Dashboard screenshot (update after deploy)
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── SECURITY.md
```

---

## 👥 Role Views Explained

PathFinder adapts its UI based on the selected role. Use the role switcher in the top navigation bar.

| Role | Primary View |
|---|---|
| **PM** | Full dashboard: budget, timeline, risks, team utilization, all tasks |
| **Technical Consultant** | Technical deliverables, architecture decisions, FHIR/Epic tasks |
| **Lead Software Engineer** | Sprint tasks, code review items, engineering blockers |
| **Senior Quality Consultant** | QA checklist, test coverage, defect tracking |
| **Solutions Architect** | System design decisions, integration status, dependency map |
| **UX/UI Designer** | Design deliverables, prototype links, UX feedback items |
| **DevOps Engineer** | Infrastructure tasks, deployment pipeline, environment status |
| **Data Analyst** | Reporting tasks, data pipeline items, analytics deliverables |
| **Security Engineer** | Security findings, HIPAA controls, vulnerability tasks |
| **Technical Writer** | Documentation tasks, review queue, publication status |
| **Project Coordinator** | Meeting schedule, action item follow-ups, status reports |
| **Business Analyst** | Requirements traceability, stakeholder items, gap analysis |

---

## 🤝 Contributing

We welcome contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

All participants are expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

---

## 🔒 Security

PathFinder is designed for use in healthcare IT environments. For vulnerability disclosure and our HIPAA-aware security policy, see [SECURITY.md](SECURITY.md).

**Never commit real patient data (PHI) to this repository.**

---

## 📄 License

[MIT](LICENSE) © 2026 [Your Organization]
