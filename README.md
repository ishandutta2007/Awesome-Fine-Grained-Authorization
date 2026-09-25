# Awesome-Fine-Grained-Authorization

## Top Fine-Grained Authorization (FGA) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Relationship-Based Access Control (ReBAC), Zanzibar-style Permissions, Policy-as-Code & Resource-Level Authorization*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Fine-Grained Authorization (FGA)**. These systems answer questions like “Can user X perform action Y on resource Z?” at the individual-object level using relationship tuples, schemas, or policy languages—far beyond simple roles.



**Examples** include Auth0 FGA, OpenFGA, Permit.io, Cerbos, Oso, AuthZed / SpiceDB, Aserto, Topaz, and Styra DAS (the category leaders).



**Open-source emphasis**: This domain is unusually strong in open source. **OpenFGA** (CNCF), **SpiceDB**, **Cerbos**, **Oso**, and related engines provide production-grade FGA that many teams self-host. Commercial offerings mainly add managed hosting, enterprise support, and integrated developer experience. This section heavily expands the open options.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Auth0 FGA](https://fga.dev/)**  

  Managed fine-grained authorization service from Okta/Auth0 built on OpenFGA—relationship-based permissions with enterprise scale, SDKs, and tight Auth0 identity integration.



- **[Permit.io](https://www.permit.io/)**  

  Full-stack authorization platform offering policy-as-code, no-code UI, ReBAC/ABAC/RBAC models, and managed decision APIs for application developers.



- **[AuthZed (SpiceDB Cloud)](https://authzed.com/)**  

  Managed service for SpiceDB—the Zanzibar-inspired authorization database—providing hosted relationship stores, schema management, and enterprise support.



- **[Aserto](https://www.aserto.com/)**  

  Cloud authorization platform focused on policy-as-code, developer-friendly SDKs, and fine-grained access control for modern applications.



- **[Styra DAS](https://www.styra.com/)**  

  Enterprise policy management platform built around Open Policy Agent (OPA)—governance, decision logging, and large-scale policy distribution.



- **[Oso Cloud](https://www.osohq.com/)**  

  Managed authorization service from the Oso team using the Polar policy language, aimed at developers embedding fine-grained checks in applications.



- **[Cerbos Hub / managed offerings](https://www.cerbos.dev/)**  

  Commercial hosting and collaboration features around the open-source Cerbos policy decision point.



- **[Topaz and related managed policy runtimes](https://www.example.com/)**  

  Hosted or enterprise distributions of open policy engines used for fine-grained and attribute-based decisions.



- **[Other CIAM-bundled FGA services](https://www.example.com/)**  

  Additional managed fine-grained authorization capabilities offered by identity platforms.



## Open-Source GitHub Projects

- **[OpenFGA](https://github.com/openfga/openfga)**  

  High-performance, CNCF open-source authorization engine inspired by Google Zanzibar—relationship-based access control (ReBAC) with a flexible modeling language, SDKs, and self-hostable store (Apache 2.0).



- **[SpiceDB](https://github.com/authzed/spicedb)**  

  Open-source Zanzibar-inspired authorization database from AuthZed—schema + relationships, strong consistency options, high throughput, and production use at scale (Apache 2.0).



- **[Cerbos](https://github.com/cerbos/cerbos)**  

  Open-source policy decision point focused on fine-grained, context-aware authorization with a simple YAML/JSON policy language and sidecar or embedded deployment.



- **[Oso](https://github.com/osohq/oso)**  

  Open-source authorization library using the Polar policy language—embed fine-grained rules next to your application code (library is open; cloud is commercial).



- **[Topaz](https://github.com/aserto-dev/topaz)**  

  Open-source authorization service that combines policy (OPA/Rego) with a local directory for fine-grained and relationship-aware decisions.



- **[Open Policy Agent (OPA)](https://github.com/open-policy-agent/opa)**  

  General-purpose open policy engine widely used for authorization decisions; often paired with Styra or custom FGA models.



- **[Casbin](https://github.com/casbin/casbin)**  

  Lightweight open-source authorization library supporting ACL, RBAC, ABAC, and other models embeddable in many languages.



- **[Permify and other Zanzibar-style open engines](https://github.com/)**  

  Additional open-source relationship-based authorization servers inspired by the Zanzibar paper.



- **[Cedar (Amazon)](https://github.com/cedar-policy)**  

  Open-source policy language and engine designed for expressive, analyzable authorization rules.



- **[SDKs, modeling tools, and playground open projects](https://github.com/openfga)**  

  Client libraries, CLI tools, VS Code extensions, and sample stores that accelerate adoption of OpenFGA and related engines.



### Additional Strong Open-Source Options

- Self-hosting **OpenFGA** or **SpiceDB** as the central relationship store for multi-tenant or resource-level permissions.

- Embedding **Cerbos**, **Oso**, or **Casbin** for in-process or sidecar policy decisions.

- Combining open FGA engines with your existing identity provider and application data.

- Using commercial managed services (Auth0 FGA, AuthZed, Permit.io, etc.) when you prefer not to operate the authorization store yourself.

- Focusing open-source efforts on transparent permission models, auditability, and avoiding vendor lock-in for core authorization logic.



**Frameworks for building custom systems**: Model your domain relationships (users, resources, roles, parent/child) in OpenFGA or SpiceDB schema → write relationship tuples from your application → call Check / ListObjects APIs on every sensitive action → optionally layer a policy engine (Cerbos/OPA) for attribute-rich rules. Suitable for any application that needs object-level permissions. Many teams start open-source and add managed hosting only when operational burden grows.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- Authorization systems are security-critical. Incorrect models or policies can create privilege-escalation or data-exposure risks. Thorough testing, least-privilege design, and security review are required. This list is not security or compliance advice.



---

**Made for application security, platform, and backend engineering teams.**

Let's keep permissions fine-grained, auditable, and as open as practical.
