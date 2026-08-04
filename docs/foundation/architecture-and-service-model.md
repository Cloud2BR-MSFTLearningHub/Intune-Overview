# Intune Architecture and Service Model

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [What is Microsoft Intune?](https://learn.microsoft.com/en-us/intune/fundamentals/what-is-intune)
- [Intune core concepts](https://learn.microsoft.com/en-us/intune/fundamentals/core-concepts)
- [Conditional Access with Intune](https://learn.microsoft.com/en-us/intune/device-security/conditional-access-integration/overview)

</details>

## Design objective

Define a cloud-first endpoint control plane that aligns identity, device, app,
and data posture in one operating model.

![Microsoft Intune service model from Microsoft Learn](https://learn.microsoft.com/en-us/intune/fundamentals/media/shared/intune-overview.png)

*Source: [What is Microsoft Intune?](https://learn.microsoft.com/en-us/intune/fundamentals/what-is-intune).* 

## Core pillars

| Pillar | Purpose |
| --- | --- |
| Identity | Authenticate users and define access trust context |
| Devices | Enroll and evaluate endpoint posture |
| Apps | Deliver and protect productivity and business apps |
| Access control | Enforce Conditional Access using compliance and risk signals |
| Operations | Monitor health, enforce governance, and continuously improve |

## MDM (mobile device management) and MAM (mobile application management) strategy

- MDM (mobile device management): full device control, preferred for corporate-owned endpoints.
- MAM (mobile application management): app and data protection without full device management, preferred for BYOD (bring your own device).
- Combined mode: full device management plus app protection for high-sensitivity workloads.

## Control boundaries

1. Identity and group model in Microsoft Entra.
2. Device ownership and enrollment model per platform.
3. App protection and data movement restrictions.
4. Compliance state and access enforcement model.
5. Support and remediation ownership model.

## Architecture anti-patterns

- One global policy ring for every device type.
- Treating BYOD (bring your own device) and corporate-owned as equivalent risk models.
- Applying blocking Conditional Access before compliance and remediation workflows are stable.
- Skipping pilot validation for network, enrollment, and app delivery dependencies.