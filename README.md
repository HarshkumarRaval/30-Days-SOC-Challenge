# 🛡️ 30 Days SOC Analyst Challenge

> A daily, hands-on build log of a complete **Security Operations Center home lab** — from log collection to detection engineering to live attack investigation.
>
> Following the [30 Days SOC Analyst Challenge](https://www.youtube.com/@MyDFIR) by **Steven (MyDFIR)**.

**Author:** **Harshkumar Raval** · `HRTechVerse`
**Personal brand:** *"I think like an attacker to defend like a professional. Calm mind, relentless hunt."*

---

## 📌 About This Repository

This repo documents every day of the challenge with notes, diagrams, detection rules, and investigation evidence. The goal isn't to *watch* a SOC get built — it's to **build it, attack it, detect the attack, and investigate it**, then leave a defensible trail of work behind.

Each day includes:
- 📝 **Notes** — concepts, commands, and decisions
- 📊 **Diagrams** — architecture and logical network maps
- 🔎 **Evidence** — screenshots, alerts, and investigation write-ups

---

## 🗺️ Roadmap

| Week | Theme | Focus |
|:----:|-------|-------|
| **1** | Foundation | ELK stack setup + log ingestion (incl. Sysmon) |
| **2** | Detection | Public SSH/RDP server + brute-force alerts & dashboards |
| **3** | Adversary Simulation | C2 server with Mythic + attacking the lab |
| **4** | Response | Ticketing system integration + full investigations |

---

## 📅 Progress Tracker

| Day | Topic | Notes | Status |
|:---:|-------|:-----:|:------:|
| 00 | Introduction & 30-Day Roadmap | [📄](notes/Day-00-Introduction.md) | ✅ |
| 01 | Logical Network Diagram (draw.io) | [📄](notes/Day-01-Logical-Diagram.md) | ✅ |
| 02 | _Coming soon_ | — | ⬜ |
| ... | ... | — | ⬜ |

> 🗺️ **Lab blueprint:** [`diagrams/soc-lab-architecture.svg`](diagrams/soc-lab-architecture.svg)

*Tracker updated daily as the challenge progresses.*

---

## 🧰 Tech Stack

| Category | Tools |
|----------|-------|
| **SIEM / Logging** | Elasticsearch, Kibana, Logstash |
| **Endpoint Telemetry** | Sysmon |
| **Adversary Simulation** | Mythic (C2) |
| **Frameworks** | MITRE ATT&CK |
| **Infrastructure** | Vultr / Cloud VMs (Windows + Linux) |
| **Case Management** | Ticketing system (Week 4) |

---

## 📂 Repository Structure

```
30-Days-SOC-Challenge/
├── README.md            ← you are here
├── notes/               ← daily write-ups
├── diagrams/            ← architecture & network diagrams
├── reports/             ← formatted PDF reports
└── evidence/            ← screenshots, alerts, investigations
```

---

## 🎯 Skills Demonstrated

`SIEM Administration` · `Log Ingestion` · `Detection Engineering` · `Threat Detection` ·
`Incident Investigation` · `MITRE ATT&CK Mapping` · `Adversary Simulation` · `Documentation`

---

> 📺 Cybersecurity, AI & tech content by **Harshkumar Raval** on my channel **HRTechVerse**.
> 🤝 Open to SOC Analyst opportunities in Canada.
