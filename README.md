# Latent

Latent (Latent Health) is an enterprise pharmacy intelligence platform for health systems, powered by a clinical agentic engine that reads the chart, reasons over payer policy and drug labels, and acts inside the EHR. The platform spans four modules — **Identify** (care-gap identification, eligibility screening, site-of-care routing), **Access** (prior authorization, clinical review, appeals generation, benefit routing, payer outreach), **Capture** (340B eligibility auditing, leakage analytics, financial dashboards), and **Engage** (patient outreach, queue management, outcomes analytics).

Latent is chart-native and EHR agnostic (Epic, Cerner and others), used by 45+ health systems including Ochsner Health, MetroHealth, Yale New Haven Health, St. Luke's Health System and Henry Ford Health, serving more than two million patients annually. Founded by Sriram Somasundaram and Rishabh Jain; $80M raised from Spark Capital, Transformation Capital, McKesson Ventures, Conviction, General Catalyst and Y Combinator.

- Website — https://latenthealth.com
- Platform — https://latenthealth.com/platform
- Trust Center — https://security.latenthealth.com

## API surface

**Latent publishes no public developer API.** As of 2026-07-19 there is no developer portal, API reference, OpenAPI/AsyncAPI specification, SDK or package, MCP server, CLI, sandbox, status page, or public changelog. No `/.well-known/` discovery documents are served. Integration is delivered EHR-natively under health-system contracts.

Artifacts in this repo reflect what Latent genuinely publishes:

| Artifact | Method |
|---|---|
| `security/latent-domain-security.yml` | probed (TLS 1.3, HSTS, DNSSEC, CAA, SPF, DMARC quarantine) |
| `security/latent-trust-center.yml` | searched (Vanta-hosted, HIPAA) |
| `conformance/latent-conformance.yml` | searched (HIPAA published; SOC 2/ISO/HITRUST unknown) |
| `well-known/latent-well-known.yml` | searched (all 404 — recorded as valid absence) |
| `llms/latent-llms.txt` | generated |

Backed by: spark-capital
