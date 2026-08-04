# Intune Overview

Atlanta, USA

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR OSS - Learning Hub](https://github.com/Cloud2BR-MSFTLearningHub)

Last updated: 2026-08-04

----------

Comprehensive documentation hub for planning, deploying, securing, and operating
Microsoft Intune across BYOD, corporate-owned, frontline/shared, and hybrid
environments.

## Documentation site (GitHub Pages)

- Site URL: https://cloud2br-msftlearninghub.github.io/Intune-Overview/

## Scope

- Intune architecture and service model
- Planning, migration, and licensing
- Network and endpoint prerequisites
- Enrollment across platforms and ownership types
- Compliance and Conditional Access
- Configuration profiles and security baselines
- Apps, app protection, and lifecycle operations
- Reporting, rollout governance, and helpdesk readiness

## Repository layout

| File or folder | Purpose |
| --- | --- |
| `mkdocs.yml` | Site metadata, navigation, and theme configuration for the Intune documentation hub. |
| `requirements.txt` | MkDocs Material dependencies used for build and local authoring. |
| `docs/` | Published documentation pages for setup guidance and operations. |
| `.github/workflows/deploy-github-pages.yml` | Build and deploy workflow for GitHub Pages. |

## Local build

```bash
pip install -r requirements.txt
mkdocs build --strict
mkdocs serve
```

## Contribution standards

- Keep page headers aligned with org requirements.
- Use authoritative Microsoft Learn references for technical claims.
- Add new pages to `mkdocs.yml` navigation.
- Validate with `mkdocs build --strict` before committing.

<!-- START BADGE -->
<div align="center">
  <img src="https://img.shields.io/badge/Total%20views-40-limegreen" alt="Total views">
  <p>Refresh Date: 2026-04-07</p>
</div>
<!-- END BADGE -->
