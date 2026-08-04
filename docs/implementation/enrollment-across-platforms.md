# Enrollment Across Platforms

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Enroll devices in Intune](https://learn.microsoft.com/en-us/intune/device-enrollment/enroll-devices)
- [Intune enrollment guide](https://learn.microsoft.com/en-us/intune/device-enrollment/guide)

</details>

## Enrollment principles

- Start with pilots and staged rings.
- Align enrollment path with ownership and platform reality.
- Prepare pre-enrollment settings before broad rollout.

![Intune enrollment deployment diagram from Microsoft Learn](https://learn.microsoft.com/en-us/intune/device-enrollment/media/enroll-devices/deployment-plan-enroll.png)

*Source: [Enroll devices in Microsoft Intune](https://learn.microsoft.com/en-us/intune/device-enrollment/enroll-devices).* 

## Platform pathways

| Platform | BYOD option | Corporate option |
| --- | --- | --- |
| Android | Personally owned work profile | Corporate-owned work profile, fully managed, dedicated, AOSP |
| iOS/iPadOS | User enrollment or device enrollment | Automated Device Enrollment or Configurator |
| macOS | Company Portal user-driven enrollment | Automated Device Enrollment or direct provisioning |
| Windows | Work account connect or Company Portal | Entra join, Autopilot, co-management, provisioning package |
| Linux | User enrollment with supported scenarios | Organization-managed Linux design as applicable |

## Pre-enrollment controls

- Enrollment restrictions.
- Device category strategy.
- Terms and conditions and/or Entra terms.
- Multifactor authentication requirements.
- Device enrollment manager usage for high-volume provisioning.

## Enrollment success indicators

- Completion rate by platform and method.
- Time-to-productive-device metrics.
- Abandoned enrollment trend.
- Top failure causes and remediation time.