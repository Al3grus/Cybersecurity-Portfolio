# Cybersecurity Portfolio — Al3grus

Repository of practical cybersecurity projects and tools.  
Projects are stored here with summaries and full reports.  
Tools are listed here but link to their own dedicated repositories.  
All work was produced in controlled lab environments.

---

## ⭐ Featured - Project in development

### [Argus SOC — AI-Augmented Security Operations Center](https://github.com/Al3grus/Argus-SOC)

*Edge to cloud. Threat to response.*

A fully operational SOC lab built on Raspberry Pi hardware and a cloud-hosted 
central platform, designed to mirror real MSSP/MDR infrastructure.

**Stack:** Wazuh SIEM · Suricata NIDS · Zeek · Velociraptor DFIR · Claude API (AI triage) · 
n8n · WireGuard VPN · Cowrie Honeypot · Frigate (AI camera) · Grafana · PagerDuty · Telegram Bot

**Architecture:** Hetzner VPS (cloud SOC platform, Helsinki) + Pi 5 (home infrastructure + 
physical security) + Pi 3B+ (remote edge sensor) — the exact topology used by MSSPs. SPAN port mirroring provides full Lab VLAN traffic visibility to Suricata and Zeek.

**What it demonstrates:**
- End-to-end incident workflow: detection → AI triage → alert → PagerDuty escalation → PDF report
- Claude API integration for real-time alert triage and ~80% noise reduction
- Multi-agent SIEM with custom detection rules and MITRE ATT&CK mapping
- Cloud-hosted SOC platform on GDPR-compliant x86_64 VPS — Wazuh full stack + n8n (SOAR) + Velociraptor
- Layered network detection: Suricata (signature) + Zeek (protocol metadata) on hardware SPAN port
- Live endpoint forensics with Velociraptor — artifact collection and VQL threat hunting
- Physical security integration: OV5647 camera → MediaMTX → Frigate AI detection → SOC alerts
- Five documented red team scenarios across the full kill chain
- Detection gap analysis per scenario — a Detection Engineering deliverable

---

## 📂 Projects

- **[Red Team Pentest](Projects/RedTeam-Pentest/summary.md)**
  
  Full engagement simulation → reconnaissance → exploitation → post-exploitation → 30-page professional report.

- **[Blue Team DFIR](Projects/BlueTeam-DFIR/summary.md)**

  Linux audit log analysis, event timeline reconstruction, IOC identification, containment actions.  

---

## 🛠️ Tools
Tools I developed and maintain are hosted as separate GitHub repositories.  
This section provides direct links to them:

- **[OpenVPN-Manager](https://github.com/Al3grus/OpenVPN-Manager)** | Manage and switch OpenVPN profiles with ease.
  
- *(More to come as I expand my tooling.)*

---

## 📜 Certifications

- **eJPT (Junior Penetration Tester) — INE** — Issued Nov 2025 - certified with 97% score
- **Cybersecurity Bootcamp — Code Labs Academy** (Apr–Oct 2025)
- **Certified in Cybersecurity (CC) — ISC2** — Issued Mar 2025 (expires Mar 2028)  
- **Introduction to Programming with Python — Harvard** — Issued Apr 2024 
- **Anti-Money Laundering (AML) — Thomson Reuters** — Issued Feb 2023 

---

### ⚠️ Disclaimer

All work uses **sanitized data** in **controlled lab environments**.  
No unauthorized access or testing of real systems.
