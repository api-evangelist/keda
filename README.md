# KEDA (keda)
KEDA (Kubernetes Event Driven Autoscaling) is a CNCF graduated application autoscaler that drives scaling of any container in Kubernetes based on the number of events needing to be processed. It extends Kubernetes with custom resources for defining scaling behavior and supports over 50 built-in scalers for event sources including Kafka, RabbitMQ, AWS SQS, Azure Service Bus, and Prometheus.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/apis.yml)

## Scope

- **Type:** Index 
- **Position:** Consuming 
- **Access:** 3rd-Party 

## Tags:

 - Kubernetes, Autoscaling, Event-Driven, CNCF, Graduated

## Timestamps

- **Created:** 2025-01-01 
- **Modified:** 2026-03-18 

## APIs

### KEDA Metrics API
External metrics API server that exposes event-driven metrics from configured scalers to the Kubernetes Horizontal Pod Autoscaler. It implements the Kubernetes external metrics API interface, allowing the HPA controller to query scaler-derived metrics when making scaling decisions.

**Human URL:** [https://keda.sh/docs/latest/operate/metrics-server/](https://keda.sh/docs/latest/operate/metrics-server/)


#### Tags:

 - Metrics, External Metrics, HPA, Kubernetes

#### Properties

- [Documentation](https://keda.sh/docs/latest/operate/metrics-server/)
- [Getting Started](https://keda.sh/docs/latest/deploy/)
- [Reference](https://keda.sh/docs/latest/concepts/)
- [OpenAPI](openapi/keda-metrics-api-openapi.yml)

### KEDA ScaledObject API
The ScaledObject custom resource defines the mapping between an event source and a Kubernetes Deployment, StatefulSet, or custom resource that should be scaled based on event metrics. It specifies trigger scalers, scaling thresholds, min/max replica counts, and cooldown periods for workload-based autoscaling.

**Human URL:** [https://keda.sh/docs/latest/concepts/scaling-deployments/](https://keda.sh/docs/latest/concepts/scaling-deployments/)


#### Tags:

 - Kubernetes, CRD, Autoscaling, ScaledObject

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/scaling-deployments/)
- [JSONSchema](scaled-object.json)
- [JSONSchema](json-schema/keda-scaled-object-schema.json)
- [JSON-LD](keda-context.jsonld)
- [Reference](https://keda.sh/docs/latest/reference/scaledobject-spec/)

### KEDA ScaledJob API
The ScaledJob custom resource defines the mapping between an event source and Kubernetes Jobs that should be created in response to events. Unlike ScaledObject, ScaledJob creates new Job instances to process each unit of work rather than scaling existing long-running deployments, making it suited for batch workloads.

**Human URL:** [https://keda.sh/docs/latest/concepts/scaling-jobs/](https://keda.sh/docs/latest/concepts/scaling-jobs/)


#### Tags:

 - Kubernetes, CRD, Autoscaling, Jobs

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/scaling-jobs/)
- [JSONSchema](scaled-job.json)
- [JSON-LD](keda-context.jsonld)
- [Reference](https://keda.sh/docs/latest/reference/scaledjob-spec/)

### KEDA TriggerAuthentication API
The TriggerAuthentication and ClusterTriggerAuthentication custom resources define authentication parameters for KEDA trigger scalers, allowing credentials to be sourced from Kubernetes Secrets, environment variables, pod identity providers such as AWS IRSA or Azure Workload Identity, or HashiCorp Vault without embedding them in the ScaledObject.

**Human URL:** [https://keda.sh/docs/latest/concepts/authentication/](https://keda.sh/docs/latest/concepts/authentication/)


#### Tags:

 - Kubernetes, CRD, Authentication, Security

#### Properties

- [Documentation](https://keda.sh/docs/latest/concepts/authentication/)
- [JSONSchema](trigger-authentication.json)
- [JSON-LD](keda-context.jsonld)
- [Reference](https://keda.sh/docs/latest/reference/triggerauthentication-spec/)

### KEDA CloudEventSource API
The CloudEventSource and ClusterCloudEventSource custom resources define HTTP or Azure Event Grid destinations where KEDA delivers CloudEvents when scaling events occur. Events follow the CloudEvents specification v1.0 and carry reason codes and messages for events such as ScalerError, ScaledObjectReady, ScaledObjectDeleted, and AuthenticationFailed. Optional event type filters allow consumers to subscribe to only the events they care about.

**Human URL:** [https://keda.sh/docs/latest/operate/cloud-events/](https://keda.sh/docs/latest/operate/cloud-events/)


#### Tags:

 - Kubernetes, CRD, CloudEvents, Events, Webhooks

#### Properties

- [Documentation](https://keda.sh/docs/latest/operate/cloud-events/)
- [AsyncAPI](asyncapi/keda-cloud-events-asyncapi.yml)
- [JSONSchema](json-schema/keda-cloud-event-schema.json)

## Common Properties

- [Website](https://keda.sh/)
- [Documentation](https://keda.sh/docs/latest/)
- [Getting Started](https://keda.sh/docs/latest/deploy/)
- [GitHub Organization](https://github.com/kedacore)
- [GitHubRepository](https://github.com/kedacore/keda)
- [Blog](https://keda.sh/blog/)
- [Community](https://keda.sh/community/)
- [Slack](https://kubernetes.slack.com/archives/CKZJ36A5D)
- [Change Log](https://github.com/kedacore/keda/blob/main/CHANGELOG.md)
- [Security](https://github.com/kedacore/keda/blob/main/SECURITY.md)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/keda)
- [JSON-LD](keda-context.jsonld)
- [JSON-LD](json-ld/keda-context.jsonld)
- [JSONSchema](json-schema/keda-scaled-object-schema.json)
- [JSONSchema](json-schema/keda-cloud-event-schema.json)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
