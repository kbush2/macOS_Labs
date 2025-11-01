# 🛡️ macOS Lab 3 — Endpoint Hardening & Security Baseline

## 🎯 Lab Objective
Harden a macOS system using built-in security controls (Firewall, FileVault, Gatekeeper, lock policy, and Safari privacy/security) and document the evidence and exported configuration.

---

## 🧰 Tools & Technologies Used
- macOS System Settings (Ventura / Sonoma)
- Terminal: `system_profiler`
- Safari Settings
- Local file export

---

## 📁 Artifacts

| Artifact | Description |
|----------|-------------|
| `/Artifacts/README.md` | This documentation file |
| `/Artifacts/security_baseline.txt` | Export from Terminal containing Firewall/FileVault state |
| `/Artifacts/Screenshots/` | All screenshots for each step |

---

## 📌 Steps, Commands, and Artifacts

| Step | Action | Command/Action | Artifact (Screenshot/File) |
|------|--------|----------------|----------------------------|
| 1 | Enable macOS Firewall | System Settings → Network → Firewall → **Turn On** | `step01_Firewall_On.png` |
| 2 | Turn On FileVault (Disk Encryption) | System Settings → Privacy & Security → FileVault → **Turn On** | `step02_FileVault_Encrypting.png` |
| 3 | Restrict App Downloads with Gatekeeper | System Settings → Privacy & Security → Security → **App Store and identified developers** | `step03_Gatekeeper_Restricted.png` |
| 4 | Enforce Immediate Password Lock | System Settings → Lock Screen → Require Password: **Immediately** | `step04_Password_Lock_Immediately.png` |
| 5 | Harden Safari Browser Settings | Safari → Settings → Privacy/Security (cross-site tracking blocked, auto-fill reduced, fraud warnings on) | `step05_Safari_Hardened.png` |
| 6 | Export Security Baseline | `sudo system_profiler SPFirewallDataType SPFileVaultDataType > security_baseline.txt` | `step06_Security_Export.png` <br> `security_baseline.txt` |

---

## ✅ Summary
This device now reflects a baseline-hardened macOS posture suitable for enterprise/federal environments. Evidence is captured in screenshots; `security_baseline.txt` provides a terminal-exported record of key security states.

---

## 🔗 Next Lab
➡️ [Proceed to Lab 4 — macOS Log Collection & Threat Detection](../../Lab4_Logging/Artifacts/README.md)
