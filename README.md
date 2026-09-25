# Kubernetes Production Best Practices

A practical collection of patterns and checklists for running **secure, scalable and resilient workloads on Kubernetes**.

This repository is organized around three concerns that repeatedly appear in production environments: how applications are built for Kubernetes, how clusters are governed, and how the platform itself is configured.

![Kubernetes production best practices](preview.gif)

## Scope

The material covers production-oriented topics such as:

- workload design and application lifecycle
- health checks and graceful termination
- resource requests, limits and capacity
- availability and disruption handling
- configuration and secrets
- security and governance
- cluster-level operational practices
- observability and troubleshooting considerations

## Guide

| Area | Document | Focus |
|---|---|---|
| Application | [Application development](application-development.md) | Workload and application design |
| Governance | [Governance](governance.md) | Security, policy and operational controls |
| Cluster | [Cluster configuration](configuration.md) | Production cluster configuration |

## How to use this repository

Treat this repository as an **engineering checklist and discussion framework**, not as a universal set of defaults.

Production decisions should take into account:

- workload characteristics
- failure domains
- latency and availability requirements
- traffic patterns
- security constraints
- cost and capacity
- recovery objectives
- operational maturity

The goal is to make reliability decisions explicit and reviewable.

## Production-readiness mindset

A Kubernetes workload should not be considered production-ready simply because it can be deployed.

A mature review should also ask:

- What happens when a dependency is unavailable?
- How does the workload behave during overload?
- Can it terminate gracefully?
- Are resource requirements measurable?
- Are alerts tied to user-impacting symptoms?
- Is the service observable during partial failure?
- Are rollback and recovery procedures tested?
- Is scaling behavior understood before an incident?

## Related areas

This repository complements work in:

- Site Reliability Engineering
- Platform Engineering
- Production Readiness
- Observability
- Capacity Planning
- Incident Response
- Kubernetes troubleshooting

---

Maintained by [Marco Cristofolini](https://github.com/marcocristofolini).
