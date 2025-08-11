# app-deploy
This repository demonstrates the integration of automated repository management and deployment workflows using GitHub Actions.

The featured workflow, **deploy-app**, is designed for CI/CD demonstration and is triggered every push to the main branch.

# Features
- Continuous Integration:
  
  Automated workflow (`deploy-app`) on every push to the main branch.

- Branch Management:

  Includes a feature branch, `feature-deploy`, for updating deployment configuration.

- Security and Permissions:

  Set up uses a GitHub Personal Access Token with the `repo` and `admin:repo_hook` scopes for secure automation.

# Usage

**1. Clone the repository:**
```
git clone https://github.com/allfi-06/app-deploy.git
cd app-deploy
```
**2. Workflow Execution:**

- Any push to the `main` branch automatically triggers the `deploy-app` workflow.
- The workflow can be monitored under the Actions tab.

# Workflow Details
- **File:** `.github/workflows/deploy-app.yml`
- **Trigger:** `push` events on the `main` branch
- **Sample Job:**
  - Checkout code
  - Runs a deploy script (e.g., `echo "Deploying app..."` )

# Branches
- **main**
   -Primary deployment branch where the workflow is triggered
  
- **feature-deploy**
   -Used for development and configuration updates related to app deployment

# Assignment Reference

The repository is configured as per the assignment to:
- Update repo security settings and credentials
- Set up a workflow named `deploy-app`
- Make a required commit on `feature-deploy` branch
- Ensure workflow triggers and completes successfully

# Author
Maintained by allfi-06.

Educational demonstration for CI/CD with GitHub Actions.

# Workflow Status Badge

![Workflow Status](https://github.com/allfi-06/app-deploy/actions/workflows/deploy-app.yml/badge.svg)



