<h1 align="center">Hey, I'm Hesham 👋</h1>

<p align="center">
  <b>Staff Platform Engineer</b> &nbsp;·&nbsp; Site Reliability Engineering &nbsp;·&nbsp; Kubernetes &amp; AWS
  <br>
  <sub>📍 Cairo, Egypt &nbsp;·&nbsp; building the platform that runs a Rails monolith across four production regions</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hesham-sherif-elmosalamy/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:heshamelsherif97@gmail.com">
    <img src="https://img.shields.io/badge/Email-16283C?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="https://heshamelsherif97.github.io">
    <img src="https://img.shields.io/badge/Website-2C6E7A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website">
  </a>
  <img src="https://img.shields.io/badge/AWS%20Certified-Solutions%20Architect-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS Certified Solutions Architect Associate">
</p>

---

## 🧭 What I actually do

I build and run the Kubernetes platform underneath a large Ruby on Rails monolith — the kind of system where a bad rollout is a customer-visible outage and a 3am page is a real possibility. 🚨

Most of my work sits at the boundary between **infrastructure and the developers who depend on it**: turning cluster-level capability into something application teams can self-serve, without them needing to learn Helm internals or my alerting stack.

- ☸️ **Multi-region EKS fleet** across development, staging, sandbox and four production regions
- 🚀 **GitOps + progressive delivery** with ArgoCD and Argo Rollouts — canary analysis, automated rollback
- 📈 **Event-driven autoscaling** with KEDA, replacing static and schedule-based scaling
- 🔐 **Security & supply chain** — fleet-wide vulnerability burndown, automated patching with Renovate
- 🤖 **AI platform work** — agent tooling standards, and sandboxed agent workloads running on Kubernetes
- 📟 **Production on-call** — incident response, post-incident reviews, and the runbooks that follow

---

## 🌱 Open source

I try to push fixes back upstream to the projects my platform depends on, rather than carrying patches internally. **Merged:**

| Project | What I fixed | PR |
|---|---|:--|
| 🔁 **Argo Rollouts** | A controller bug where one failed pod-metadata update cascaded into **every other rollout** in the cluster | [#4258](https://github.com/argoproj/argo-rollouts/pull/4258) |
| ⚖️ **AWS Load Balancer Controller** | Added support for **named ports on sidecar containers** | [#4237](https://github.com/kubernetes-sigs/aws-load-balancer-controller/pull/4237) |
| 🐙 **Argo CD** | Remediated **CVE-2025-29786** by upgrading the `expr-lang` dependency | [#22651](https://github.com/argoproj/argo-cd/pull/22651) |

Also proposed fixes to [Cilium](https://github.com/cilium/cilium/pull/38081) (Helm chart flexibility for `hostPort`/`externalIPs`), [Prometheus Adapter](https://github.com/kubernetes-sigs/prometheus-adapter/pull/685) (Go upgrade for CVEs), and a few more to [Argo CD](https://github.com/argoproj/argo-cd/pulls?q=is%3Apr+author%3Aheshamelsherif97) around retry semantics and health checks.

> 💡 Most of my day-to-day lives in private repos, so this is the visible slice. The [contribution graph](https://github.com/heshamelsherif97) tells a fuller story than the repo list.

---

## 🧰 Toolbox

**Orchestration & Platform**

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Argo](https://img.shields.io/badge/ArgoCD%20%2B%20Rollouts-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![KEDA](https://img.shields.io/badge/KEDA-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Cilium](https://img.shields.io/badge/Cilium-F8C517?style=flat-square&logo=cilium&logoColor=black)
![Envoy](https://img.shields.io/badge/Envoy%20Gateway-AC6199?style=flat-square&logo=envoyproxy&logoColor=white)

**Cloud & IaC**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Observability & Data**

![Datadog](https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Ruby](https://img.shields.io/badge/Ruby-CC342D?style=flat-square&logo=ruby&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Go templates](https://img.shields.io/badge/Go%20templates-00ADD8?style=flat-square&logo=go&logoColor=white)

---

## 📌 Currently

- 🏗️ Architecting connection pooling and traffic control for a Rails monolith at scale
- 🤖 Working on agent tooling standards and sandboxed agent workloads on Kubernetes
- 🔭 Watching [agent-sandbox](https://github.com/kubernetes-sigs/agent-sandbox), [kagent](https://kagent.dev) and [agentgateway](https://agentgateway.dev) closely
- 📚 Always reading post-incident writeups &mdash; other people's outages are cheap lessons

---

## 🤝 Say hello

Always happy to talk **platform engineering**, **Kubernetes at scale**, **progressive delivery**, or where **AI agents** fit into developer platforms. ☕

<p align="center">
  <a href="https://www.linkedin.com/in/hesham-sherif-elmosalamy/"><b>LinkedIn</b></a> &nbsp;·&nbsp;
  <a href="mailto:heshamelsherif97@gmail.com"><b>Email</b></a> &nbsp;·&nbsp;
  <a href="https://heshamelsherif97.github.io"><b>heshamelsherif97.github.io</b></a>
</p>
