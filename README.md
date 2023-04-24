# Renovate-Config

This repository contains a default configuration file from which the `renovate.json` can extend from in other repositories.

## Renovate

Renovate allows for automatic dependency updates.

### default.json

Listed are some default configurations, that can be extended from in a `renovate.json` file inside another repository.

| Configuration                      | Details                                                                                 |
|------------------------------------|-----------------------------------------------------------------------------------------|
| semanticCommits                    | Created PRs follow the semantic commit message format.                                  |
| group:allNonMajor                  | All non major dependency updates are grouped into one PR.                               |
| enableVulnerabilityAlertsWithLabel | Any PR with known dependency vulnerabilities get assigned a high priority label.        |
| rebaseStalePrs                     | Renovate will rebase stale PRs (e.g. if there are conflicts or are behind base branch). |
| dependencyDashboard                | Provides a dependency dashboard under the issues section of the repo if set to true.    |
| schedule                           | Renovate runs every hour.                                                               |
| pre-commit                         | Enable updating of pre-commit hooks.                                                    |
