# 👁️ macOS Lab 4 — Log Collection & Threat Detection

## 🎯 Lab Objective
Collect, simulate, and analyze macOS security logs. Generate a failed-login event, query with Terminal, and export recent logs to JSON for SIEM ingestion or audit.

---

## 🧰 Tools & Technologies Used
- Console app (GUI)
- Terminal: `log show`
- JSON export
- (Optional) SIEM (Splunk / Wazuh / Elastic)

---

## 📁 Artifacts

| Artifact | Description |
|----------|-------------|
| `/Artifacts/README.md` | This documentation file |
| `/Artifacts/macos_logs.json` | Filtered JSON export (kept small for GitHub) |
| `/Artifacts/Screenshots/` | All screenshots for each step |

---

## 📌 Steps, Commands, and Artifacts

| Step | Action | Command/Action | Artifact (Screenshot/File) |
|------|--------|----------------|----------------------------|
| 1 | View Live Logs in Console | Open **Console** → select `system.log` | `step01_Console_Logs.png` |
| 2 | Simulate Failed Login | Lock screen → enter wrong password 3x → unlock | `step02_Failed_Login_Event.png` |
| 3 | Query Failed Login Events | `log show --predicate 'eventMessage contains "Failed"' --last 1h` | `step03_Failed_Login_Terminal.png` |
| 4 | Export Logs as JSON (filtered) | `log show --predicate '(eventMessage CONTAINS "Failed") OR (process == "loginwindow")' --last 30m --style json > macos_logs.json` | `step04_Export_JSON.png` <br> `macos_logs.json` |

---

## ✅ Summary
Demonstrated macOS log visibility, targeted event generation, CLI-based filtering, and JSON export suitable for SIEM ingestion. The export is intentionally filtered to remain <100MB for GitHub.

---

## 🔗 Previous Lab
⬅️ [Return to Lab 3 — Endpoint Hardening & Security Baseline](../Lab3_Hardening/Artifacts/README.md)


