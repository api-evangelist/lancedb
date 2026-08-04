# LanceDB

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

> The AI-Native multimodal lakehouse built on the open-source Lance columnar storage format.

LanceDB pairs an Apache 2.0 licensed embedded retrieval library (Python, TypeScript, Rust, Go, C, Java) with a managed cloud service (LanceDB Cloud) and an enterprise lakehouse (LanceDB Enterprise). It unifies vector, full-text, hybrid, and SQL search across billions of multimodal records.

This repository is the API Evangelist catalog entry for LanceDB. It captures the provider's machine-readable APIs.json profile, the canonical Lance Namespace REST OpenAPI spec, capability definitions, schemas, examples, vocabulary, Spectral rules, plans, rate limits, and FinOps mapping.

## Surface area covered

- **LanceDB OSS** — Apache 2.0 embedded library, [github.com/lancedb/lancedb](https://github.com/lancedb/lancedb) (10.4k stars).
- **LanceDB Cloud** — managed serverless service exposing the Lance Namespace REST API.
- **LanceDB Enterprise** — distributed multimodal lakehouse with GPU-accelerated index build (cuVS), materialized views, Python UDF feature engineering, and PyTorch / Ray training integration. Deployable in customer VPC on AWS, GCP, or Azure.
- **Lance Format** — Apache 2.0 columnar Parquet replacement at [lance.org](https://lance.org/) and [github.com/lance-format/lance](https://github.com/lance-format/lance) (6.5k stars).
- **Lance Namespace Spec** — open OpenAPI 3.1 contract at [github.com/lance-format/lance-namespace](https://github.com/lance-format/lance-namespace) with reference implementations for Apache Hive, Apache Polaris, Apache Gravitino, Unity Catalog, and AWS Glue.
- **SDKs** — Python, TypeScript, Rust, Go, C, plus an MCP server.

## Repository contents

| Path | What it contains |
|---|---|
| `apis.yml` | APIs.json 0.20 profile listing every LanceDB API, SDK, and surface, plus integrations and use cases. |
| `openapi/lance-namespace-openapi.yaml` | Canonical Lance Namespace OpenAPI 3.1 spec mirrored from `lance-format/lance-namespace`. 50+ operations across namespaces, tables, indices, tags, transactions, and materialized views. |
| `capabilities/shared/lancedb-rest.yaml` | Per-API shared capability bundle for the REST surface. |
| `capabilities/multimodal-retrieval.yaml` | Workflow capability: provision namespace, declare table, upsert, build indexes, hybrid-query, pin reproducibility tag. |
| `capabilities/training-curation.yaml` | Workflow capability: dedupe, score, snapshot, and tag a training corpus. |
| `json-schema/` | JSON Schemas for the Table, Query, and Namespace resources. |
| `json-structure/` | JSON Structure (typed) variant of the Table schema. |
| `json-ld/lancedb-context.jsonld` | JSON-LD context mapping LanceDB concepts to schema.org and the LanceDB vocabulary. |
| `examples/` | Realistic request payloads: create table, hybrid query, vector index, merge-insert, create tag. |
| `vocabulary/lancedb-vocabulary.yml` | Domain vocabulary covering namespaces, tables, indexes, search modes, embedding providers, and operations. |
| `rules/lancedb-rules.yml` | Spectral ruleset enforcing Lance Namespace conventions (path prefixes, tag enums, operationId casing, security, error shape). |
| `plans/lancedb-plans-pricing.yml` | API Commons Plans 0.1 capturing OSS, Cloud Free, Cloud Business, and Enterprise tiers. |
| `rate-limits/lancedb-rate-limits.yml` | API Commons Rate Limits 0.1 capturing the per-tier rate posture. |
| `finops/lancedb-finops.yml` | FinOps Framework / FOCUS 1.1 mapping of LanceDB's billable entities and cost allocation dimensions. |

## Quick links

- Website — [lancedb.com](https://lancedb.com/)
- Documentation — [docs.lancedb.com](https://docs.lancedb.com/)
- llms.txt — [docs.lancedb.com/llms.txt](https://docs.lancedb.com/llms.txt)
- GitHub (product) — [github.com/lancedb](https://github.com/lancedb)
- GitHub (format) — [github.com/lance-format](https://github.com/lance-format)
- Trust Center — [trust.lancedb.com](https://trust.lancedb.com/)
- Discord — [discord.com/invite/G5DcmnZWKB](https://discord.com/invite/G5DcmnZWKB)

## Notes

- The Lance Namespace OpenAPI is authoritative; this repo mirrors the upstream `docs/src/spec.yaml` and references it as the canonical contract.
- Plans, rate limits, and FinOps reflect the public posture (free tier + contact-sales business + annual enterprise contract). Where LanceDB does not publish list prices, the value is marked `contact-sales`.
- LanceDB is headquartered in San Francisco. Series A ($30M) closed in 2025.

## License

Catalog files in this repository are CC BY 4.0 unless noted otherwise. The mirrored Lance Namespace OpenAPI spec retains its upstream Apache 2.0 license header.
