# Tenant Setup and Baseline

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Get started with Intune](https://learn.microsoft.com/en-us/intune/fundamentals/get-started)
- [Planning guide](https://learn.microsoft.com/en-us/intune/fundamentals/planning-guide)

</details>

## Objective

Establish tenant-wide readiness and governance controls before assigning platform
policies at scale.

## Baseline setup steps

1. Confirm tenant roles, role-based access control, and operational ownership.
2. Define group structure for users, devices, and environment segmentation.
3. Configure naming standards and policy documentation format.
4. Build baseline policy rings for pilot, pre-production, and production.
5. Set compliance policy settings to align with Conditional Access intent.

## Governance controls

| Control area | Baseline recommendation |
| --- | --- |
| RBAC | Least privilege with scoped admin boundaries |
| Scope tags | Distributed administration model where needed |
| Group strategy | Clear separation of user and device assignment groups |
| Change management | Versioned policy change logs and approval flow |

## Readiness checklist

- [ ] Group and assignment design approved.
- [ ] Pilot rings and success criteria documented.
- [ ] Support and escalation paths agreed.
- [ ] Reporting baseline dashboards identified.