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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LanceDB is the AI-Native multimodal lakehouse built on the open-source Lance columnar storage format. It pairs an Apache 2.0 licensed embedded retrieval library (Python, TypeScript, Rust, Go, C, Java SDKs) with a managed cloud service (LanceDB Cloud) and an enterprise lakehouse (LanceDB Enterprise) that unify vector, full-text, hybrid, and SQL search across billions of multimodal records. The REST surface is governed by the open Lance Namespace specification (OpenAPI 3.1) covering namespace, table, index, tag, and transaction operations with first-class support for materialized views, schema evolution, and time-travel versioning. LanceDB is used in production by Midjourney, Runway, World Labs, Netflix, Character.AI, Uber, NVIDIA, ByteDance, Databricks, and others for RAG, agent memory, training data curation, feature engineering, and large-scale retrieval.

**Areas:** Vector Search · Multi-Modal · Lance Format · Lakehouse · RAG · Agent Memory · Open Source · Embeddings · Full-Text Search · Hybrid Search · Columnar Storage · Arrow

## LanceDB on APIs.io

Everything profiled for LanceDB is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/lancedb/](https://apis.io/providers/lancedb/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [LanceDB Enterprise](https://apis.io/apis/lancedb/enterprise/) — Distributed, multi-tenant multimodal lakehouse. Adds curation and deduplication, Python UDF feature engineering, materialized views, GPU-accelerated index…
- [Lance Format](https://apis.io/apis/lancedb/lance-format/) — Apache 2.0 open lakehouse format for multimodal AI. Columnar Parquet replacement offering 100x faster random access, zero-copy reads, vector indexes, and…
- [LanceDB Python SDK](https://apis.io/apis/lancedb/python-sdk/) — Primary client library. First-class Arrow, Pandas, Polars, and Pydantic integration; pluggable embedding functions covering OpenAI, Cohere, Jina, Hugging…
- [LanceDB TypeScript SDK](https://apis.io/apis/lancedb/typescript-sdk/) — Node.js / TypeScript / JavaScript client library for LanceDB OSS, Cloud, and Enterprise. Bundles native bindings via napi-rs.
- [LanceDB Rust SDK](https://apis.io/apis/lancedb/rust-sdk/) — Native Rust client library; the LanceDB core and storage layer are written in Rust.
- [LanceDB Go SDK](https://apis.io/apis/lancedb/go-sdk/) — Official Go client library for LanceDB OSS, Cloud, and Enterprise.
- [LanceDB C Bindings](https://apis.io/apis/lancedb/c-sdk/) — C ABI bindings for LanceDB enabling embedding into C, C++, and other FFI-capable hosts.
- [LanceDB MCP Server](https://apis.io/apis/lancedb/mcp-server/) — Model Context Protocol (MCP) server exposing LanceDB tables as retrieval tools for MCP-aware agents and IDEs.
- [LanceDB MaterializedView API](https://apis.io/apis/lancedb/lancedb-materializedview-api/) — The MaterializedView API from LanceDB — 2 operation(s) for materializedview.
- [LanceDB Namespace API](https://apis.io/apis/lancedb/lancedb-namespace-api/) — Operations that are related to a namespace
- [LanceDB Table API](https://apis.io/apis/lancedb/lancedb-table-api/) — Operations that are related to a table
- [LanceDB Transaction API](https://apis.io/apis/lancedb/lancedb-transaction-api/) — Operations that are related to a transaction

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Lancedb Agentic Access](https://apis.io/agentic-access/lancedb/lancedb-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Lance Namespace](https://apis.io/schemas/lancedb/lancedb-namespace/)
- [LanceDB Query Request](https://apis.io/schemas/lancedb/lancedb-query/)
- [LanceDB Table](https://apis.io/schemas/lancedb/lancedb-table/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Lancedb Table Structure](https://apis.io/json-structure/lancedb/lancedb-table-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Lancedb Context](https://apis.io/jsonld/lancedb/lancedb-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Lancedb Vocabulary](https://apis.io/vocabularies/lancedb/lancedb-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Lancedb Create Table Example](https://apis.io/examples/lancedb/lancedb-create-table-example/)
- [Lancedb Create Tag Example](https://apis.io/examples/lancedb/lancedb-create-tag-example/)
- [Lancedb Create Vector Index Example](https://apis.io/examples/lancedb/lancedb-create-vector-index-example/)
- [Lancedb Hybrid Query Example](https://apis.io/examples/lancedb/lancedb-hybrid-query-example/)
- [Lancedb Merge Insert Example](https://apis.io/examples/lancedb/lancedb-merge-insert-example/)

#### Collections (8)

Postman and Open Collection request collections.

- [Lance Namespace Specification Data API](https://apis.io/collections/lancedb/open-lancedb-data-api/)
- [Lance Namespace Specification Data Index API](https://apis.io/collections/lancedb/open-lancedb-index-api/)
- [Lance Namespace Specification Data MaterializedView API](https://apis.io/collections/lancedb/open-lancedb-materializedview-api/)
- [Lance Namespace Specification Data Metadata API](https://apis.io/collections/lancedb/open-lancedb-metadata-api/)
- [Lance Specification Data Namespace API](https://apis.io/collections/lancedb/open-lancedb-namespace-api/)
- [Lance Namespace Specification Data Table API](https://apis.io/collections/lancedb/open-lancedb-table-api/)
- [Lance Namespace Specification Data Tag API](https://apis.io/collections/lancedb/open-lancedb-tag-api/)
- [Lance Namespace Specification Data Transaction API](https://apis.io/collections/lancedb/open-lancedb-transaction-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [LanceDB — jsonschema rules](https://apis.io/rules/lancedb/lancedb-jsonschema-spectral-rules/)
- [LanceDB API Rules](https://apis.io/rules/lancedb/lancedb-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Lancedb Authentication](https://apis.io/security/lancedb/lancedb-authentication/)
- [Lancedb Domain Security](https://apis.io/security/lancedb/lancedb-domain-security/)
- [Lancedb Trust Center](https://apis.io/security/lancedb/lancedb-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Lancedb Scopes](https://apis.io/scopes/lancedb/lancedb-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Lancedb Plans Pricing](https://apis.io/plans/lancedb/lancedb-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Lancedb Rate Limits](https://apis.io/rate-limits/lancedb/lancedb-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Lancedb Finops](https://apis.io/finops/lancedb/lancedb-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://lancedb.com/)
- [Documentation](https://docs.lancedb.com/)
- [Blog](https://lancedb.com/blog)

## API Evangelist rating

**Kin Score 41.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 50.7 |
| Contract governance | 27.3 |
| Operational transparency | 26.3 |
| Developer ergonomics | 40.5 |
| Access clarity | 15.8 |

**Agent readiness 24.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 29.1** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/lancedb/](https://apis.io/providers/lancedb/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for LanceDB: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/lancedb/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
