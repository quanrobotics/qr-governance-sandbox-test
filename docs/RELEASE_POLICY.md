# QuanRobotics Release Policy

## 1. Purpose

This policy defines the minimum technical and governance requirements for
creating versioned QuanRobotics software releases.

A release must be traceable to an immutable Git commit, validated through
the required CI and security controls, and accompanied by meaningful
release notes.

## 2. Versioning Convention

QuanRobotics repositories should use Semantic Versioning:

MAJOR.MINOR.PATCH

Git release tags use the format:

vMAJOR.MINOR.PATCH

Examples:

v0.1.0
v0.2.0
v1.0.0
v1.2.3

## 3. Version Meaning

### MAJOR

Increment when incompatible or major architectural changes are introduced.

### MINOR

Increment when backward-compatible features or substantial capabilities
are added.

### PATCH

Increment for backward-compatible bug fixes, documentation corrections,
security remediations, or small improvements.

During early development, repositories may remain in the 0.x.y version
range.

## 4. Release Source

Production/public releases must originate from an approved commit that has
passed the repository's required engineering workflow.

A release must not be created from an unreviewed experimental branch.

## 5. Required Pre-Release Validation

Before creating a release, verify:

- Required CI checks pass.
- Unit/basic tests pass.
- Dependency-security checks pass where configured.
- Secret/security checks pass where configured.
- Required reviews are complete.
- Relevant documentation is updated.
- CHANGELOG.md is updated.
- Known limitations are documented.
- Release version is confirmed.
- No confidential information is included.

## 6. Release Tag Rules

Release tags must use:

vMAJOR.MINOR.PATCH

Examples:

v0.1.0
v1.0.0
v1.4.2

Released tags must not normally be moved, overwritten, or reused.

If a released version is defective, create a corrective version rather
than silently replacing the existing tag.

Example:

v0.1.0
then
v0.1.1

## 7. Release Notes

Each GitHub Release should include:

- Release version
- Release date
- Summary
- Important changes
- Validation status
- Known limitations
- Relevant issue or PR references where useful

## 8. Security

Never include in release notes or artifacts:

- Passwords
- API keys
- Access tokens
- Private keys
- Environment secrets
- Customer credentials
- Confidential partner information
- Sensitive personal information

If secret exposure is detected, release publication must stop until the
incident is handled.

## 9. Release Approval

A release should have appropriate technical review before publication.

Higher-risk or public releases may require additional technical,
governance, publication, or operational approval.

## 10. Bad Release / Correction Procedure

If a released version contains a defect:

1. Identify the affected version.
2. Assess technical and security impact.
3. Create a remediation issue.
4. Fix the problem through the normal PR workflow.
5. Run required CI and security validation.
6. Create a new PATCH or appropriate version.
7. Document the correction in CHANGELOG.md and release notes.

Do not silently modify an already published release tag to point at
different source code.

## 11. Evidence

Each release should be traceable through:

- Version
- Git tag
- Commit SHA
- Pull request
- CI/release workflow run
- GitHub Release URL
- Reviewer/approval evidence
