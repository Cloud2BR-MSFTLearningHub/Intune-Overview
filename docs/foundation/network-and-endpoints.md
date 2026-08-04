# Intune Network and Endpoints

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Network endpoints for Intune](https://learn.microsoft.com/en-us/intune/fundamentals/endpoints)
- [Windows Autopilot network requirements](https://learn.microsoft.com/en-us/autopilot/networking-requirements)

</details>

## Objective

Ensure device-to-cloud communication works for enrollment, policy check-in, app
delivery, updates, and security signals across all managed environments.

## Core endpoint categories

| Category | Examples |
| --- | --- |
| Intune core service | `*.manage.microsoft.com`, `*.dm.microsoft.com` |
| Identity dependencies | `login.microsoftonline.com` |
| Device actions and notifications | WNS (Windows Push Notification Services), platform push services |
| App and script delivery | Intune management extension and content delivery endpoints |
| Autopilot and provisioning | Windows update and enrollment dependencies |

## Network design requirements

- Allow required outbound traffic over TCP (transmission control protocol) 443 (and 80 where required).
- Avoid SSL (secure sockets layer) inspection on endpoints where Microsoft states inspection is unsupported.
- Validate proxy behavior for device and system contexts.
- Include regional endpoints for macOS scripts and Win32 content where applicable.

## Validation checklist

- [ ] Enrollment succeeds from corporate and remote networks.
- [ ] Device sync and immediate actions complete successfully.
- [ ] Win32 and script content delivery works in each region.
- [ ] Autopilot provisioning completes without endpoint blocking.
- [ ] Firewall and proxy owners maintain endpoint review cadence.

## Common failure patterns

- Network teams allow identity endpoints but block Intune content delivery endpoints.
- SSL (secure sockets layer) inspection interrupts enrollment, attestation, or Defender-dependent traffic.
- Regional CDN (content delivery network) endpoints are omitted for globally distributed tenants.