# 👁️ macOS Lab 4 — Log Collection & Threat Detection

## 🎯 Lab Objective
This lab demonstrates the ability to collect, analyze, and export macOS system logs for security monitoring purposes. The lab includes generating a failed login security event, querying logs via Terminal, and exporting results in JSON format for use in a SIEM.

---

## 🧰 Tools & Technologies Used
- macOS Terminal (`log`, `grep`, `system.log`)
- Console App (GUI log viewer)
- JSON export via `log show` command
- (Optional) SIEM tools: Splunk, Wazuh, Elastic Stack

---

## 📁 Artifacts

| Artifact | Description |
|----------|-------------|
| `/Artifacts/README.md` | This documentation file |
| `/Artifacts/macos_logs.json` | Exported log output in JSON format |
| `/Artifacts/Screenshots/` | Folder containing screenshot evidence for this lab |

---

## 📌 Steps, Commands, and Artifacts

| Step | Action | Command/Action | Artifact (Screenshot/File) |
|------|--------|----------------|----------------------------|
| 1 | View Live Logs in Console App | Open Console → `system.log` | `Step_01_Console_Logs.png` |
| 2 | Simulate Failed Login Attempt | Lock screen → enter wrong password 3x | `Step_02_Failed_Login_Event.png` |
| 3 | Query Failed Login Events via Terminal | `log show --predicate 'eventMessage contains "Failed"' --last 1h` | `Step_03_Failed_Login_Terminal.png` |
| 4 | Export Logs as JSON | `log show --last 30m --style json > macos_logs.json` | `Step_04_Export_JSON.png` <br> `macos_logs.json` |
| 5 | (Optional) Forward logs to SIEM | Upload JSON file or configure agent | `Step_05_SIEM_Dashboard.png` |

---

## ✅ Summary

This lab demonstrates core security monitoring capabilities on macOS: triggering events, collecting logs, querying them via CLI, and exporting in structured format. These skills are essential for roles in **incident response** and **SOC operations**.

---

## 🔗 Previous Lab

⬅️ [Return to Lab 3 — Endpoint Hardening & Security Baseline](../Lab3_Hardening/README.md)

