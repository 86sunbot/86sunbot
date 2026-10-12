# Surya — Cybersecurity Architect | Microsoft Sentinel & AI Agents | Technical Author

I design Azure and hybrid security architectures, engineer Microsoft Sentinel detections and log-assurance pipelines, and build AI agents governed by deterministic validation gates and human review. Alongside enterprise security delivery, I author CISSP and Microsoft security architecture study guides and maintain a separate algorithmic trading research practice.

**Start Here:** [**Engineering Portfolio & Technical Catalogue (`86sunbot/portfolio`) →**](https://github.com/86sunbot/portfolio)

---

## Three Public Flagship Examples (Inspect Source & Run Locally)

### 1. Azure & Enterprise AI/DR Security Architecture
- **Problem:** CISOs and cloud architects need concrete control-plane designs comparing enterprise AI/Detection & Response ecosystems and enforcing API authentication and rate-limiting boundaries on internal RAG services.
- **Contribution:** Authored the **491-line Microsoft Security vs. CrowdStrike Falcon Enterprise AI/DR Architecture Comparison** (7 Mermaid diagrams, 4 attack scenarios, 20-item checklist) and engineered the **`v3-enterprise-assistant` FastAPI security boundary** (`secrets.compare_digest` `X-API-Key` auth, sliding-window rate limiter, non-root Docker isolation, and `ADR-001`..`ADR-006`).
- **Evidence & Access:** **Public source and demo instructions** ([AI/DR Architecture Guide](https://github.com/86sunbot/fde-lab/blob/main/microsoft_vs_crowdstrike_ai_dr_guide.md) · [`v3-enterprise-assistant/app/security.py`](https://github.com/86sunbot/fde-lab/blob/main/document-assistant/versions/v3-enterprise-assistant/app/security.py), `32 passed` `pytest` tests); **public case study with implementation currently private** ([`azure-security-framework`](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md)).

### 2. Microsoft Sentinel Detection Engineering & Two-Layer KQL Validation
- **Problem:** SIEM teams face noisy or broken KQL rules, missing entity mappings, and silent log drop-offs when deploying detections without structural and semantic validation.
- **Contribution:** Built a **Scheduled `SigninLogs` password-spray detection rule** (`DetectionWindow = 15m`, `dcount(UserPrincipalName) >= 10`, `IP` & `Account` entity mappings) and a **two-layer KQL validator** (`structural.py`, `detection.py`) enforcing `enabled = False`, blocking destructive KQL operators, and verifying threshold agreement, alongside multi-rule ATT&CK v14 and 3-way log-reconciliation frameworks.
- **Evidence & Access:** **Public source and demo instructions** ([`reference_proposer.py`](https://github.com/86sunbot/fde-lab/blob/main/sentinel-usecase-deployment/src/sentinel_usecase/agent/reference_proposer.py) · [`structural.py`](https://github.com/86sunbot/fde-lab/blob/main/sentinel-usecase-deployment/src/sentinel_usecase/validation/structural.py), `28 passed` `pytest` tests); **public case studies with implementations currently private** ([Sentinel Detections, Log Assurance & Greenfield IaC](https://github.com/86sunbot/portfolio/blob/main/sentinel.md)).

### 3. AI Agents for Security Operations & Regulated Workflows
- **Problem:** Allowing LLMs to directly execute SIEM changes or clinical/manufacturing workflow transitions introduces ungoverned drift and fail-open safety risks.
- **Contribution:** Engineered a **governed Sentinel rule-generation workflow** (`workflow.py`, `gateway.py`) that isolates the LLM from tool execution, runs single-pass validation repair, requires human `ApprovalDecision.APPROVE`, and re-validates `enabled = False` before deployment, plus a **fail-closed CGT orchestration console** (`FDE-Final-Capstone`) and **pre-GxP clinical report triage prototype** (`caldera-monitoring-triage`).
- **Evidence & Access:** **Public source and demo instructions** ([`fde-lab/sentinel-usecase-deployment`](https://github.com/86sunbot/fde-lab/tree/main/sentinel-usecase-deployment) [`28` tests] · [`FDE-Final-Capstone`](https://github.com/86sunbot/FDE-Final-Capstone) [`118` tests] · [`caldera-monitoring-triage`](https://github.com/86sunbot/caldera-monitoring-triage) [`9` tests on `main`]); **private V3.4 case study** ([`ai-agents.md`](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md)).

---

## Portfolio Navigation & Supporting Practice Areas

1. [**Security Architecture**](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md) — Public AI/DR comparison, RAG security boundary, and Azure CAF / Zero Trust designs.
2. [**Microsoft Sentinel**](https://github.com/86sunbot/portfolio/blob/main/sentinel.md) — Public `SigninLogs` KQL rule & validator, plus log assurance, Terraform/PowerShell IaC, and Logic App SOAR case studies.
3. [**AI Agents & Applied Engineering**](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md) — Governed Sentinel agent workflow, CGT Control Tower, clinical triage prototype, and LLM/RAG threat models.
4. [**Technical Authorship & Study Guides**](https://github.com/86sunbot/portfolio/blob/main/books-and-learning.md) — Includes a **public cross-domain sample lesson** (*CISSP → Entra ID `SC-100`/`SC-500` → Sentinel KQL*), public [LinkedIn Sentinel architecture article](https://www.linkedin.com/feed/update/urn:li:activity:7434462569752571904/), and verified chapter outlines for four unpublished local manuscripts (*MS Security Architect Blueprint v1.1*, *SC-500 Guide v1.1*, *Surya Master CISSP Guide*, *AI-901 Guides*).

### Separate Personal Research Practice
5. [**Algorithmic Trading Research**](https://github.com/86sunbot/portfolio/blob/main/trading-research.md) — Independent quantitative research practice featuring a pure-Python CPR + Wilder RSI backtesting prototype.

---

## Credentials & Contact

- **CISSP (ISC2):** [Verified Credly Badge (Valid 2026–2029)](https://www.credly.com/badges/5c478c9e-77f0-4227-9251-69ecb1d639e5)
- **Contact:** [Experience & Impact](https://github.com/86sunbot/portfolio/blob/main/experience-and-impact.md) · [LinkedIn](https://www.linkedin.com/in/surya-ps-cissp-a5a097160/) · Bengaluru, India
