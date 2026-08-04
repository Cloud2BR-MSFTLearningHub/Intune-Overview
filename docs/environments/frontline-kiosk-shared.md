# Frontline, Kiosk, and Shared Devices

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Planning guide: frontline worker devices](https://learn.microsoft.com/en-us/intune/fundamentals/planning-guide#frontline-worker-flw-devices)
- [Android enrollment guide](https://learn.microsoft.com/en-us/intune/device-enrollment/android/guide)

</details>

## Strategy

Frontline and shared device programs should optimize reliability, constrained
access, and fast recoverability over broad end-user customization.

## Common scenarios

| Scenario | Management model |
| --- | --- |
| Shared shift tablets | Shared profile or userless enrollment where supported |
| Kiosk signage and terminals | Dedicated or kiosk enrollment with app allowlist |
| Scanner and warehouse devices | Corporate-managed restricted profile with targeted apps |

## Control priorities

- Restrict app surface to approved workflow apps.
- Configure automatic sign-in or managed identity patterns as needed.
- Enforce network, update, and patching windows aligned to operations.
- Provide rapid reset and reprovisioning paths.

## Governance model

1. Define device persona and critical workflows.
2. Build persona-specific baseline profile.
3. Validate offline, low-bandwidth, and shift-change behavior.
4. Implement replacement and incident playbooks.

## Field support recommendations

- Maintain spare device inventory and pre-staged profiles.
- Document tier-1 troubleshooting paths for connectivity and app failures.
- Track uptime and incident category trends by location.