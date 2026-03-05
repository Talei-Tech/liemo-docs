# Sprint Plan — First 3 Sprints (Sprint 0–2)

## Sprint 0 — Foundation & Setup (2 Weeks)

**Goal:** Team is aligned, repos are set up, environments are running, and architecture is agreed upon.

| Task ID | Task | Team | Points |
|---------|------|------|--------|
| T-001 | Create GitHub Organization, repos (api, mobile, web-admin, web-superadmin, infra, docs) | Tech Lead | 2 |
| T-002 | Set up GitHub Projects board with Epics, Milestones, Labels | Scrum Master | 2 |
| T-003 | Define Definition of Done and Definition of Ready in GitHub Wiki | Scrum Master | 1 |
| T-004 | Set up Django project: apps structure, PostgreSQL connection, JWT auth, Swagger/OpenAPI | Backend | 5 |
| T-005 | Set up Flutter project: folder structure, routing (GoRouter), state management (Riverpod/Bloc) | Mobile | 5 |
| T-006 | Set up React project (Vite + TypeScript + TailwindCSS) for admin and super admin portals | Frontend | 5 |
| T-007 | Set up Docker Compose for local dev (Django + PostgreSQL + Redis) | DevOps | 3 |
| T-008 | Set up GitHub Actions CI: lint, test, build pipelines for all repos | DevOps | 5 |
| T-009 | Create ERD and finalize core data models in PostgreSQL via Django migrations | Backend | 5 |
| T-010 | Design System: define colors, typography, components in Figma for Flutter and React | UI/UX | 8 |

**Sprint 0 Total: 41 points**

## Sprint 1 — Auth & Store Core (2 Weeks)

**Goal:** Users can register and log in. Store admins can create a store and add links.

- US-001, US-002, US-003 — End user registration, login, SSO, password reset
- US-004 — Store admin onboarding flow
- US-010 — Store profile creation (name, logo, bio)
- US-011 — Add/edit/delete platform links
- US-012 — Assign store to categories
- US-043 — Super admin: create and manage categories

## Sprint 2 — Discovery & Live Status (2 Weeks)

**Goal:** End users can browse, search, and see live stores on mobile.

- US-020 — Browse stores by category
- US-021 — Search stores
- US-022 — Top rated feed
- US-023 — Live now feed
- US-013 — Store admin: toggle live status
- US-025 — End user: follow stores
- US-026 — View store profile with all links
