# macOS Security Labs (Portfolio)

Hands-on macOS labs demonstrating endpoint hardening, log collection, and threat detection workflows aligned to enterprise/federal environments (e.g., CBP IT Analyst).

---

## 🎯 Labs Overview

| Lab | Focus | Key Artifacts | Docs |
|-----|-------|---------------|------|
| **Lab 3** | Endpoint Hardening (Firewall, FileVault, Gatekeeper, Lock screen policy, Safari hardened) | Screenshots + `security_baseline.txt` | [Lab 3 README](Lab3_Hardening/Artifacts/README.md) |
| **Lab 4** | Log Collection & Threat Detection (failed login simulation, JSON export) | Screenshots + filtered `macos_logs.json` | [Lab 4 README](Lab4_Logging/Artifacts/README.md) |

> **Note:** The full raw macOS log export exceeded GitHub’s 100MB limit. A filtered JSON is included for review and SIEM ingestion.

---

## 🧪 Tech Used

- macOS System Settings (Ventura/Sonoma)
- Terminal: `system_profiler`, `log show`
- Console app
- (Optional) SIEM: Splunk / Wazuh / Elastic

---

## 📂 Repo Structure


---

## 🛠️ Future Work (Planned)

- **Lab 5:** Ingest filtered `macos_logs.json` into SIEM (Splunk/Wazuh) and build dashboard for failed logins.
- Add detection write-up and screenshot(s) for dashboard.
