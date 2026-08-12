# Contract discovery — Epic Bio

**Result: no machine-readable contract exists.** Recorded 2026-08-12 after the full
STEP 0b contract-discovery sweep, not after a single docs-host check.

Epic Bio is the operating name of **Epicrispr Biotechnologies, Inc.** — a clinical-stage
epigenetic-editing therapeutics company. Its only public host is the corporate WordPress
site at `epicrispr.com` (WP Engine origin behind Cloudflare). There is no API host, no
developer subdomain, and no GitHub organization.

| Probe | URL | Status |
|---|---|---|
| REST OpenAPI | `https://epicrispr.com/openapi.json` | 404 |
| REST OpenAPI | `https://epicrispr.com/openapi.yaml` | 404 |
| Swagger | `https://epicrispr.com/swagger.json` | 404 |
| Versioned spec | `https://epicrispr.com/v1/openapi.json` | 404 |
| Spec UI | `https://epicrispr.com/api-docs` | 404 |
| Docs | `https://epicrispr.com/docs` | 404 |
| Redoc | `https://epicrispr.com/redoc` | 404 |
| GraphQL | `https://epicrispr.com/graphql` | 404 |
| A2A agent card | `https://epicrispr.com/.well-known/agent-card.json` | 404 |
| A2A legacy card | `https://epicrispr.com/.well-known/agent.json` | 404 |
| llms.txt | `https://epicrispr.com/llms.txt` | 404 |
| API host | `https://api.epicrispr.com/` | DNS NXDOMAIN |
| Developer host | `https://developer.epicrispr.com/` | DNS NXDOMAIN |
| Docs host | `https://docs.epicrispr.com/` | DNS NXDOMAIN |
| GitHub org | `https://github.com/epicrispr` | 404 |
| GitHub org | `https://github.com/epic-bio` | 404 |
| GitHub org | `https://github.com/epicbio` | 404 |

**Name collision warning.** Two unrelated surfaces answer to similar names and must not be
attributed to this company:

- `epic.bio` / `www.epic.bio` returns **200** but is a **Guerbet** product login portal
  ("Epic" by Guerbet, support `contact@digitalis-cdc.com`), not Epicrispr Biotechnologies.
- `open.epic.com` / `vendorservices.epic.com` belong to **Epic Systems** (the healthcare
  EHR vendor). Their FHIR APIs are a different company entirely.

The company's own `platform/` page describes "proprietary computational and experimental
methods" for guide-RNA design, but these are internal R&D tooling — nothing is exposed
publicly as an API, SDK, dataset, or specification.
