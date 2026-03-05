# Risk Register

| ID | Risk | Likelihood | Impact | Mitigation |
|----|------|-----------|--------|------------|
| R-01 | Live status accuracy — platforms don't offer APIs for live status detection | High | High | Implement manual toggle by store admin as MVP; explore platform API access and webhooks in Phase 2 |
| R-02 | Payment gateway integration complexity (multiple regions: PH, Kuwait) | Medium | High | Start with Stripe globally; integrate PayMongo (PH) in Sprint 5; KNET (Kuwait) in Phase 2 |
| R-03 | App Store / Play Store rejection (ads, payments) | Medium | High | Follow Apple/Google guidelines strictly; use In-App Purchase for subscriptions on iOS |
| R-04 | GDPR / Philippine DPA / Kuwait data privacy compliance | Medium | High | Engage legal counsel early; implement consent management, data residency options |
| R-05 | Scope creep — platform too broad too early | High | Medium | Enforce MoSCoW prioritization; PO must approve scope changes; freeze Phase 1 scope |
| R-06 | Team velocity lower than estimated | Medium | Medium | Build buffer in sprint capacity (plan at 70%); use velocity from Sprint 1 to calibrate |
| R-07 | Third-party platform link rot (TikTok, FB links change) | Low | Medium | Implement link health check job (Celery) that pings links and flags broken ones |
