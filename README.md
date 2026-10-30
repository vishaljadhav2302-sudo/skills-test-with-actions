# Skills: Test with Actions (Continuous Integration)

![Python package](https://github.com/vishaljadhav2302-sudo/skills-test-with-actions/actions/workflows/python-package.yml/badge.svg)
![Python Coverage](https://github.com/vishaljadhav2302-sudo/skills-test-with-actions/actions/workflows/python-coverage.yml/badge.svg)

---

## CI/CD Write-up & Concept Summary

### 1. What is a GitHub Actions Workflow?
A GitHub Actions workflow is an automated, configurable process defined by a YAML file in the `.github/workflows` directory. It automatically runs one or more jobs whenever a specified event (such as a pull request or code push) occurs in the repository.

### 2. Triggers, Jobs, and Steps
- **Triggers (`on`):** Events that initiate the workflow execution, such as `push`, `pull_request`, or schedule triggers.
- **Jobs:** A set of steps executed on the same runner environment (e.g., `ubuntu-latest`). Jobs run in parallel by default unless configured with dependencies (`needs`).
- **Steps:** Individual tasks within a job executed sequentially. They can run shell commands, scripts, or reusable GitHub Marketplace actions.

### 3. How to Use This in a Real Project
In real-world production environments, CI/CD pipelines automate linting, unit testing, code coverage thresholds, and multi-version matrix builds on every pull request. This enforces branch protection rules to prevent broken code from merging into production branches, and automatically builds, tests, and deploys containerized applications or packages to artifact registries.
