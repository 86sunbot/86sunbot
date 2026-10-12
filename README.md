# Surya — Cybersecurity Architect | Microsoft Sentinel & AI Agents | Technical Author

I design Azure and hybrid security architectures, engineer Microsoft Sentinel detections and log-assurance pipelines, and build AI agents governed by deterministic validation gates and human review. Alongside enterprise security delivery, I author CISSP and Microsoft security architecture study guides and maintain a separate algorithmic trading research practice.

**Start Here:** [**Engineering Portfolio & Technical Catalogue (`86sunbot/portfolio`) →**](https://github.com/86sunbot/portfolio)

---

## Three Public Flagship Examples (Inspect Source & Run Locally)

### 1. Azure & Enterprise AI/DR Security Architecture
- **Problem:** Architects need control-plane designs comparing enterprise AI/DR ecosystems and enforcing API auth and rate-limiting boundaries on RAG services.
- **Contribution:** Authored a **491-line Microsoft vs. CrowdStrike Enterprise AI/DR Architecture Comparison** (8 Mermaid diagrams, 4 attack scenarios, 20-item checklist) and built the **`v3-enterprise-assistant` FastAPI security boundary** (`secrets.compare_digest` `Bearer` API-key auth, SHA-256 client-ID hashing, `InMemoryRateLimiter`, non-root Docker, `ADR-001`..`ADR-006`).
- **Evidence & Access:** **Public source and demo instructions** ([AI/DR Guide](https://github.com/86sunbot/fde-lab/blob/main/microsoft_vs_crowdstrike_ai_dr_guide.md) · [`app/security.py`](https://github.com/86sunbot/fde-lab/blob/main/document-assistant/versions/v3-enterprise-assistant/app/security.py), `32 passed` `pytest` tests); **private implementation case study** ([`azure-security-framework`](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md)).

### 2. Microsoft Sentinel Detection Engineering & Two-Layer KQL Validation
- **Problem:** SIEM teams face noisy or broken KQL rules, missing entity mappings, and silent log drop-offs when deploying detections without validation.
- **Contribution:** Built a **Scheduled `SigninLogs` password-spray detection rule** (`DetectionWindow = 15m`, `dcount(UserPrincipalName) >= 10`, `IP` & `Account` entities) and a **two-layer KQL validator** (`structural.py`, `detection.py`) enforcing `enabled = False`, blocking destructive KQL commands, and checking threshold agreement.
- **Evidence & Access:** **Public source and demo instructions** ([`reference_proposer.py`](https://github.com/86sunbot/fde-lab/blob/main/sentinel-usecase-deployment/src/sentinel_usecase/agent/reference_proposer.py) · [`structural.py`](https://github.com/86sunbot/fde-lab/blob/main/sentinel-usecase-deployment/src/sentinel_usecase/validation/structural.py), `28 passed` `pytest` tests); **private implementation case studies** ([Sentinel Detections, Log Assurance & IaC](https://github.com/86sunbot/portfolio/blob/main/sentinel.md)).

### 3. AI Agents for Security Operations & Regulated Workflows
- **Problem:** Allowing LLMs to directly execute SIEM changes or regulated workflow transitions introduces drift and fail-open risks.
- **Contribution:** Engineered a **governed Sentinel rule-generation workflow** (`workflow.py`, `gateway.py`) isolating the LLM from execution, running single-pass repair, requiring `ApprovalDecision.APPROVE`, and enforcing `enabled = False`, plus a **fail-closed CGT console** (`FDE-Final-Capstone`) and **pre-GxP clinical triage prototype** (`caldera-monitoring-triage`).
- **Evidence & Access:** **Public source and demo instructions** ([`sentinel-usecase-deployment`](https://github.com/86sunbot/fde-lab/tree/main/sentinel-usecase-deployment) [`28` tests] · [`FDE-Final-Capstone`](https://github.com/86sunbot/FDE-Final-Capstone) [`118` tests] · [`caldera-monitoring-triage`](https://github.com/86sunbot/caldera-monitoring-triage) [`9` tests on `main`]); **private V3.4 case study** ([`ai-agents.md`](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md)).

---

## Portfolio Navigation & Practice Areas

1. [**Security Architecture**](https://github.com/86sunbot/portfolio/blob/main/security-architecture.md) — Public AI/DR comparison, RAG security boundary, and Azure CAF / Zero Trust designs.
2. [**Microsoft Sentinel**](https://github.com/86sunbot/portfolio/blob/main/sentinel.md) — Public `SigninLogs` KQL rule & validator, plus log assurance, Terraform/PowerShell IaC, and SOAR case studies.
3. [**AI Agents & Applied Engineering**](https://github.com/86sunbot/portfolio/blob/main/ai-agents.md) — Governed Sentinel agent, CGT Control Tower, clinical triage prototype, and LLM/RAG threat models.
4. [**Books & Technical Learning**](https://github.com/86sunbot/portfolio/blob/main/books-and-learning.md) — Original **public cross-domain sample lesson** (*CISSP → Entra ID `SC-100`/`SC-500` → Sentinel KQL*), [LinkedIn Sentinel article](https://www.linkedin.com/feed/update/urn:li:activity:7434462569752571904/), and outlines for four unpublished manuscripts (*MS Security Architect v1.1*, *SC-500 v1.1*, *CISSP Guide*, *AI-901*).
5. [**Algorithmic Trading Research (Separate Practice)**](https://github.com/86sunbot/portfolio/blob/main/trading-research.md) — Independent quantitative research featuring a Python CPR + Wilder RSI backtesting prototype.

---

## Credentials & Contact

- **CISSP (ISC2):** [Verified Credly Badge (2026–2029)](https://www.credly.com/badges/5c478c9e-77f0-4227-9251-69ecb1d639e5) · **Contact:** [Experience & Impact](https://github.com/86sunbot/portfolio/blob/main/experience-and-impact.md) · [LinkedIn](https://www.linkedin.com/in/surya-ps-cissp-a5a097160/) · Bengaluru, India

