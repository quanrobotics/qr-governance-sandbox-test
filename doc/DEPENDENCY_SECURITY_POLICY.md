# QuanRobotics Dependency Security Policy

## 1. Purpose

This policy defines how QuanRobotics identifies, reviews, remediates, and tracks security risks in software dependencies.

The goal is to ensure that known vulnerable, outdated, unsupported, or unnecessary dependencies do not reach protected branches or public releases without review.

---

## 2. Scope

This policy applies to:

- Python dependencies
- GitHub Actions dependencies
- Build and CI/CD dependencies
- Runtime dependencies
- Development and testing dependencies
- Third-party libraries
- Packages used by QuanRobotics repositories
- Future ROS, Node.js, system, container, and other ecosystem dependencies

---

## 3. Dependency Requirements

QuanRobotics repositories should:

- Declare dependencies explicitly.
- Keep dependency files under version control.
- Pin important dependency versions where practical.
- Use lock files where supported.
- Avoid unnecessary dependencies.
- Review new dependencies before merging.
- Keep dependencies actively maintained.
- Review licensing implications before introducing third-party packages.
- Monitor dependencies for known vulnerabilities.
- Keep GitHub Actions versions maintained.

Dependencies must not be added only because they are convenient if equivalent functionality can be implemented safely with the existing stack.

---

## 4. Dependency Security Controls

Active code repositories should use the following controls where applicable:

- GitHub Dependency Graph
- Dependabot Alerts
- Dependabot Security Updates
- Dependabot Version Updates
- CI-based dependency vulnerability scanning
- Repository-specific package audit tools

For the current Python baseline, QuanRobotics uses:

```text
pip-audit
