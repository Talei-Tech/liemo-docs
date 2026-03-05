# Definition of Done (DoD)

A User Story or Task is **DONE** when ALL of the following are true:

1. Code is written and peer-reviewed via GitHub Pull Request (minimum 1 reviewer approval)
2. Unit tests written and passing (>= 80% coverage for business logic)
3. Integration tests passing in CI pipeline
4. API endpoints documented in Swagger / OpenAPI spec
5. No P1 or P2 bugs open against the story
6. Feature tested on all target platforms (iOS, Android, Chrome, Safari)
7. UX matches Figma design within agreed tolerance
8. Product Owner has accepted the story in the Sprint Review
9. Deployed to staging environment

# Definition of Ready (DoR)

A User Story is **READY** to enter a Sprint when:

1. Story is written in 'As a [actor], I want [action], so that [value]' format
2. Acceptance criteria are defined (Given/When/Then or clear checklist)
3. Story is estimated in story points by the team
4. Dependencies are identified and resolved or tracked
5. UI/UX mockup is available for frontend stories
6. API contract is agreed for stories spanning mobile/web and backend
