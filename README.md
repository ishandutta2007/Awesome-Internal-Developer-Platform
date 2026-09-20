# Awesome-Internal-Developer-Platform

Top Internal Developer Platform (IDP) Tools Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Developer Portals, Service Catalogs, Self-Service Infrastructure & Platform Orchestration
Last updated: September 2026

This repository tracks notable SaaS platforms and open-source projects for Internal Developer Platforms (IDPs). These tools help platform engineering teams provide self-service infrastructure, standardized golden paths, service catalogs, and developer portals that reduce cognitive load and accelerate software delivery.

Examples include Humanitec, Port, OpsLevel, Cortex, Backstage, Roadie, Qovery, Northflank, Dagger, Kratix, Harness IDP, Mia-Platform, Akuity, Massdriver, Rafay Platform, Score.dev, Krateo, Appvia, and KrakenD (the category leaders).

Open-source emphasis: This section is heavily expanded with every major active project for self-hosting, custom platform APIs, and transparent developer experiences — ideal for platform teams that need full control over their IDP without vendor lock-in or per-developer SaaS fees.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

How to Contribute

Disclaimer

SaaS/Hosted Platforms

Humanitec
Platform Orchestrator that dynamically generates environment-specific configuration and provisions real infrastructure. Uses the open-source Score workload specification (CNCF Sandbox) so developers declare what an app needs without writing environment-specific config. Kubernetes-centric and architecturally opinionated -
9
-
18
.

Port
Commercial no-code IDP with visual builder for software catalog, self-service actions, and scorecards. Deploys in days rather than months, with built-in integrations for GitHub, GitLab, PagerDuty, Datadog, and ArgoCD. Pricing around $78/user/month -
1
-
8
.

OpsLevel
Service catalog and maturity tracking platform with auto-discovery from repos and infrastructure. Bronze/silver/gold maturity rubrics and "campaigns" for org-wide improvements. Pricing around $39/user/month, known for fast time-to-value -
1
-
3
.

Cortex
Service catalog with deep scorecard engine (CQL - Cortex Query Language) for production readiness, security posture, and migration tracking. Engineering intelligence dashboards with DORA metrics. Pricing $65-69/user/month -
1
-
3
.

Roadie
Managed Backstage offering — open-source portal delivered as SaaS with plugin curation, upgrades, and scaling handled. The pragmatic middle path for teams that want Backstage's ecosystem without operating it -
3
-
6
.

Qovery
Internal platform and application deployment layer (often Kubernetes-based) providing self-service environments, deployment workflows, and platform abstractions. Reduces "yak shaving" for application teams -
6
.

Northflank
Developer platform for deploying and managing applications with self-service environments, CI/CD, and infrastructure abstraction.

Harness IDP
Internal Developer Portal built on Backstage, integrated into the Harness platform. Provides service catalog, software templates, and self-service workflows with Harness pipeline integration.

Mia-Platform
Platform orchestrator and IDP for building and managing cloud-native applications with self-service capabilities and developer experience focus -
18
.

Akuity
Managed Argo CD platform for GitOps-driven application delivery. Provides enterprise-grade Argo CD with SSO, RBAC, and multi-cluster management.

Massdriver
Platform engineering solution for self-service cloud infrastructure with pre-built components and guardrails.

Rafay Platform
Kubernetes Operations Platform (KOP) for cluster lifecycle management, GitOps, and policy governance across multi-cloud and edge.

Appvia
Platform engineering consultancy with Wayfinder, a Kubernetes developer platform for self-service application delivery.

KrakenD
Ultra-high performance API gateway for building platform APIs. Can serve as the API layer in an IDP architecture.

Open-Source GitHub Projects

Backstage
The CNCF Incubating open-source developer portal framework created by Spotify. Provides software catalog, Scaffolder for golden path templates, TechDocs for docs-as-code, and 200+ community plugins. The de facto standard for building IDPs. Requires 2-5 FTE for maintenance and 6-12 months to implement meaningfully. Apache 2.0 -
1
-
5
-
17
.

Kratix
Kubernetes-native platform-as-a-product framework. Extends the Kubernetes API with "Promises" — platform APIs that developers interact with using kubectl or GitOps. Multi-cluster by design with clean separation between platform team and developer concerns. Pairs with Backstage or Port for the UI layer -
8
-
12
.

Horizon
Go-based framework for building internal developer platforms with a Kubernetes-like API on top of NATS. Designed to decouple end users from underlying platform technologies (Kubernetes, AWS, GCP, Azure). Thin wrapper with minimal dependencies — only NATS required. Proof of concept but promising architecture for platform teams who want to build and own their API layer -
2
.

OpenChoreo
CNCF Sandbox project providing a complete, open-source developer platform for Kubernetes. Multi-plane architecture (Experience, Control, Data, Observability, CI) with Backstage-powered portal. Opinionated abstractions for components, endpoints, and connections. Originally developed by WSO2 based on their Choreo SaaS experience -
10
-
13
.

Radius
Open-source application platform for cloud-native apps. Application graph for understanding dependencies, Recipes for infrastructure provisioning (Terraform, Bicep), and separation of app definition from infrastructure details. Strong Azure integration, growing multi-cloud support. Apache 2.0 -
7
.

Crossplane
CNCF graduated Kubernetes-native control plane framework. Lets platform teams expose higher-level APIs for infrastructure and services so developers can self-serve without becoming infrastructure experts. v2.x removed claims in favor of namespaced XRs and composition functions -
6
-
9
.

Argo CD
CNCF graduated GitOps continuous delivery controller for Kubernetes. Continuously reconciles desired state in Git with running clusters. The standard for GitOps-driven application delivery in IDPs -
6
.

Dagger
Programmable CI/CD engine that runs pipeline steps in containers. Makes pipelines portable across laptops and CI environments, easier to standardize across many services -
6
.

Score
CNCF Sandbox workload specification (Apache 2.0). Developer-owned, environment-agnostic specification for defining what an application needs (database, cache, memory). The foundation for Humanitec's Platform Orchestrator and portable across implementations -
9
.

Additional Strong Open-Source Options

Platform Orchestrators: Kratix (Kubernetes-native Promises), Crossplane (CNCF graduated control plane), Humanitec (Score-based, commercial).

GitOps & CI/CD: Argo CD (CNCF graduated), Flux (CNCF graduated), Dagger (portable pipelines).

Policy & Guardrails: OPA Gatekeeper (admission control), Kyverno (Kubernetes-native policy), Score (workload specification).

Observability: OpenTelemetry (CNCF standard), Grafana LGTM stack (Loki, Grafana, Tempo, Mimir) -
6
.

Secrets Management: Infisical (secrets + identity security), External Secrets Operator (sync external secrets to Kubernetes) -
6
.

Frameworks for building custom systems: Combine Backstage for the portal layer, Kratix or Crossplane for platform orchestration, Argo CD for GitOps delivery, Dagger for CI/CD pipelines, and Score for workload specifications. Add OpenTelemetry + Grafana for observability and OPA Gatekeeper or Kyverno for guardrails.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

IDPs require significant investment in platform engineering headcount; Backstage's "free" license masks $150K+ per 20 developers in engineering time -
1
.

The real decision is not "which portal" but whether your team has outgrown wikis and Slack threads as the system of record for service ownership -
16
.

Made for platform engineers, DevOps leads, SREs, and engineering leaders.
Let's make internal developer platforms more open, self-service, and developer-friendly.
