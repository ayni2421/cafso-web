# CAFSO Network — Web Frontend

Commercial Asset & Field-Service Orchestration Network — Web UI

## Overview

Single-page application built with React 18 (CDN), plain HTML/CSS/JS.
No build step required — just serve with Node.js.

## Tech Stack

- React 18 (via CDN, no bundler)
- Babel Standalone (JSX transform in browser)
- Pure CSS (no framework)
- Node.js HTTP server

## Role-Based Dashboards

| Role | Dashboard Features |
|------|--------------------|
| OrgAdmin | Service status, invite team members, org overview |
| Dispatcher | Work order queue, technician assignment |
| Technician | Assigned jobs, field execution, evidence upload |
| Supervisor | Verification queue, SLA monitoring |
| Asset Manager | Asset registry, risk scoring, maintenance plans |
| Inventory Manager | Stock levels, reorder alerts, procurement |
| Requester | Fault reporting, request tracking |

## Running

```bash
node server.js
```

Open: http://localhost:3000

## Backend API

Connects to Identity Service at http://localhost:4001
See the backend repository for full API documentation.

## Environment

The API base URL is hardcoded to `http://localhost:4001`.
Update `const ID = 'http://localhost:4001'` in `public/index.html`
to point to your deployed backend.
