# BWNFiber SEO and conversion roadmap

## Status

**Proposed for review; not approved for implementation.** This roadmap is based only on the repository audit in `AUDIT.md`. It does not assert that any listed product category or website issue exists. Do not implement site changes until the owner approves the audit and plan and supplies the required access and evidence.

## Prioritized plan

| Priority / phase | Work and expected business impact | Dependencies | Acceptance criteria |
| --- | --- | --- | --- |
| P0 — Confirm scope and baseline | Identify the authoritative WordPress code repository, site owner, staging environment, deployment/rollback process, and approved access. Preserve current behavior before proposing modifications. | Owner approval; authorized access; verified backup and rollback path. | Scope and environment are documented; staging is available; baseline URLs and current deployment revision are recorded; no production changes are made. |
| P1 — Gather evidence | Crawl authorized pages and collect sitemap/robots/canonical/status data, Search Console and analytics exports, and inquiry-form journey evidence. Establish technical and conversion baselines. | P0; permissioned datasets and test inquiry process. | Each finding has a URL or data source, observation date, impact, priority, and reproducible verification; unknowns remain explicitly labeled. |
| P1 — Product and keyword mapping | Verify existing category/product URLs and search intent for patch cords, hardened connector patch cords, outdoor cables, pre-terminated assemblies, PLC splitters/ODN, MPO/MTP, distribution frames/patch panels, transceivers, DAC, and AOC. Identify gaps and possible cannibalization. | URL inventory; crawl and Search Console evidence; approved product documentation and claims. | Every proposed target maps to a verified existing URL or is explicitly labeled a proposed page; no specification, certification, capability, lead time, or performance claim is invented. |
| P1 — Conversion journey | Evaluate product discovery, specification readability, technical resources, RFQ/contact calls to action, form usability, and mobile/error/success states for telecom engineers, integrators, distributors, and procurement buyers. | Staging access; approved form submissions; product documentation. | Representative desktop and mobile journeys are documented; proposed form/page changes have observable acceptance criteria and an approved rollback. |
| P2 — Technical and content recommendations | Prioritize fixes to metadata, headings, canonical/indexability, internal links, breadcrumbs, applicable structured data, images, accessibility, performance, and duplicate/broken content. Respect existing SEO-plugin responsibilities. | P1 evidence; approved scope; source code and plugin configuration; owner review. | Each recommendation names affected URLs/files, expected behavior, test method, dependencies, and risks; proposed structured data is valid and not duplicated. |
| P2 — Staged implementation and QA | If approved, make small reversible changes in the authorized codebase and verify them in staging before any separately approved deployment. | Explicit implementation approval; backups; access to staging; defined tests. | Existing important URLs remain available and intentionally indexable; no redirect/canonical conflicts, broken links, PHP/JS errors, form regressions, or material performance regressions are introduced; rollback is tested. |
| P3 — Measure outcomes | Compare qualified organic traffic, target-page visibility, and qualified inquiry outcomes with the baseline without promising rankings or leads. | Deployed changes; permissioned Search Console, analytics, and CRM/inquiry data. | Measurement window, metrics, and attribution limits are documented; results are reported as observed, not guaranteed. |

## Required deliverables after evidence and approval

Do not create empty reports or fabricate mappings. Produce these when the corresponding evidence exists:

- `KEYWORD-MAP.md`: verified search intent mapped to crawled existing URLs, with proposed URLs clearly distinguished.
- `CONVERSION-PLAN.md`: evidence-backed product-page and inquiry-flow observations and recommendations.
- `TEST-PLAN.md`: change-specific acceptance checks, regression checks, and staging/rollback procedure.
- `CHANGELOG.md`: actual approved code/configuration changes only.
- `ROLLBACK.md`: recovery steps tied to the verified deployment mechanism.

`AUDIT.md` and this roadmap can be reviewed now; the remaining documents depend on site, product, or implementation evidence.

## Open questions for the owner

1. Which repository and environment contain the authorized WordPress implementation?
2. Is there a staging site, and what is the approved deployment and rollback process?
3. Can the team provide a current URL inventory, Search Console/analytics exports, and representative inquiry-flow access?
4. Which product categories are live, and where are the approved specifications, certifications, capabilities, and claims documented?
5. Which SEO plugin and form system are in use, and who approves changes to their configuration?
