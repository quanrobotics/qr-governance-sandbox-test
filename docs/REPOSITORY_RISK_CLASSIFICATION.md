# QuanRobotics Repository Risk Classification

## Risk Levels

### LOW
Public documentation, examples, governance tests, non-confidential demos.

### MEDIUM
Engineering utilities and internal tooling without sensitive credentials,
proprietary algorithms, customer data, or confidential research.

### HIGH
Core robotics software, QR-Core, QR-Sim, QR-Perception,
QR-RobotData, infrastructure configuration, CI/CD configuration,
deployment code, model weights, datasets, authentication,
security configuration, or unpublished research.

### CRITICAL
Credentials, production secrets, highly sensitive partner/customer data,
regulated data, production signing material, or highly restricted intellectual property.

Critical secrets must not be committed to Git repositories.

## Current Repository Register

| Repository | Default Branch | Visibility | Risk | Confidential Code |
|---|---|---|---|---|
| qr-governance-sandbox | main | Public | Low | Prohibited |

## Governance Rule

Any future QuanRobotics repository must be classified before active development begins.
