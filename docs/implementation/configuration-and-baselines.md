# Configuration Profiles and Security Baselines

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Configure device configuration profiles](https://learn.microsoft.com/en-us/intune/device-configuration/create-device-profile)
- [Security baselines in Intune](https://learn.microsoft.com/en-us/intune/device-security/security-baselines/overview)

</details>

## Strategy

Use a layered policy design with clear purpose by profile type.

## Profile design layers

| Layer | Purpose |
| --- | --- |
| Security baseline | Fast adoption of vetted baseline controls |
| Settings catalog profiles | Granular configuration for targeted requirements |
| Template profiles | Scenario-based controls like VPN (virtual private network), Wi-Fi, kiosk, certificates |
| Applicability rules | Refine policy scope for specific Windows editions/versions |

## Implementation sequence

1. Deploy foundational baselines to pilot rings.
2. Add settings catalog profiles for business and security requirements.
3. Use templates for network, certificates, email, and device restrictions.
4. Validate conflict behavior and assignment overlap.

![Windows profile creation experience from Microsoft Learn](https://learn.microsoft.com/en-us/intune/device-configuration/media/create-device-profile/windows-create-device-profile.png)

*Source: [Configure device configuration profiles](https://learn.microsoft.com/en-us/intune/device-configuration/create-device-profile).* 

## Policy quality standards

- Descriptive naming convention.
- Scope alignment to user or device assignment intent.
- Conflict checks before promotion to production rings.
- Documented rollback pattern for every high-impact policy.