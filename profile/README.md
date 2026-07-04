# 🏛️ RPDevs-Vault Security Command Center

Welcome to the automated core of **RPDevs-Vault**. This organization is a high-performance sovereign hub managed by a robust 9-repo tiered architecture dedicated to infrastructure archival, governance, task sync, build fleets, secret brokers, and GitOps distribution.

---

## 📊 The 9-Repo Management Architecture

| Tier | Manager | Role / Function | Operational Status |
| :--- | :--- | :--- | :--- |
| **Tier 0** | **[github-manager](https://github.com/RPDevs-Vault/github-manager)** | 🌐 **Global Cockpit**: Live health, runner telemetry, & API limits. | ![Health](https://img.shields.io/badge/Cockpit-Active-brightgreen) |
| **Tier 0.5** | **[monitor-manager](https://github.com/RPDevs-Vault/monitor-manager)** | 🚨 **Observability**: Uptime verification, probes, and notification alerts. | ![Monitor](https://img.shields.io/badge/Monitor-Active-brightgreen) |
| **Tier 1** | **[vault-manager](https://github.com/RPDevs-Vault/vault-manager)** | 🛡️ **Governance Hub**: Policies, archival, syncs, & dispatch orchestration. | ![Sync Status](https://img.shields.io/badge/Governance-Active-brightgreen) |
| **Tier 1.5** | **[identity-manager](https://github.com/RPDevs-Vault/identity-manager)** | 🔑 **Key Broker**: Secrets, FIDO2/Age pairing, & environment validation. | ![Identity](https://img.shields.io/badge/Identity-Secure-brightgreen) |
| **Tier 2** | **[container-manager](https://github.com/RPDevs-Vault/container-manager)** | 🏗️ **Build Fleet**: CI/CD, OCI packaging, Ccache, & DaaS compilation. | ![Build Fleet](https://img.shields.io/badge/Fleet-Online-brightgreen) |
| **Tier 3** | **[project-manager](https://github.com/RPDevs-Vault/project-manager)** | 🗺️ **Task Sync**: Cross-org issue aggregation & central roadmap CLI. | ![Sync](https://img.shields.io/badge/Roadmap-Active-brightgreen) |
| **Tier 4** | **[distributor-manager](https://github.com/RPDevs-Vault/distributor-manager)** | 📦 **Release Gateway**: Final artifact publishing and GitHub Releases. | ![Release](https://img.shields.io/badge/Release-Active-brightgreen) |
| **Tier 4.5** | **[deploy-manager](https://github.com/RPDevs-Vault/deploy-manager)** | 🚀 **GitOps Deployer**: Ansible host playbooks, Docker Compose maps. | ![Deploy](https://img.shields.io/badge/Deploy-Active-brightgreen) |
| **Tier 5** | **[thought-manager](https://github.com/RPDevs-Vault/thought-manager)** | 🧠 **Knowledge Core**: ADRs, agent skillbooks, guidelines, & templates. | ![Thought](https://img.shields.io/badge/Thought-Active-brightgreen) |

---

## 🚀 Key Capabilities

```
+-------------------------------------------------------------------------------+
|                            RPDevs-Vault Architecture                          |
+-------------------------------------------------------------------------------+
|                                                                               |
|   [github-manager] <----> [monitor-manager] <----> [vault-manager]            |
|          |                                                |                   |
|          v                                                v                   |
|   [identity-manager]                               [thought-manager]          |
|    (FIDO2 + Age Key)                               (ADRs / Guidelines)        |
|          |                                                |                   |
|          v                                                v                   |
|   [container-manager]                             [project-manager]           |
|    (Runner Build fleet)                            (Cross-org sync)           |
|          |                                                                    |
|          v                                                                    |
|   [distributor-manager] ----> [deploy-manager]                                |
|    (Release gateway)           (GitOps / Ansible)                             |
|                                                                               |
+-------------------------------------------------------------------------------+
```

*   **Hardware-Bound Secrets (Tier 1.5):** Symmetric Age encryption natively bound to physical FIDO2 hardware keys via custom wrappers. Credentials only exist in-memory during step execution, mitigating persistent disk compromise.
*   **Decoupled GitOps (Tier 4.5):** Absolute decoupling between compilation (`container-manager`) and remote target deployment (`deploy-manager`) using playbooks and environment validation routines.
*   **Depends-as-a-Service (Tier 2):** Fast-tracked cross-compilation utilizing local caching over shared network attachments (NFS/ccache) across multiple runner architectures.
*   **Digital Nervous System (Tier 0):** Real-time monitoring of self-hosted nodes and automation telemetry with automatic alerts upon probe failures.

### 📦 [View Organization Packages](https://github.com/orgs/RPDevs-Vault/packages)

*This organization is fully managed by autonomous DevOps automation.*
