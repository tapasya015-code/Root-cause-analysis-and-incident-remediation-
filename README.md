# Autonomous Rollback Agent

An agent that watches error rates after each deployment and rolls back automatically when they cross a safe threshold, without waiting for a human.

**Live demo:** https://tapasya015-code.github.io/Root-cause-analysis-and-incident-remediation-

## How it works
1. A new version is deployed.
2. The agent monitors the error rate every 1.5 seconds.
3. If the error rate goes above 5%, it logs an alert and rolls back to the last stable version.
4. The service returns to Healthy and every action is logged.

## Team
- M.Tapasya: Frontend (dashboard)
- S.Hansika Reddy: Detection logic
- D.Akshara Reddy: Remediation logic
- K.Deepthi Sanjana: Docs and presentation 