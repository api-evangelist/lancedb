# LanceDB

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
