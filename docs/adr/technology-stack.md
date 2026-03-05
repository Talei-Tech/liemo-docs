# Architecture Decision Record — Technology Stack

## ADR-001: Liemo Technology Stack

**Date:** March 2026  
**Status:** Accepted

| Layer | Technology | Rationale |
|-------|-----------|----------|
| Mobile App (End User) | Flutter 3.x (Dart) | Single codebase for iOS and Android; rich UI widgets; strong community; suits Philippines and Kuwait markets |
| Web Frontend (Admin + Super Admin) | React 18 + TypeScript + Vite | Component reuse across admin and super admin portals; large ecosystem; SSR with Next.js option for SEO |
| Backend API | Python 3.12 + Django 5 + Django REST Framework | Mature, batteries-included; excellent PostgreSQL ORM; strong auth, admin scaffold; large Python talent pool |
| Database | PostgreSQL 16 | Relational integrity for subscriptions, links, ratings; JSONB for flexible platform metadata; proven at scale |
| Real-time (Live Status) | Django Channels + Redis (WebSocket) | Live status updates pushed to end users without polling |
| Cache & Queue | Redis 7 | Caching hot queries (top stores, categories); Celery task queue for notifications, analytics aggregation |
| Object Storage | AWS S3 / Cloudflare R2 | Store logos, media assets; CDN distribution for Philippines and Kuwait |
| Authentication | JWT (djangorestframework-simplejwt) + OAuth2 (Google/Apple) | Stateless API auth; social login for end users |
| Payment Gateway | Stripe (global) + PayMongo (PH) + KNET (Kuwait) | Subscription billing; wallet top-up; regional payment compliance |
| Push Notifications | Firebase Cloud Messaging (FCM) | Cross-platform push for Flutter mobile |
| CI/CD | GitHub Actions | Automated test, lint, build, deploy pipelines integrated with GitHub Projects |
| Hosting | AWS (ECS/Fargate + RDS + ElastiCache) or Railway/Render (MVP) | Scalable container deployment; RDS managed PostgreSQL |
| Source Control & Project | GitHub (Repos + Projects + Issues) | Monorepo or multi-repo; Kanban/Scrum board; issue-linked commits |
