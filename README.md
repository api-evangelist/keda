# KEDA (keda)

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

KEDA (Kubernetes Event Driven Autoscaling) is a CNCF graduated application autoscaler that drives scaling of any container in Kubernetes based on the number of events needing to be processed. It extends Kubernetes with custom resources for defining scaling behavior and supports over 50 built-in scalers for event sources including Kafka, RabbitMQ, AWS SQS, Azure Service Bus, and Prometheus.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Autoscaling
- CNCF
- Event-Driven
- Graduated
- Kubernetes

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-19

## APIs

### KEDA Metrics API

External metrics API server that exposes event-driven metrics from configured scalers to the Kubernetes Horizontal Pod Autoscaler. It implements the Kubernetes external metrics API interface, allowing the HPA controller to query scaler-derived metrics when making scaling decisions.

- **Human URL:** [https://keda.sh/docs/latest/operate/metrics-server/](https://keda.sh/docs/latest/operate/metrics-server/)

#### Tags

- External Metrics
- HPA
- Kubernetes
- Metrics

#### Properties

- [Documentation](https://keda.sh/docs/latest/operate/metrics-server/)
- [Getting Started](https://keda.sh/docs/latest/deploy/)
- [Reference](https://keda.sh/docs/latest/concepts/)
- [OpenAPI](openapi/keda-metrics-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/keda-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keda-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### KEDA ScaledObject API

The ScaledObject custom resource defines the mapping between an event source and a Kubernetes Deployment, StatefulSet, or custom resource that should be scaled based on event metrics. It specifies trigger scalers, scaling thresholds, min/max replica counts, and cooldown periods for workload-based autoscaling.

- **Human URL:** [https://keda.sh/docs/latest/concepts/scaling-deployments/](https://keda.sh/docs/latest/concepts/scaling-deployments/)

#### Tags

- Autoscaling
- CRD
- Kubernetes
- ScaledObject

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/scaling-deployments/)
- [JSON Schema](scaled-object.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/keda-scaled-object-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](keda-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Reference](https://keda.sh/docs/latest/reference/scaledobject-spec/)
- [Postman Collection](collections/keda-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keda-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### KEDA ScaledJob API

The ScaledJob custom resource defines the mapping between an event source and Kubernetes Jobs that should be created in response to events. Unlike ScaledObject, ScaledJob creates new Job instances to process each unit of work rather than scaling existing long-running deployments, making it suited for batch workloads.

- **Human URL:** [https://keda.sh/docs/latest/concepts/scaling-jobs/](https://keda.sh/docs/latest/concepts/scaling-jobs/)

#### Tags

- Autoscaling
- CRD
- Jobs
- Kubernetes

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/scaling-jobs/)
- [JSON Schema](scaled-job.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](keda-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Reference](https://keda.sh/docs/latest/reference/scaledjob-spec/)
- [Postman Collection](collections/keda-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keda-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### KEDA TriggerAuthentication API

The TriggerAuthentication and ClusterTriggerAuthentication custom resources define authentication parameters for KEDA trigger scalers, allowing credentials to be sourced from Kubernetes Secrets, environment variables, pod identity providers such as AWS IRSA or Azure Workload Identity, or HashiCorp Vault without embedding them in the ScaledObject.

- **Human URL:** [https://keda.sh/docs/latest/concepts/authentication/](https://keda.sh/docs/latest/concepts/authentication/)

#### Tags

- Authentication
- CRD
- Kubernetes
- Security

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/authentication/)
- [JSON Schema](trigger-authentication.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](keda-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Reference](https://keda.sh/docs/latest/reference/triggerauthentication-spec/)
- [Postman Collection](collections/keda-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keda-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### KEDA CloudEventSource API

The CloudEventSource and ClusterCloudEventSource custom resources define HTTP or Azure Event Grid destinations where KEDA delivers CloudEvents when scaling events occur. Events follow the CloudEvents specification v1.0 and carry reason codes and messages for events such as ScalerError, ScaledObjectReady, ScaledObjectDeleted, and AuthenticationFailed. Optional event type filters allow consumers to subscribe to only the events they care about.

- **Human URL:** [https://keda.sh/docs/latest/operate/cloud-events/](https://keda.sh/docs/latest/operate/cloud-events/)

#### Tags

- CloudEvents
- CRD
- Events
- Kubernetes
- Webhooks

#### Properties

- [Documentation](https://keda.sh/docs/latest/operate/cloud-events/)
- [AsyncAPI](asyncapi/keda-cloud-events-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/keda-cloud-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/keda-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/keda-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://keda.sh/)
- [Documentation](https://keda.sh/docs/latest/)
- [Getting Started](https://keda.sh/docs/latest/deploy/)
- [GitHub Organization](https://github.com/kedacore)
- [GitHub Repository](https://github.com/kedacore/keda)
- [Blog](https://keda.sh/blog/)
- [Community](https://keda.sh/community/)
- [Slack](https://kubernetes.slack.com/archives/CKZJ36A5D)
- [Changelog](https://github.com/kedacore/keda/blob/main/CHANGELOG.md)
- [Security](https://github.com/kedacore/keda/blob/main/SECURITY.md)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/keda)
- [JSON-LD](keda-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/keda-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/keda-scaled-object-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/keda-cloud-event-schema.json) — [JSON Schema](https://json-schema.org/specification)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
