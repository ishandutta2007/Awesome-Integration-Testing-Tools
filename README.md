# Awesome-Integration-Testing-Tools

## Top Integration Testing Tools Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Containerized Test Dependencies, Realistic Integration Environments & Self-Hosted Test Infrastructure*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Integration Testing Tools**. These tools help developers validate that application components work correctly together—spinning up real databases, message brokers, and external services in isolated, reproducible environments rather than relying on mocks that drift from production behavior.



**Examples** include Testcontainers, Docker Desktop, Testsigma, BrowserStack, Sauce Labs, Postman, ReadyAPI, Katalon Studio, and Tricentis (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding per-minute cloud testing fees, and transparent test infrastructure—ideal for teams that want realistic dependencies without managing permanent test environments. The open-source landscape is anchored by **Testcontainers** (the disposable container library available across Java, .NET, Python, Go, Node.js, and Rust), with **Keploy** offering traffic-driven test generation and **dockerlet** providing a minimal Rust alternative for narrow use cases.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global software testing and quality engineering market is estimated at approximately **$50–$60 billion** (2025–2026), expanding at a CAGR of roughly 8–13%. The sector is **moderately fragmented**: while enterprise leaders (such as Tricentis, SmartBear, and BrowserStack) capture large commercial footprints, no single vendor commands a winner-take-all monopoly, leaving substantial market share distributed across open-source ecosystems, specialized cloud device clouds, and AI-driven testing startups.

## SaaS/Hosted Platforms

| Product | Company Size (Valuation / Revenue) | Pricing | Free Tier / Free Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Postman](https://www.postman.com/)** | $5.6B valuation (~$170M–$300M ARR) | Starts at $9/user/month (Solo, annual) or $19/user/month (Team, annual) | Free plan: 1 user, unlimited collection runs & mock servers, 1,000 API monitoring calls/month, 50 AI credits/month | API platform featuring collection-based automated testing, mock servers, and contract testing workflows. |
| **[Tricentis](https://www.tricentis.com/)** | $4.5B valuation (~$500M ARR) | Starts around $3,000/user/year (or core platform from €20,000/year) | 14-day free trial (full evaluation access to Tosca / qTest cloud features, no credit card required) | Enterprise-grade continuous testing and model-based test automation platform for complex integrated workflows. |
| **[BrowserStack](https://www.browserstack.com/)** | $4.0B valuation (~$225M ARR) | Starts at $29/user/month (Live Desktop, annual) or $99/parallel/month (Automate Desktop) | Free trial: 30 minutes Live testing (desktop/mobile, ~1 min/device limit), 60 minutes Automate, 100 screenshots; Percy visual tier free for 5,000 screenshots/month | Cloud device and browser testing cloud providing real device execution for web and mobile integration validation. |
| **[Docker Desktop](https://www.docker.com/products/docker-desktop/)** | $2.1B valuation (~$207M ARR) | Starts at $9/user/month (Pro, annual) or $15/user/month (Team, annual) | Free-forever Personal plan: Limited to personal use, education, and businesses with <250 employees AND <$10M revenue | Local container engine that developers and CI workflows use to run Testcontainers and containerized dependencies. |
| **[ReadyAPI (SmartBear)](https://smartbear.com/product/ready-api/)** | Private (~$500M ARR) | Starts at $1,000/license/year (individual module) or $4,700+/license/year (full bundle) | 14-day free trial (complete unrestricted access to all ReadyAPI functional, load, and virtualization modules) | API integration and testing suite providing service virtualization, security validation, and performance testing. |
| **[Sauce Labs](https://saucelabs.com/)** | Private (~$70M–$90M ARR) | Starts at $39/month (Live Testing, annual) or $149/month (Virtual Cloud, annual) | 28-day free trial: 60 automated/live testing minutes with 3 concurrent virtual machines | Enterprise cloud continuous testing platform offering real device grids, emulators, and virtual browser environments. |
| **[Katalon Studio](https://katalon.com/)** | Private (~$36M–$60M ARR) | Starts at $229/month (or $1,000/seat/year for Studio Enterprise); Cloud platform from $59/month | Free-forever plan: Local test creation & manual execution only; excludes CI/CD execution (no KRE) & capped at 2,000 TestOps uploads/month | Low-code test automation platform covering web, mobile, API, and desktop applications. |
| **[Testcontainers Cloud](https://testcontainers.com/cloud/)** | Division of Docker ($2.1B valuation) | Bundled in Docker Pro ($9/user/month, annual) or Team ($15/user/month, annual) | Docker Personal trial: evaluation access only; paid plans include 100 mins/mo (Pro) or 500 mins/mo (Team) before per-minute overages | Managed cloud container runtime for Testcontainers removing local daemon constraints and accelerating CI pipeline jobs. |
| **[Testsigma](https://testsigma.com/)** | Early-stage ($25M–$50M valuation / ~$8M–$10M ARR) | Test Management starts at $14/user/month; Automation Cloud plans start via custom quotes | 21-day free trial of Automation Cloud (full access); self-hosted Community Edition is free (requires managing own infrastructure/device grid) | Cloud-based low-code and AI-driven automation platform supporting web, mobile app, and API integration tests. |


## Open-Source GitHub Projects



- **[Testcontainers (Java)](https://github.com/testcontainers/testcontainers-java)**  

  **The reference implementation.** Java library that provides lightweight, throwaway instances of databases, Selenium browsers, message brokers, or anything else that runs in a Docker container for JUnit tests . **Adoption**: 8.7k+ GitHub stars, used by 31.3k+ projects, 511 contributors, and 92 releases (latest 2.0.5 in April 2026) . **Language bindings**: the same core concept is available for .NET, Python, Go, Node.js, and Rust—making it the most portable approach to containerized test dependencies. MIT licensed . Best for any team that wants real dependencies in tests without maintaining permanent test instances.



- **[Keploy](https://github.com/keploy/keploy)**  

  **Traffic-driven test generation.** Records real API and database traffic (HTTP, gRPC, GraphQL, Postgres, MySQL, MongoDB, Redis, Kafka, RabbitMQ) and replays it as test cases with mocks—no live infrastructure needed during replay. On Linux, capture uses eBPF at the network layer (kernel 5.10+); Apple Silicon macOS and x86-64 Windows run natively . **Open core**: Apache-2.0 licensed local record-and-replay core; Kubernetes capture, shared mock registry, dashboards, and SSO/RBAC are paid features. **Caveats**: CLI requires a Keploy account sign-in; no stable release in the past 12 months as of the source date . Best for teams that want to generate integration tests from real traffic rather than writing them by hand.



- **[dockerlet](https://github.com/metastable-void/dockerlet)**  

  A minimal Rust wrapper over `bollard` for spinning up transient containers (databases, message brokers) in integration tests. **Deliberately narrow**: Unix-socket Docker daemon only, no TLS, no auth file reads, no heavy dependency tree (no `rustls`, no `webpki-roots`, no `ring`) . Intended as a lightweight alternative to the broader Testcontainers Rust crate for projects that don't need its full surface area. **Status**: 0.0.0 placeholder as of the source date; 0.1.0 surface is planned . Best for Rust projects with simple container needs and a preference for minimal dependencies.



### Additional Strong Open-Source Options



- **Testcontainers (Python/Go/Node.js/.NET)** — The same core concept implemented across languages. Choose the binding matching your stack for consistent disposable-container testing.

- **Testcontainers Desktop** — Desktop app for running Testcontainers Cloud, included with Docker subscriptions. Best for developers on ARM Macs or resource-constrained machines .

- **Frameworks for building custom systems**: Use **Testcontainers** (your language's binding) as the backbone for disposable dependencies. Add **Keploy** if you want traffic-recorded tests alongside hand-written ones. Use **dockerlet** only if you're in Rust and want the absolute minimum wrapper. For local execution, **Docker Desktop** (with appropriate licensing) or Docker Engine on Linux provides the daemon.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Docker Desktop licensing requires attention**: organizations above 250 employees or $10M revenue need a paid subscription for commercial use . The open-source Docker Engine (Linux) does not carry this restriction.

- **Testcontainers Cloud pricing is consumption-based**: included minutes vary by Docker plan tier (100–1,500/month), with per-minute charges beyond that . Model your CI runtime before committing.

- **Keploy's local core is open (Apache-2.0), but advanced features are paid**: Kubernetes/production capture, shared mock registry, dashboards, and SSO/RBAC require paid plans . Evaluate whether the open core covers your needs.



---



**Made for developers, QA engineers, and platform teams that want integration tests against real dependencies without maintaining permanent test environments.**  

Let's make integration testing more open, container-native, and appropriately scoped.
