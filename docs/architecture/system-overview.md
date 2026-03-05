# System Architecture Overview

## Repository Structure

GitHub Organization: `talei-tech`

| Repo | Purpose |
|------|---------|
| `liemo-mobile` | Flutter app (end user iOS/Android) |
| `liemo-web-admin` | React app (store owner portal) |
| `liemo-web-superadmin` | React app (super admin dashboard) |
| `liemo-api` | Django REST API (shared backend) |
| `liemo-infra` | Terraform/IaC scripts, Docker Compose, CI configs |
| `liemo-docs` | Architecture diagrams, ADRs, API specs (OpenAPI) |

## Component Overview

| Component | Responsibility | Talks To |
|-----------|---------------|----------|
| Flutter Mobile App | End user discovery, browsing, following, live status | Django REST API (HTTPS), FCM (push) |
| React Admin Web | Store management, link CRUD, analytics, subscription | Django REST API (HTTPS) |
| React Super Admin Web | Platform management, user management, analytics, ads | Django REST API (HTTPS) |
| Django API | Business logic, auth, all data operations, WebSocket gateway | PostgreSQL, Redis, S3, FCM, Stripe/PayMongo |
| PostgreSQL | Primary data store: users, stores, links, categories, ratings, subscriptions | Django ORM |
| Redis | Session cache, Celery broker, WebSocket channel layer | Django Channels, Celery |
| Celery Workers | Async tasks: notification dispatch, analytics aggregation, email | Redis, PostgreSQL, FCM, SMTP |
| AWS S3 / R2 | Static assets, store logos, ad images | Django (upload), CDN (serve) |
