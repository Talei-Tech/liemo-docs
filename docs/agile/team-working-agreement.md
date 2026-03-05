# Team Working Agreement

| Area | Agreement |
|------|-----------|
| Sprint Length | 2 weeks; Sprint starts Monday, ends Friday of second week |
| Sprint Planning | Monday morning of sprint start; max 3 hours; PO presents top stories; team estimates and commits |
| Daily Standup | Async in GitHub Discussions or Slack by 10:00 AM local time; 3 questions: Done, Doing, Blockers |
| Sprint Review | Friday afternoon of sprint end; demo to PO; stories accepted or rejected |
| Retrospective | Friday after Sprint Review; max 1 hour; Start/Stop/Continue format; action items as GitHub Issues |
| Backlog Grooming | Mid-sprint (Wednesday of week 1); PO + Tech Lead + Scrum Master; max 2 hours |
| Pull Requests | All code via PR; min 1 approval; CI must pass; link to GitHub Issue; use PR template |
| Branch Naming | `feature/US-001-user-registration`, `fix/BUG-042-login-crash`, `chore/setup-ci` |
| Code Review SLA | Reviewer must review within 24 business hours of PR raised |
| Definition of Ready check | Scrum Master confirms DoR before any story enters sprint planning |
| Communication | GitHub Issues for tasks/bugs; Slack/Teams for async chat; Video call for planning/retro |
| Working Hours | Core overlap hours 10:00 AM – 4:00 PM (Manila time as reference for PH market team) |

## Commit Convention

Enforce conventional commits across all repos:

```
feat(scope): add store live toggle endpoint
fix(auth): resolve JWT refresh token race condition
docs(api): update OpenAPI spec for /stores endpoint
test(ratings): add unit tests for rating aggregation
chore(ci): add flutter build step to GitHub Actions
```

**Valid scopes:** `auth`, `stores`, `links`, `categories`, `analytics`, `subscriptions`, `wallet`, `ads`, `notifications`, `mobile`, `web`, `api`, `infra`
