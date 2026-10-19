# Self-Healing Orchestrator

A GitHub Actions-based workflow demonstrating automated deployment orchestration, failure detection, recovery execution, and incident notification.

## Purpose
- Reusable deployment workflow using `workflow_call`.
- Trigger deployments on pushes to `main` or manual execution.
- Detect deployment failures and trigger a recovery workflow.
- Capture deployment outcomes for workflow-level reporting.

## Workflow
1. **Deploy:** Invoke the reusable deployment workflow.
2. **Detect:** Check whether the deployment job failed.
3. **Recover:** Execute the configured recovery script.
4. **Notify:** Provide a placeholder for incident notifications.

## Structure
- `.github/workflows/enterprise-orchestrator.yml` — Main orchestration workflow.
- `.github/workflows/reusable-deploy.yml` — Reusable deployment workflow.
- `scripts/` — Deployment and recovery scripts generated during workflow execution.

## Note
This repository demonstrates the orchestration pattern. Actual deployment, rollback, and notification integrations must be implemented and configured for the target environment.
