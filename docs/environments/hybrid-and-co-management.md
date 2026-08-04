# Hybrid and Co-Management

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Migration guide to Intune](https://learn.microsoft.com/en-us/intune/fundamentals/setup-migration)
- [Planning guide to Intune](https://learn.microsoft.com/en-us/intune/fundamentals/planning-guide)
- [What is co-management?](https://learn.microsoft.com/en-us/intune/configmgr/comanage/overview)

</details>

## Strategy

Hybrid estates should move intentionally from legacy management stacks to cloud
management while preserving business continuity and supportability.

## Hybrid pathways

| Pathway | Best fit |
| --- | --- |
| Tenant attach | Need cloud visibility and actions while retaining ConfigMgr authority |
| Co-management | Split workload authority between ConfigMgr and Intune |
| Full migration | Long-term cloud-native endpoint target state |

## Migration checkpoints

1. Baseline current policies, app dependencies, and operational processes.
2. Identify workload transition order (compliance, configuration, updates, apps).
3. Pilot phased workload movement and validate user impact.
4. Retire legacy controls only after equivalent cloud controls are proven.

## Risks and controls

- Policy conflicts between legacy and cloud controls.
- Incomplete app packaging and detection logic during transition.
- Support confusion on authority boundaries.

Define ownership boundaries clearly for each workload at each migration stage.