# Surya — Cybersecurity Architect | Microsoft Sentinel & AI Agents | Technical Author

I design Azure and hybrid security architectures, engineer Microsoft Sentinel detections and log-assurance pipelines, and build AI agents governed by deterministic validation gates and human review. Alongside enterprise security architecture delivery, I author CISSP and Microsoft certification study guides and maintain a separate algorithmic trading research practice.

---

## Featured Examples

### 1. Microsoft Sentinel Detection Engineering & Log Assurance
- **Problem:** SIEM teams face silent log drop-offs, unassociated Data Collection Rules (DCRs), and error-prone translation of threat requirements into KQL rules.
- **Contribution:** Built the **AI-Assisted Sentinel Detection Engineering Agent (V3.4)** and **Sentinel Log Validation Agent** to ground candidate KQL against workspace schemas, reconcile assets against DCRs and heartbeats, verify pipelines with synthetic canaries, and enforce human-gated `enabled=false` deployment.
- **Result:** Runnable CLI/FastAPI validation workbenches and MITRE ATT&CK v14 KQL rules for MFA fatigue (`T1621`), impossible travel (`T1078`), pass-the-hash (`T1550.002`), and privileged role assignment (`T1098.003`).
- **Evidence:** [Sentinel Detections & Assurance](https://github.com/86sunbot/portfolio/blob/main/sentinel.md) · [AI Detection Agent V3.4](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md#1-ai-assisted-microsoft-sentinel-detection-engineering-agent-ai-agent-usecase-deployment-v34)

### 2. Cell & Gene Therapy (CGT) Patient-to-Batch Orchestration
- **Problem:** A brownfield orchestration baseline had fail-open exceptions, single-timestamp overwrites on out-of-order lab events, and unauthenticated role elevation.
- **Contribution:** Engineered a Python orchestration engine (`src/fde_capstone/`), FastAPI service, and browser console with three-state gate evaluation (`satisfied` / `not-satisfied` / `unknown`), bitemporal history, opaque bearer-token mutation auth mapped to server-side RBAC roles/scopes, and a SHA-256 hash-chained SQLite audit log.
- **Result:** Runnable Control Tower demo (`START_DEMO.command`) with three synthetic POCs, disruption previews, and seven read-only persona lenses.
- **Evidence:** [Public Repository & Runnable Demo (`FDE-Final-Capstone`)](https://github.com/86sunbot/FDE-Final-Capstone)

### 3. Azure Zero Trust Architecture & Enterprise AI/DR Benchmark
- **Problem:** Cloud architects need implementation-level designs connecting Entra ID Conditional Access, Hub-Spoke segmentation, Private Link DNS, encryption hierarchies, and SIEM/XDR trade-offs.
- **Contribution:** Authored the **Azure Security Architecture Framework** and the **Microsoft Security vs. CrowdStrike Falcon Enterprise AI/DR Benchmark**.
- **Result:** Conditional Access matrices, Hub-Spoke/Private Link topologies, PMK/CMK/CPK patterns, HLD/ADR templates, and comparative SIEM/XDR guidance.
- **Evidence:** [Security Architecture](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md) · [Public AI/DR Benchmark](https://github.com/86sunbot/fde-lab/blob/main/microsoft_vs_crowdstrike_ai_dr_guide.md)

---

## Portfolio Categories

1. [**Security Architecture**](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md) — Azure CAF landing zones, Conditional Access, Hub-Spoke topologies, encryption, and HLD/ADR templates.
2. [**Microsoft Sentinel**](https://github.com/86sunbot/portfolio/blob/main/sentinel.md) — KQL detections, log assurance, PowerShell/ARM orchestrator, and Logic App SOAR playbooks.
3. [**AI Agents & Applied Engineering**](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md) — Sentinel detection agent, CGT capstone, clinical triage prototype, and LLM/RAG threat models.
4. [**Books & Learning**](https://github.com/86sunbot/portfolio/blob/main/books-and-learning.md) — Unpublished self-authored manuscripts, mindmaps, lab runbooks, and `cissp-knowledge-base`.
5. [**Algorithmic Trading Research**](https://github.com/86sunbot/portfolio/blob/main/trading-research.md) — Separate personal research with an October 2026 Python backtest prototype.

---

## Books

Unpublished self-authored manuscripts and articles ([details & previews](https://github.com/86sunbot/portfolio/blob/main/books-and-learning.md)):
- ***Microsoft Security Architect Blueprint (v1.1)*** & ***SC-500 Guide (v1.1)*** ([Cover](https://github.com/86sunbot/portfolio/blob/main/media/sc500-study-guide-v1.1-cover.png) · [TOC](https://github.com/86sunbot/portfolio/blob/main/media/sc500-study-guide-v1.1-toc.png))
- ***Surya Master CISSP Guide*** ([Mindmap](https://github.com/86sunbot/portfolio/blob/main/media/cissp-eight-domain-mindmap-overview.png)) · ***AI-901 Guides*** · [***How NOT to Design Microsoft Sentinel***](https://www.linkedin.com/feed/update/urn:li:activity:7434462569752571904/)

---

## Credentials & Contact

- **CISSP (ISC2):** [Verified Credly Badge (2026–2029)](https://www.credly.com/badges/5c478c9e-77f0-4227-9251-69ecb1d639e5)
- **Contact:** [Career Summary](https://github.com/86sunbot/portfolio/blob/main/experience-and-impact.md) · [LinkedIn](https://www.linkedin.com/in/surya-ps-cissp-a5a097160/) · Bengaluru, India
