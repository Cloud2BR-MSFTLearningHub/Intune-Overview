# Compliance and Conditional Access

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

<details markdown>
<summary>References</summary>

- [Device compliance policies](https://learn.microsoft.com/en-us/intune/device-security/compliance/overview)
- [Conditional Access integration](https://learn.microsoft.com/en-us/intune/device-security/conditional-access-integration/overview)

</details>

## Objective

Use device compliance as a trusted signal to enforce access policy consistently
across apps and resources.

## Tenant-wide compliance settings

A critical setting is how devices with no compliance policy are treated.

- Strong security posture generally requires setting this state to not compliant.
- Combine with a scoped pilot to avoid accidental broad access disruption.

## Policy model

1. Create platform-specific compliance policies.
2. Define actions for noncompliance and user notifications.
3. Integrate compliance signals with Conditional Access.
4. Validate remediation flow in Company Portal before broad enforcement.

## Design checklist

- [ ] Every in-scope platform has a baseline compliance policy.
- [ ] Exceptions are documented and time-bound.
- [ ] Conditional Access dependencies are tested with pilot users.
- [ ] Helpdesk has compliant/noncompliant remediation runbooks.

## Common pitfalls

- Enforcing Conditional Access before devices are properly scoped to compliance policies.
- Relying on one policy for all platforms without platform-specific controls.
- Missing user guidance for remediation actions.