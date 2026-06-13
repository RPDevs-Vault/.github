# 🏛️ RPDevs Vault Command Center

Welcome to the automated core of **RPDevs Vault**. This organization is a high-performance hub dedicated to infrastructure archival, governance automation, and containerized build fleets.

---

## 📊 Comprehensive Status

| Command Center | Status | Focus |
| :--- | :--- | :--- |
| **[vault-manager](https://github.com/RPDevs-Vault/vault-manager)** | ![Sync Status](https://img.shields.io/badge/Sync-Active-brightgreen) | Governance, Security, & Archival |
| **[container-manager](https://github.com/RPDevs-Vault/container-manager)** | ![Build Fleet](https://img.shields.io/badge/Fleet-Online-brightgreen) | CI/CD, Registry, & Asset Discovery |
| **[Package Registry](https://github.com/orgs/RPDevs-Vault/packages)** | ![Packages](https://img.shields.io/badge/Registry-Public-blue) | OCI Artifacts & Build Runners |

---

### 🚀 Infrastructure Control (`container-manager`)
*   **[Container Build Fleet](https://github.com/RPDevs-Vault/container-manager/actions):** High-throughput image builds utilizing local `vault-builder` runners with cloud fallback.
*   **[Asset Harvester](https://github.com/RPDevs-Vault/container-manager/blob/main/.github/workflows/docker-collector.yml):** Weekly organization-wide scan for Docker and Compose assets across 260+ repositories.
*   **[Fleet Registry](https://github.com/RPDevs-Vault/container-manager/tree/main/containers):** Centralized deployment configurations and one-liner execution scripts.

### 🛡️ Governance Control (`vault-manager`)
*   **[Global Sync Engine](https://github.com/RPDevs-Vault/vault-manager/blob/main/.github/workflows/sync-forks.yml):** Daily automated synchronization of all forked repositories.
*   **[Policy Enforcer](https://github.com/RPDevs-Vault/vault-manager/blob/main/.github/workflows/policy-enforcer.yml):** Standardizing labels, branch protection, and notification settings organization-wide.
*   **[Archival Engine](https://github.com/RPDevs-Vault/vault-manager/blob/main/.github/workflows/archive-engine.yml):** Automated monorepo backups and stale project auditing.

---

### 📦 [View Organization Packages](https://github.com/orgs/RPDevs-Vault/packages)

*This organization is fully managed by autonomous DevOps automation.*
