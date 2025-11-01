
# 🛡️ macOS Lab 3 — Endpoint Hardening & Security Baseline

## 🎯 Lab Objective
The purpose of this lab is to harden a macOS system using built-in security features such as Firewall, FileVault, Gatekeeper, and privacy settings—demonstrating the ability to apply enterprise-level security controls suitable for roles like **CBP IT Analyst**.

---

## 🧰 Tools & Technologies Used
- macOS System Settings (Ventura / Sonoma)
- Terminal (`system_profiler`)
- Safari Settings (for browser hardening)
- Local file export

---

## 📁 Artifacts

| Artifact | Description |
|----------|-------------|
| `/Artifacts/README.md` | This documentation file |
| `/Artifacts/security_baseline.txt` | Export of macOS security configuration via Terminal |
| `/Artifacts/Screenshots/` | Folder containing screenshot evidence for this lab |

---

## 📌 Steps, Commands, and Artifacts

| Step | Action | Command/Action | Artifact (Screenshot/File) |
|------|--------|----------------|----------------------------|
| 1 | Enable macOS Firewall | System Settings → Network → Firewall → **Turn On** | `step01_Firewall_On.png` |
| 2 | Turn On FileVault (Disk Encryption) | System Settings → Privacy & Security → FileVault → **Turn On** | `step02_FileVault_Encrypting.png` |
| 3 | Restrict App Downloads with Gatekeeper | System Settings → Privacy & Security → Security → **Allow apps from App Store and identified developers** | `step03_Gatekeeper_Restricted.png` |
| 4 | Enforce Immediate Password Lock | System Settings → Lock Screen → Require Password: **Immediately** | `step04_Password_Lock_Immediately.png` |
| 5 | Harden Safari Browser Settings | Safari → Settings → Privacy / Security (Cross-site tracking blocked, AutoFill reduced) | `step05_Safari_Hardened.png` |
| 6 | Export Security Baseline from Terminal | `sudo system_profiler SPFirewallDataType SPFileVaultDataType > security_baseline.txt` | `step06_Security_Export.png` <br> `security_baseline.txt` |

---

## ✅ Summary

This macOS device is now configured with baseline hardening suitable for enterprise or federal security requirements. Key security measures (Firewall, FileVault, Gatekeeper, password policy, and Safari privacy settings) were successfully applied and documented. The exported system configuration (`security_baseline.txt`) serves as proof of compliance and can be used for audits or repeat deployments.

---

## 🔗 Next Lab

➡️ [Proceed to Lab 4 — macOS Log Collection & Threat Detection](../Lab4_Logging/README.md)
