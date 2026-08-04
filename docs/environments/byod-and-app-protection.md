# BYOD (bring your own device) and App Protection

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [What is Intune? MDM (mobile device management) and MAM (mobile application management) model](https://learn.microsoft.com/en-us/intune/fundamentals/what-is-intune)
- [Planning guide: personal vs organization-owned devices](https://learn.microsoft.com/en-us/intune/fundamentals/planning-guide#personal-devices-vs-organization-owned-devices)
- [Add apps to Intune](https://learn.microsoft.com/en-us/intune/app-management/deployment/)

</details>

## Strategy

BYOD (bring your own device) programs should prioritize data protection, identity trust, and user
experience without overreaching into personal device control.

## Recommended model

1. Use app protection policies for Microsoft 365 and approved line-of-business apps.
2. Enforce Conditional Access for approved apps and risk posture.
3. Apply app configuration policies for consistent app behavior.
4. Use selective wipe for corporate data lifecycle events.

## Control matrix

| Control area | Recommended baseline |
| --- | --- |
| Access | Require multifactor authentication and trusted app context |
| Data movement | Restrict copy/paste and save-as to managed apps or locations |
| Session control | Require app PIN (personal identification number) and inactivity timeout where appropriate |
| Device trust | Use device or app-level controls based on risk and legal constraints |

## Rollout sequence

- Pilot with mobile-first users.
- Validate mail, files, collaboration, and line-of-business app scenarios.
- Socialize privacy boundaries clearly to users.
- Expand by business unit once support volume stabilizes.

## Risks to mitigate

- Overly restrictive controls that break business workflows.
- Unclear user communication around what IT can and cannot see.
- Inconsistent policy scope between app protection and Conditional Access.