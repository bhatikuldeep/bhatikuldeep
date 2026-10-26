### Hi, I'm Kuldeep

**Senior Staff Field Engineer at Kong Professional Services, Netherlands.**
I help enterprises run APIs and AI agents in production.

[kuldeepbhati.com](https://kuldeepbhati.com) · [LinkedIn](https://www.linkedin.com/in/bhatikuldeep/) · [RSS](https://kuldeepbhati.com/index.xml)

I work with the teams that run API platforms inside large companies: banks, insurers, retailers, pharma. Some are putting Kong into production for the first time, some are moving from a self-managed setup to Konnect, and more and more of them want to know how to let AI agents use their APIs safely. I started on API platforms in 2014 with Apigee, then 3scale, Mashery and MuleSoft, and joined Kong in 2023. The products changed; the problems mostly didn't.

Whatever the project, the goal is the same: get the customer live, help them see real value from the platform, and leave them able to run it themselves.

### What I work on

- **Platform ops.** Running the gateway well after go-live: upgrades, ownership, capacity, and the observability that tells you why something broke.
- **Security and traffic management.** Identity with OIDC and mTLS, rate limits and quotas, and routing rules that keep one noisy consumer from hurting everyone else.
- **APIOps.** Gateway config in git, checked in CI and applied by a pipeline, so a change to a route doesn't need a ticket or a meeting.
- **Production readiness.** Hardening before go-live: configuration review, failure testing, certificates, and a checklist the team can own.
- **AI and agentic work.** Token budgets, model fallback, MCP and per-tool authorization: running LLM and agent traffic safely, including exposing existing REST APIs or MCP servers to agents with proper security and insight into access and cost.

### Upstream

When something is broken in a tool I depend on, I'd rather fix it upstream than work around it.

| Project | Contribution |
|---|---|
| **[Kong/kong-operator](https://github.com/Kong/kong-operator/pull/5982)** | Certificate rotation without 401s: register the renewed `KonnectExtension` client certificate with Konnect before data planes use it |
| **[Kong/developer.konghq.com](https://github.com/Kong/developer.konghq.com/pull/7615)** | Document that `kongctl lint` uses vacuum rulesets, with a working example |
| **[Kong/kwot](https://github.com/Kong/kwot/pull/32)** | Inject RBAC user tokens from environment variables (CI secrets, no YAML pre-processing) |

### Projects

| Repository | What it does |
|---|---|
| **[kong-grafana-observability-stack](https://github.com/bhatikuldeep/kong-grafana-observability-stack)** | Metrics, logs and traces from a Konnect hybrid gateway, wired into Prometheus, Loki and Tempo on a local kind cluster with one command |
| **[kong-konnect-observability-datadog](https://github.com/bhatikuldeep/kong-konnect-observability-datadog)** | The same idea wired into Datadog, as Terraform |
| **[dvm](https://github.com/bhatikuldeep/dvm)** | decK Version Manager, written during a Kong 2.8 to 3.4 upgrade. For new work I recommend [pinning tools with mise](https://kuldeepbhati.com/posts/pin-cli-versions-per-project-with-mise/) instead |

<details>
<summary><b>From the Apigee years</b></summary>
<br>

| Repository | What it does |
|---|---|
| **[hello-world-elk-logging](https://github.com/bhatikuldeep/hello-world-elk-logging)** | Message logging from Apigee Edge to the ELK stack |
| **[apigee-hybrid-x-provision](https://github.com/bhatikuldeep/apigee-hybrid-x-provision)** | Provisioning the Apigee hybrid control plane with Terraform |
| **[maven-archetype-apigee-proxy](https://github.com/bhatikuldeep/maven-archetype-apigee-proxy)** | Maven archetype that scaffolds an Apigee Edge API proxy |

</details>

### Writing

Notes, tools and fixes from real enterprise gateway projects, at **[kuldeepbhati.com](https://kuldeepbhati.com/posts/)**:

<!-- writing:start -->
- [From plugin to entities: local Ollama behind Kong AI Gateway 2.x](https://kuldeepbhati.com/posts/ollama-kong-ai-gateway-2-konnect/)
- [Stop switching tool versions: pin every CLI per project with mise](https://kuldeepbhati.com/posts/pin-cli-versions-per-project-with-mise/)
- [Kong hybrid mode on Kubernetes with Helm, and what keeps working when the control plane doesn't](https://kuldeepbhati.com/posts/kong-hybrid-gateway-setup-via-helm/)
- [Your CI is green, Kong says no: lint route paths before you deploy](https://kuldeepbhati.com/posts/kong-deck-lint-validation/)
<!-- writing:end -->

### Toolbox

`Kong Gateway` · `Konnect` · `AI Gateway` · `decK` · `kongctl` · `Terraform` · `Kubernetes` · `Helm` · `OIDC` · `OpenTelemetry` · `Grafana` · `Datadog` · `Apigee` · `MuleSoft`

<sub>Based in the Netherlands. Views are my own.</sub>
