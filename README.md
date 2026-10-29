# Autonomous Rollback Agent

An agent that watches error rates after each deployment and rolls back automatically when they cross a safe threshold, without waiting for a human.

**Live demo:** https://tapasya015-code.github.io/Root-cause-analysis-and-incident-remediation-

## How it works
1. A new version is deployed.
2. The agent monitors the error rate every 1.5 seconds.
3. If the error rate goes above 5%, it logs an alert and rolls back to the last stable version.
4. The service returns to Healthy and every action is logged.

## Setup and run instructions
1. Open the live demo: https://tapasya015-code.github.io/Root-cause-analysis-and-incident-remediation-
2. Or download this repo and open 'index.html' in any web browser. No installation needed.
3. Tap **Deploy v1.1.0 (with bug)** to simulate a bad release.
4. Watch the error rate spike above 5%, the agent roll back to v1.0.0, and the log record each step.
5. Tap **Reset demo** to run it again.

## Team
- M.Tapasya: Frontend (dashboard)
- S.Hansika Reddy: Detection logic
- D.Akshara Reddy: Remediation logic
- K.Deepthi Sanjana: Docs and presentation 