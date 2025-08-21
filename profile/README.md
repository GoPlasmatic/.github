<div align="center">
  <img src="./plasmatic_logo.png" alt="Plasmatic logo" width="160" height="160">
</div>

# Plasmatic

Plasmatic builds open-source payment infrastructure focused on high-performance, low-latency payment processing. We create auditable, production-ready engines and tooling so teams can operate reliable, auditable payment systems without vendor lock-in.

## Reframe

Reframe is Plasmatic's enterprise-grade, open-source transformation engine that currently supports SWIFT CBPR+ ↔ ISO 20022 transformations and the SR2025 specification. Implemented in Rust for speed and reliability, Reframe is designed for container-native deployment and high-throughput production workloads. It uses a declarative mapping syntax, making it straightforward to implement additional transformation profiles quickly and in an auditable manner.

Repository: https://github.com/GoPlasmatic/Reframe

## Other important libraries

Plasmatic maintains several focused libraries that power Reframe and related tooling:

- [datalogic-rs](https://github.com/GoPlasmatic/datalogic-rs) — Declarative logic engine for auditable field mappings and business rules.
- [dataflow-rs](https://github.com/GoPlasmatic/dataflow-rs) — High-performance dataflow/workflow engine.
- [SwiftMTMessage](https://github.com/GoPlasmatic/SwiftMTMessage) — SWIFT MT models and parsing utilities.
- [MXMessage](https://github.com/GoPlasmatic/MXMessage) — ISO 20022 (MX) models and helpers.
- [datafake-rs](https://github.com/GoPlasmatic/datafake-rs) — Test data tooling for realistic message samples and load testing.

