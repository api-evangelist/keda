# KEDA

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

KEDA (Kubernetes Event Driven Autoscaling) is a CNCF graduated application autoscaler that drives scaling of any container in Kubernetes based on the number of events needing to be processed. It extends Kubernetes with custom resources for defining scaling behavior and supports over 50 built-in scalers for event sources including Kafka, RabbitMQ, AWS SQS, Azure Service Bus, and Prometheus.

**Areas:** Auto-Scaling · CNCF · Event-Driven · Graduated · Kubernetes · Cloud-Native

## KEDA on APIs.io

Everything profiled for KEDA is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/keda/](https://apis.io/providers/keda/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [KEDA Metrics API](https://apis.io/apis/keda/keda-metrics-api/) — External metrics API server that exposes event-driven metrics from configured scalers to the Kubernetes Horizontal Pod Autoscaler. It implements the…
- [KEDA ScaledObject API](https://apis.io/apis/keda/keda-scaled-object-api/) — The ScaledObject custom resource defines the mapping between an event source and a Kubernetes Deployment, StatefulSet, or custom resource that should be…
- [KEDA ScaledJob API](https://apis.io/apis/keda/keda-scaled-job-api/) — The ScaledJob custom resource defines the mapping between an event source and Kubernetes Jobs that should be created in response to events. Unlike…
- [KEDA TriggerAuthentication API](https://apis.io/apis/keda/keda-trigger-authentication-api/) — The TriggerAuthentication and ClusterTriggerAuthentication custom resources define authentication parameters for KEDA trigger scalers, allowing credentials…
- [KEDA CloudEventSource API](https://apis.io/apis/keda/keda-cloud-event-source-api/) — The CloudEventSource and ClusterCloudEventSource custom resources define HTTP or Azure Event Grid destinations where KEDA delivers CloudEvents when scaling…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [KEDA CloudEvent Source](https://apis.io/asyncapis/keda/keda-cloud-events-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [/events](https://apis.io/channels/keda/events/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Keda Agentic Access](https://apis.io/agentic-access/keda/keda-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [KEDA CloudEvent](https://apis.io/schemas/keda/keda-cloud-event/)
- [KEDA ScaledObject](https://apis.io/schemas/keda/keda-scaled-object/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Keda Context](https://apis.io/jsonld/keda/keda-context/)

#### Collections (1)

Postman and Open Collection request collections.

- [KEDA Metrics API](https://apis.io/collections/keda/open-keda-metrics-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [KEDA — asyncapi rules](https://apis.io/rules/keda/keda-asyncapi-spectral-rules/)
- [KEDA — jsonschema rules](https://apis.io/rules/keda/keda-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Keda Authentication](https://apis.io/security/keda/keda-authentication/)
- [Keda Domain Security](https://apis.io/security/keda/keda-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Keda Plans Pricing](https://apis.io/plans/keda/keda-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Keda Rate Limits](https://apis.io/rate-limits/keda/keda-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Keda Finops](https://apis.io/finops/keda/keda-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://keda.sh/)
- [Documentation](https://keda.sh/docs/latest/)
- [Getting started](https://keda.sh/docs/latest/deploy/)
- [Changelog](https://github.com/kedacore/keda/blob/main/CHANGELOG.md)
- [Blog](https://keda.sh/blog/)
- [Security](https://github.com/kedacore/keda/blob/main/SECURITY.md)
- [GitHub](https://github.com/kedacore)

## API Evangelist rating

**Kin Score 45.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 67.3 |
| Contract governance | 13.6 |
| Operational transparency | 34.2 |
| Developer ergonomics | 45.2 |
| Access clarity | 5.3 |

**Agent readiness 27.8** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/keda/](https://apis.io/providers/keda/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for KEDA: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/keda/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
