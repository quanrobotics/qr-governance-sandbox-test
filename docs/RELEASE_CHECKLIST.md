# QuanRobotics Release Checklist

## Version

- [ ] Release version confirmed
- [ ] Version follows vMAJOR.MINOR.PATCH
- [ ] Version has not already been released

## Source

- [ ] Release source is reviewed
- [ ] Release commit is identified
- [ ] Required pull request is merged
- [ ] No unreviewed experimental code is included

## Quality

- [ ] Tests pass
- [ ] CI passes
- [ ] Required status checks pass
- [ ] Known regressions are documented

## Security

- [ ] Secret/security checks pass
- [ ] Dependency audit passes
- [ ] No unresolved Critical vulnerabilities
- [ ] High-risk findings are resolved or approved
- [ ] No credentials or confidential data are included

## Documentation

- [ ] CHANGELOG.md updated
- [ ] README/docs updated where necessary
- [ ] Known limitations documented
- [ ] Release notes prepared

## Approval

- [ ] Engineering review complete
- [ ] Additional technical/governance approval complete where required

## Release

- [ ] Git tag created
- [ ] Release workflow passes
- [ ] GitHub Release created
- [ ] Release points to expected tag
- [ ] Tag resolves to expected commit SHA

## Evidence

- [ ] Tag URL recorded
- [ ] Commit SHA recorded
- [ ] Workflow URL recorded
- [ ] Release URL recorded
- [ ] Reviewer evidence recorded

## Post-Release

- [ ] Release page checked
- [ ] Documentation links checked
- [ ] No unexpected artifacts published
- [ ] Tracker updated
