# 🏛️ RPDevs-Vault Security Command Center

Welcome to the automated core of **RPDevs-Vault**. This organization is a high-performance sovereign hub managed by a consolidated **4-Core Manager Architecture** dedicated to infrastructure telemetry, governance, build fleets, key brokering, task sync, and GitOps distribution.

---

## 📊 The 4-Core Manager Architecture

| Tier | Manager | Role / Function | Operational Status |
| :--- | :--- | :--- | :--- |
| **Tier 1** | **[ops-manager](https://github.com/RPDevs-Vault/ops-manager)** | 🌐 **Global Cockpit & Governance**: Live health, runner telemetry, uptime probes, identity validation, & FIDO2/Age key brokering. | ![Ops Status](https://img.shields.io/badge/Ops-Active-brightgreen) |
| **Tier 2** | **[builder-manager](https://github.com/RPDevs-Vault/builder-manager)** | 🏗️ **Build Fleet & Dependency Engine**: Automated dependency scanning, multi-platform container compilation, OCI packaging, & NFS/Ccache build caching. | ![Build Fleet](https://img.shields.io/badge/Builder-Online-brightgreen) |
| **Tier 3** | **[delivery-manager](https://github.com/RPDevs-Vault/delivery-manager)** | 🚀 **GitOps & Release Gateway**: Releases packaging, Ansible host playbook provisioning, and docker-compose deployment orchestration. | ![Delivery Status](https://img.shields.io/badge/Delivery-Active-brightgreen) |
| **Tier 4** | **[workspace-manager](https://github.com/RPDevs-Vault/workspace-manager)** | 🧠 **Workspace & Task Sync**: Workspace-level project CLI scanners, cross-org issue/PR roadmap sync, ADR decision logs, and agent skill templates. | ![Workspace Status](https://img.shields.io/badge/Workspace-Syncing-brightgreen) |

---

## 🚀 Key Capabilities

```
+-------------------------------------------------------------------------------+
|                            RPDevs-Vault Architecture                          |
+-------------------------------------------------------------------------------+
|                                                                               |
|             [ops-manager]  <===================> [workspace-manager]          |
|         (Telemetry / FIDO2 / Probes)             (ADRs / Tasks / CLI)         |
|                      ||                                   ||                  |
|                      || Triggers                          || Generates        |
|                      \/                                   \/                  |
|           [builder-manager] ===================> [delivery-manager]           |
|         (CI/CD / Dependency Engine)               (GitOps / Ansible)          |
|                                                                               |
+-------------------------------------------------------------------------------+
```

* **Hardware-Bound Secrets (Tier 1):** Symmetric Age encryption natively bound to physical FIDO2 hardware keys via custom wrappers inside `ops-manager/identity/`. Credentials only exist in-memory during workflow executions.
* **Unified Build Fleet (Tier 2):** Decoupled, high-speed cross-compilation pipeline utilizing local shared caching over NFS/Ccache across runner platforms, integrated with automated weekly dependency scans.
* **Decoupled Release & Deploy (Tier 3):** Absolute decoupling between code compilation and remote host deployment. `delivery-manager` automates target host provisioning using isolated Ansible playbooks and target environments.
* **Unified Workspaces (Tier 4):** Cross-organization issue aggregation, automated backlog roadmaps, and central ADRs (Architectural Decision Records) tracked dynamically in `workspace-manager`.

### 📦 [View Organization Packages](https://github.com/orgs/RPDevs-Vault/packages)

*This organization is fully managed by autonomous DevOps automation.*

