# Day 00 — Introduction & 30-Day Roadmap

> **Challenge:** [30 Days SOC Analyst Challenge](https://www.youtube.com/@MyDFIR) by Steven (MyDFIR)
> **Status:** ✅ Started | **Goal:** Build a full hands-on Security Operations Center home lab from scratch.

---

## 🎯 Why This Challenge

The 30 Days SOC Analyst Challenge exists to fix the single biggest gap for entry-level SOC candidates: **a lack of real, hands-on practical experience.**

> *"Certifications and theory are good, but you need to learn how to apply that."* — Steven (MyDFIR)

Certs and theory build a foundation. But employers hire analysts who can **apply** that knowledge — ingest logs, write detections, investigate alerts, and document findings. This challenge produces exactly that, one task per day, for 30 days.

---

## 🧠 What I Will Be Able To Do By Day 30

- Design and draw a **logical network diagram** for a SOC environment
- Stand up and configure my own **Elasticsearch + Kibana** instance
- Ingest endpoint logs — including **Sysmon** — from Windows hosts
- Simulate, detect, and investigate **malware** and **SSH/RDP brute-force** activity
- Build **detection alerts and dashboards** in Kibana
- Stand up a **Command & Control (C2)** server and detect its activity
- Integrate a **ticketing system** and run end-to-end investigations

---

## 🔄 The SOC Analyst Workflow This Lab Recreates

```
Collect Logs → Parse & Normalize → Detect & Alert → Triage → Investigate → Ticket & Respond
```

Every task in the challenge maps to a stage of the real-world detection-and-response pipeline an analyst lives in daily.

---

## 🗺️ The 4-Week Roadmap

| Week | Theme | What Gets Built |
|------|-------|-----------------|
| **Week 1** | Foundation | Intro to the ELK stack → set up Elasticsearch + Kibana → ingest endpoint logs incl. **Sysmon** |
| **Week 2** | Detection | Stand up a public **SSH + RDP** server → build **alerts & dashboards** for brute-force activity |
| **Week 3** | Adversary Simulation | Spin up a **C2 server with Mythic** → attack the public servers, detect beaconing |
| **Week 4** | Response | Integrate a **ticketing system** → run full investigations from alert to closed case |

---

## 🧰 Key Tools & Concepts

### The ELK Stack
- **Elasticsearch** — search & analytics engine that stores and indexes all log data
- **Kibana** — visualization layer where dashboards, alerts, and detection rules are built
- **Logstash / Agents** — collect, parse, and ship logs from endpoints into Elasticsearch

### Endpoint Telemetry
- **Sysmon (System Monitor)** — Windows tool that logs process creation, network connections, and file/registry changes in rich detail. This high-fidelity data makes attacker behaviour *visible* and maps cleanly to MITRE ATT&CK.

### Adversary Behaviour → MITRE ATT&CK

| Activity in the Lab | ATT&CK Reference | What the Analyst Looks For |
|---------------------|------------------|----------------------------|
| SSH / RDP Brute Force | `T1110` Brute Force | Spikes of failed logins from one source, then a success |
| RDP Remote Access | `T1021.001` Remote Services: RDP | Unexpected inbound RDP sessions, lateral movement |
| Command & Control (Mythic) | `TA0011` Command & Control | Beaconing patterns, unusual outbound connections |
| Malware Execution | `T1204` User Execution | Suspicious process trees, child-process spawning in Sysmon |

---

## 🏗️ Lab Infrastructure

The challenge runs **in the cloud** because the full stack (ELK + endpoints + attack servers) is resource-intensive.

- **Recommended:** Vultr (via free starter credit)
- **Also valid:** Any cloud that can spin up a Windows VM (Azure, AWS, GCP)
- **On-prem option:** VirtualBox / VMware for anyone with the hardware

> 💡 Shut down VMs when idle to preserve cloud credit.

---

## ✅ Day 0 Action Checklist

- [ ] Choose the build path: cloud provider or on-prem virtualization
- [ ] Create the cloud account and claim starter credit
- [ ] Sketch the **logical network diagram** (ELK server + Windows endpoint + public attack server)
- [ ] Confirm budget guardrails (shut down idle VMs)
- [x] Set up this repository to track notes, diagrams, and evidence
- [ ] Commit publicly every day — accountability is the point

---

## 💭 My Takeaway

This is where the talk-vs-action line gets drawn. Anyone can list a tool on a resume; far fewer can say *"I built the pipeline, generated the attack, wrote the detection, and investigated the alert."* Over the next 30 days, that is exactly what this lab will produce — and every step lands in this repo as documented, defensible evidence.

---

*Part of **Harshkumar Raval's** SOC Analyst portfolio — [HRTechVerse](https://www.youtube.com/).*
*"I think like an attacker to defend like a professional. Calm mind, relentless hunt."*
