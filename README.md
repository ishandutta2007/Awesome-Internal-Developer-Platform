# Awesome Internal Developer Platform (IDP) Tools & Ecosystem

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
![Internal Developer Platform](https://img.shields.io/badge/Category-Internal%20Developer%20Platform-blue)
![Platform Engineering](https://img.shields.io/badge/Focus-Platform%20Engineering-green)
![Last Updated](https://img.shields.io/badge/Updated-September%202026-brightgreen)

> A curated list of top **Internal Developer Platform (IDP)** tools, **Developer Portals**, **Service Catalogs**, **Self-Service Infrastructure Orchestrators**, and **Platform Engineering frameworks**.

Internal Developer Platforms (IDPs) enable platform engineering teams to deliver standardized golden paths, automated infrastructure self-service, and centralized service ownership. By reducing cognitive load and eliminating "yak shaving," IDPs accelerate software delivery while maintaining security, compliance, and operational guardrails.

---

## Table of Contents
- [Market Overview & Industry Dynamics](#market-overview--industry-dynamics)
- [SaaS & Hosted IDP Platforms](#saas--hosted-idp-platforms)
- [Open-Source IDP Projects & Frameworks](#open-source-idp-projects--frameworks)
- [IDP Architecture & Component Mapping](#idp-architecture--component-mapping)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

---

## Market Overview & Industry Dynamics

The global **Internal Developer Platform (IDP) & Platform Engineering Market** is estimated at **$6.2 Billion in 2026** and is projected to reach **$18.5 Billion by 2032** (CAGR ~20.1%).

### Market Structure & Concentration Analysis
- **Fragmentation Level**: **Moderately Fragmented** with rapid consolidation around foundational standards.
- **Market Dynamics**: The market is divided between **Developer Portals & Service Catalogs** (dominated by open-source Backstage and SaaS leaders like Harness & Port), **Platform Orchestrators** (Humanitec, Kratix, Crossplane), and **GitOps / Continuous Delivery** engines (Argo CD, Flux).
- **Winner-Take-All Potential**: Low. Due to diverse cloud infrastructure requirements and heterogeneous enterprise stacks, no single vendor captures the entire workflow. Instead, modular platform engineering stacks combining open-source standards (CNCF) with specialized SaaS layers are winning.

---

## SaaS & Hosted IDP Platforms

The table below lists leading commercial SaaS and hosted Internal Developer Platforms, sorted by company valuation/funding in descending order.

| Platform | Description & Key Features | Starting Tier Price | Free Tier / Trial Limits | Company Size (Valuation / Funding) |
| :--- | :--- | :--- | :--- | :--- |
| **[Harness IDP](https://harness.io/products/internal-developer-portal)** | Enterprise-grade developer portal built on Backstage, tightly integrated with Harness CI/CD pipelines, service catalogs, and software templates. | $10 / developer / month | Free Tier up to 5 developers & 100 service catalog entities | **$5.5 Billion Valuation** ($600M+ Raised) |
| **[Port](https://www.getport.io/)** | Visual no-code developer portal for software catalogs, self-service developer actions, scorecards, and automated SDLC workflows. | $78 / user / month (Pro) | Free Forever Plan up to 10,000 entities and 5 blueprints | **$800 Million Valuation** ($158M Total Raised) |
| **[Cortex](https://www.cortex.io/)** | Service catalog with powerful scorecard engine (CQL), production readiness tracking, and engineering intelligence dashboards (DORA metrics). | $65 / user / month | 14-day Free Trial with unlimited entities and full CQL access | **~$500M+ Valuation Est.** ($112M Total Raised) |
| **[Roadie](https://roadie.io/)** | Fully managed, SaaS-hosted Spotify Backstage platform with pre-configured plugins, automated upgrades, and zero-maintenance operations. | $30 / active developer / month | 14-day Free Trial with full plugin suite & managed Backstage instance | **~$200M Valuation Est.** ($62M Total Raised) |
| **[Akuity](https://akuity.io/)** | Enterprise managed Argo CD platform for GitOps application delivery with centralized RBAC, multi-cluster control, and audit logging. | $39 / cluster / month | 30-day Free Trial for up to 3 Kubernetes clusters | **~$100M Valuation Est.** ($20M Series A) |
| **[OpsLevel](https://www.opslevel.com/)** | Service catalog and maturity tracking platform featuring auto-discovery, gold/silver/bronze rubrics, and automated developer campaigns. | $39 / user / month | 14-day Free Trial with unlimited repository and infrastructure discovery | **~$90M Valuation Est.** ($22.2M Total Raised) |
| **[Northflank](https://northflank.com/)** | Developer platform for deploying microservices, jobs, and managed databases with cloud self-service and preview environments. | $12 / user / month | Developer Sandbox Free Tier (1 microservice, 1 DB, shared CPU/RAM) | **~$80M Valuation Est.** ($30.8M Total Raised) |
| **[Rafay Platform](https://rafay.co/)** | Kubernetes Operations Platform (KOP) providing multi-cluster lifecycle management, GitOps, environment templates, and policy guardrails. | $75 / cluster / month | 30-day Free Trial for up to 5 Kubernetes clusters | **~$75M Valuation Est.** ($37M Total Raised) |
| **[Humanitec](https://humanitec.com/)** | Platform Orchestrator that dynamically generates environment config and provisions infrastructure using the open-source Score specification. | $2,199 / month (Teams tier, up to 5 users) | 14-day Free Trial & instant 10-minute Interactive Sandbox | **~$60M Valuation Est.** ($15M+ Raised, ~$5.2M ARR) |
| **[Qovery](https://www.qovery.com/)** | On-demand cloud environment platform on top of Kubernetes providing developer self-service, preview environments, and deployment guardrails. | $49 / user / month | Free Tier for non-profits/open-source & 14-day Free Trial | **~$40M Valuation Est.** ($11M Series A) |
| **[Mia-Platform](https://mia-platform.eu/)** | End-to-end platform orchestrator and developer portal for building, running, and managing microservices and cloud-native applications. | €500 / month (Developer plan) | 30-day Free Community Trial with access to Console & Marketplace | **~$35M Valuation Est.** (Bootstrapped/Funded) |
| **[Massdriver](https://www.massdriver.cloud/)** | Cloud diagramming and self-service platform engineering tool enabling infrastructure provisioning with automated policy guardrails. | $70 / user / month | Free Trial up to 5 cloud deployments & 14 days full access | **~$20M Valuation Est.** ($3.2M Seed Raised) |
| **[KrakenD Enterprise](https://www.krakend.io/)** | Ultra-high performance API Gateway and platform API aggregation layer designed for IDP microservice endpoints. | $990 / month / cluster | Free Open-Source Community Edition (Unlimited nodes & requests) | **Acquired** (by Shop Circle) |

---

## Open-Source IDP Projects & Frameworks

Below is a curated list of top open-source repositories powering Internal Developer Platforms, sorted by GitHub Star Count in descending order.

| Project Name | Star Count | Category / Focus | Description | License |
| :--- | :--- | :--- | :--- | :--- |
| **[Backstage](https://backstage.io/)** | [![Backstage Stars](https://img.shields.io/github/stars/backstage/backstage?style=social&color=white)](https://github.com/backstage/backstage/stargazers) | Developer Portal & Catalog | CNCF Incubating developer portal framework created by Spotify. Features Software Catalog, Scaffolder, TechDocs, and 200+ plugins. | Apache 2.0 |
| **[Infisical](https://infisical.com/)** | [![Infisical Stars](https://img.shields.io/github/stars/Infisical/infisical?style=social&color=white)](https://github.com/Infisical/infisical/stargazers) | Platform Secrets Security | Open-source developer secret management platform for syncing environment variables, secrets, and identity security across infrastructure. | MIT / AGPL |
| **[Argo CD](https://argoproj.github.io/cd/)** | [![Argo CD Stars](https://img.shields.io/github/stars/argoproj/argo-cd?style=social&color=white)](https://github.com/argoproj/argo-cd/stargazers) | GitOps Continuous Delivery | CNCF Graduated declarative GitOps CD tool for Kubernetes, managing application deployments as the core delivery engine in IDPs. | Apache 2.0 |
| **[Dagger](https://dagger.io/)** | [![Dagger Stars](https://img.shields.io/github/stars/dagger/dagger?style=social&color=white)](https://github.com/dagger/dagger/stargazers) | Programmable CI/CD Engine | Programmable CI/CD engine that runs pipelines in containers, making delivery workflows portable across local machines and CI providers. | Apache 2.0 |
| **[Crossplane](https://www.crossplane.io/)** | [![Crossplane Stars](https://img.shields.io/github/stars/crossplane/crossplane?style=social&color=white)](https://github.com/crossplane/crossplane/stargazers) | Infrastructure Control Plane | CNCF Graduated Kubernetes control plane framework allowing platform teams to build custom infrastructure APIs and CRDs for developers. | Apache 2.0 |
| **[Kyverno](https://kyverno.io/)** | [![Kyverno Stars](https://img.shields.io/github/stars/kyverno/kyverno?style=social&color=white)](https://github.com/kyverno/kyverno/stargazers) | Kubernetes Policy Engine | CNCF Graduated Kubernetes-native policy management engine for validating, mutating, and generating cloud-native configurations and guardrails. | Apache 2.0 |
| **[Score](https://score.dev/)** | [![Score Stars](https://img.shields.io/github/stars/score-spec/spec?style=social&color=white)](https://github.com/score-spec/spec/stargazers) | Workload Specification | CNCF Sandbox developer-centric, environment-agnostic workload specification file (`score.yaml`) for declaring containerized app dependencies. | Apache 2.0 |
| **[KubeVela](https://kubevela.io/)** | [![KubeVela Stars](https://img.shields.io/github/stars/kubevela/kubevela?style=social&color=white)](https://github.com/kubevela/kubevela/stargazers) | Application Delivery Platform | CNCF Incubating modern application delivery and management platform based on Open Application Model (OAM) abstractions. | Apache 2.0 |
| **[OpenTelemetry Collector](https://opentelemetry.io/)** | [![OpenTelemetry Stars](https://img.shields.io/github/stars/open-telemetry/opentelemetry-collector?style=social&color=white)](https://github.com/open-telemetry/opentelemetry-collector/stargazers) | Observability Pipeline | CNCF Graduated vendor-agnostic proxy that receives, processes, and exports telemetry data (metrics, logs, traces) for IDP service intelligence. | Apache 2.0 |
| **[Devtron](https://devtron.ai/)** | [![Devtron Stars](https://img.shields.io/github/stars/devtron-labs/devtron?style=social&color=white)](https://github.com/devtron-labs/devtron/stargazers) | K8s Application Management | Complete open-source App Management Platform for Kubernetes combining CI, CD, GitOps, Security, and Observability in a unified UI. | Apache 2.0 |
| **[Apache DevLake](https://devlake.apache.org/)** | [![DevLake Stars](https://img.shields.io/github/stars/apache/devlake?style=social&color=white)](https://github.com/apache/devlake/stargazers) | Engineering Management / DORA | Apache Top-Level open-source dev lake for analyzing engineering data, tracking DORA metrics, and measuring platform engineering adoption. | Apache 2.0 |
| **[Radius](https://radapp.io/)** | [![Radius Stars](https://img.shields.io/github/stars/radius-project/radius?style=social&color=white)](https://github.com/radius-project/radius/stargazers) | Cloud-Native App Platform | Open-source application platform designed for multi-cloud app graphs, infrastructure recipes (Bicep/Terraform), and decoupled deployment specs. | Apache 2.0 |
| **[OpenChoreo](https://openchoreo.dev/)** | [![OpenChoreo Stars](https://img.shields.io/github/stars/openchoreo/openchoreo?style=social&color=white)](https://github.com/openchoreo/openchoreo/stargazers) | CNCF Developer Platform | CNCF Sandbox project providing an open-source, multi-plane Kubernetes developer platform with experience, control, and observability layers. | Apache 2.0 |
| **[Kratix](https://kratix.io/)** | [![Kratix Stars](https://img.shields.io/github/stars/syntasso/kratix?style=social&color=white)](https://github.com/syntasso/kratix/stargazers) | Platform-as-a-Product Engine | Open-source framework that extends Kubernetes to build composable platform capabilities ("Promises") for enterprise multi-cluster environments. | Apache 2.0 |

---

## IDP Architecture & Component Mapping

Building an enterprise-grade Internal Developer Platform usually requires layering specialized tools across 5 architectural planes:

```
+-------------------------------------------------------------------+
|                     1. Portal / Experience Plane                 |
|  Backstage | Port | Harness IDP | OpsLevel | Cortex | Roadie       |
+-------------------------------------------------------------------+
                                  |
+-------------------------------------------------------------------+
|                   2. Orchestration & Control Plane                |
|  Humanitec | Kratix | Crossplane | Radius | Mia-Platform          |
+-------------------------------------------------------------------+
                                  |
+-------------------------------------------------------------------+
|                    3. Delivery & Pipeline Plane                   |
|  Argo CD | Dagger | Qovery | Devtron | Northflank | Akuity        |
+-------------------------------------------------------------------+
                                  |
+-------------------------------------------------------------------+
|               4. Security, Policy & Guardrails Plane              |
|  Infisical | Kyverno | OPA Gatekeeper | Score Workload Spec       |
+-------------------------------------------------------------------+
                                  |
+-------------------------------------------------------------------+
|                   5. Observability & Data Plane                   |
|  OpenTelemetry | Apache DevLake | Grafana LGTM Stack             |
+-------------------------------------------------------------------+
```

---

## How to Contribute

Contributions are welcome and greatly appreciated! To contribute to this list:

1. **Fork** this repository.
2. Add your tool/project entry in the appropriate table following the established alphabetical or metric sorting guidelines.
3. Ensure all links point to authoritative landing pages or official repositories.
4. Submit a **Pull Request** with a brief summary of the added technology.

---

## Disclaimer

This repository is a community-maintained curated resource intended for educational and research purposes. Product pricing, funding data, and feature capabilities reflect estimates and public disclosures as of late 2026. This list does not constitute financial advice or formal software endorsement.
