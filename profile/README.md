<div align="center">
  <img src="./plasmatic_logo.png" alt="Plasmatic" width="144" height="144">

  <h1>Plasmatic</h1>

  <p><strong>Builders of <a href="https://github.com/GoPlasmatic/Orion">Orion</a>, the governed services platform for teams building software with AI.</strong></p>

  <p><a href="https://goplasmatic.io">Website</a> · <a href="https://docs.goplasmatic.io">Documentation</a> · <a href="https://docs.goplasmatic.io/getting-started/install.html">Install Orion</a> · <a href="https://goplasmatic.io/contact">Get in touch</a></p>
</div>

---

AI can write business logic in minutes. Getting that logic safely into production still means rebuilding and reviewing the same foundations: routing, security, validation, resilience, observability, deployment controls, and rollback.

We build **Orion** to make that foundation the runtime's job.

Describe a service as lightweight JSON—written by an engineer or an AI assistant—and Orion turns it into a live, governed REST or Kafka service. Your team owns the logic; Orion consistently carries the production architecture around it.

## What you can build with Orion

- **Microservice APIs** that answer requests in-process
- **Decision APIs** for pricing, eligibility, classification, and routing
- **Kafka event pipelines** with retries, deduplication, and dead-letter handling
- **Webhook and data ingestion** across HTTP, databases, Elasticsearch, and object storage
- **Tools for AI agents**, with the same controls as every other service

## Governance built into the runtime

Every change follows a controlled lifecycle: **draft → dry-run → explicit activation**, with percentage rollout and one-call rollback. Definitions are immutable once active, changes are auditable, and previous versions remain reversible without rebuilding or restarting an application server.

Orion also provides the operational capabilities teams otherwise recreate for every service:

- Authentication, payload validation, rate limiting, and backpressure
- Timeouts, safe retries, circuit breakers, caching, and connection pooling
- Structured logs, Prometheus metrics, distributed tracing, and execution traces
- Zero-downtime hot reload, percentage rollouts, and one-call rollback
- SQLite for a single node; PostgreSQL or MySQL and Redis for clustered deployments
- A single Rust binary, Docker images, Kubernetes support, an admin API, CLI, and browser console

Orion is designed for request-shaped and per-record work measured in milliseconds. For durable, long-running orchestration, API-edge concerns, or stateful stream processing, it works alongside the specialist tools built for those jobs. [See where Orion fits](https://docs.goplasmatic.io/comparison.html).

## Start locally

```bash
docker run --name orion-quickstart -d -p 8080:8080 \
  ghcr.io/goplasmatic/orion:latest

curl --retry 10 --retry-delay 1 --retry-connrefused \
  http://localhost:8080/healthz
```

Then follow the [first live API quickstart](https://docs.goplasmatic.io/getting-started/quickstart.html), explore the [example packages](https://docs.goplasmatic.io/getting-started/examples.html), or learn [how Orion works](https://docs.goplasmatic.io/concepts/how-orion-works.html).

## Open-source projects

| Project | What it does |
|---|---|
| [Orion](https://github.com/GoPlasmatic/Orion) | The Apache-2.0 governed services runtime, server, CLI, deployment assets, and examples |
| [Orion UI](https://github.com/GoPlasmatic/Orion-ui) | Browser console for building, testing, deploying, and operating Orion services |
| [dataflow-rs](https://github.com/GoPlasmatic/dataflow-rs) | Embeddable Rust dataflow engine that powers Orion workflows |
| [datalogic-rs](https://github.com/GoPlasmatic/datalogic-rs) | Declarative logic engine used to evaluate conditions and expressions |

Orion is open source under the [Apache License 2.0](https://github.com/GoPlasmatic/Orion/blob/main/LICENSE). We develop it in the open and offer delivery, support, and enterprise engagement—not a separate open-core edition or a licence to the runtime.

## Join the project

- Ask questions and share ideas in [Discussions](https://github.com/GoPlasmatic/Orion/discussions)
- Report bugs through [Issues](https://github.com/GoPlasmatic/Orion/issues)
- Read the [contribution guide](https://github.com/GoPlasmatic/Orion/blob/main/CONTRIBUTING.md)
- Using Orion? Add your project to [ADOPTERS.md](https://github.com/GoPlasmatic/Orion/blob/main/ADOPTERS.md)

<div align="center">
  <strong>Build at AI speed. Keep production under control.</strong>
</div>
