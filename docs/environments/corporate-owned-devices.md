# Corporate-Owned Device Management

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Enroll devices in Intune](https://learn.microsoft.com/en-us/intune/device-enrollment/enroll-devices)
- [Configure device profiles](https://learn.microsoft.com/en-us/intune/device-configuration/create-device-profile)
- [Compliance policies](https://learn.microsoft.com/en-us/intune/device-security/compliance/overview)

</details>

## Strategy

Corporate-owned endpoints should use full device enrollment, policy baselines,
and lifecycle controls aligned to platform and ownership class.

## Platform enrollment patterns

| Platform | Typical enrollment |
| --- | --- |
| Windows | Entra join with automatic enrollment, Autopilot, or co-management |
| iOS/iPadOS | Automated Device Enrollment or Apple Configurator pathways |
| macOS | Automated Device Enrollment or Company Portal for user-driven models |
| Android Enterprise | Fully managed, corporate-owned work profile, or dedicated modes |

## Baseline controls

- Compliance policies aligned to OS, encryption, and security-state requirements.
- Configuration profiles for device restrictions, network, and settings catalog controls.
- Security baselines where available and appropriate.
- App lifecycle policies for required, available, and uninstall intents.

## Corporate lifecycle model

1. Provision and enroll.
2. Apply baseline policy set.
3. Validate compliance and app readiness.
4. Operate and monitor.
5. Retire, wipe, or repurpose securely.

## Operational checks

- [ ] Enrollment completion and policy check-in rates meet target.
- [ ] Compliance posture remains stable after update cycles.
- [ ] Critical app install success remains within defined service objectives.
- [ ] Device retirement workflow is tested and auditable.