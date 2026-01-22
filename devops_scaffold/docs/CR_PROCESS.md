# Change Request (CR) Process

## Objective
Ensure all changes are reviewed, traceable, tested, and reversible.

## Workflow
1. Create Change Request (CR) issue.
2. Create feature branch from develop.
3. Open PR and link CR.
4. CI must pass + 1 approval required.
5. Merge to develop → staging deploy.
6. Validate in staging.
7. Release PR develop → main.
8. Merge → production deploy.
9. Close CR with validation notes.

## Risk Levels
- Low: UI / config only
- Medium: business logic
- High: data, auth, payments

## Rollback
Rollback must be documented for every CR.
