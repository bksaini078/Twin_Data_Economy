# Human Digital Twins for Market Research and Enterprise Decision Support

> **Doctoral Status Report & Research Summary**  
> **Last Updated:** August 22, 2026  
> **Target Completion:** Mid 2027  
> **Institution:** Fraunhofer IAO & Academic University Partner  

---

## 1. Research Metadata & Supervision

- **Doctoral Candidate:** Bhupender Kumar Saini (Fraunhofer IAO)
- **Primary Supervisors:**
  - **Prof. Dr. Katharina Hölzle** (Fraunhofer IAO / University Partner)
  - **Prof. Dr. Kai Arras** (Institute for Artificial Intelligence, Socially Intelligent Robotics Lab)
- **Co-Supervisors & Key Collaborators:**
  - **Prof. Dr. Matthias Peissner** (Fraunhofer IAO)
  - **Dr. Chandan Kumar** (Fraunhofer IAO)
  - **Leonie Isabel Gürtler** (Fraunhofer IAO)
  - **Daniel Auspurg** (Fraunhofer IAO)
- **Research Domains:** Human Digital Twins, Market Research Simulation, Simulation Fidelity & Bias Calibration, Platform Design, Behavioural Data Markets, Human-AI Interaction.

---

## 2. Executive Summary & Research Scope

Current market research and enterprise decision support rely on either costly, slow human panels or ungrounded LLM persona prompts that suffer from systematic distortion and hallucination.

This PhD thesis builds and validates **Human Digital Twins** — AI agents grounded in authentic personal behavioral data — as a viable, scalable, and consent-first alternative to traditional market research infrastructure. The work spans simulation design, fidelity measurement, platform engineering, and the economics of a user-owned data marketplace (Twinlytics).

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                  THREE CORE PILLARS                                  │
├──────────────────────────┬──────────────────────────┬──────────────────────────────┤
│  01. Simulation Design   │  02. Platform Validation  │  03. Data Economy            │
│  Designing & calibrating │  Empirically validating   │  A consented marketplace     │
│  LLM-based multi-agent   │  Twinlytics against       │  where users own twins and   │
│  simulation environments │  traditional panels.      │  earn yield from queries.    │
└──────────────────────────┴──────────────────────────┴──────────────────────────────┘
```

---

## 3. Published Research Baseline (7 Peer-Reviewed Publications)

| # | Paper Title | Venue / Format | Status & DOI | Core Contribution |
|---|---|---|---|---|
| 1 | **A Human-Centered Interaction Framework for Multi-agent AI Reasoning in Enterprise Decision-Making** | Springer Book Chapter (2026) | Published · `DOI: 10.1007/978-3-032-29586-6_28` | Multi-agent LLM reasoning framework for enterprise decision support. |
| 2 | **DUPLet: Dynamic User Modeling for Personalized Cover Letter Generation** | Extended Abstract · ACM UMAP 2026 | Published · `DOI: 10.1145/3774935.3812726` | Dynamic user state modeling & personal signal extraction. |
| 3 | **Virtual User Lab: An Interactive System for Simulating User Perspectives with AI Personas for Ideation and Evaluation** | Full Paper · ACM UMAP 2026 | Published · `DOI: 10.1145/3774935.3812731` | Interactive persona simulation lab for ideation and evaluation. |
| 4 | **Simulation of Human Survey Responses for Market Research: The Role of Contextualization in LLM-Based Agents** | Extended Abstract · ACM CHI 2026 | Published · `DOI: 10.1145/3772363.3798991` | Empirical evidence that LLM contextualization reduces survey response skew. |
| 5 | **Toward AI-Supported Decision Making in Innovation: Requirements and Design of LLM-Based Multi-Agent Systems** | Full Paper · IPDMC 2026 | Presented | Requirements engineering for LLM multi-agent decision support systems. |
| 6 | **Miscalibrated But Correctable: Bias in LLM-Based Digital Twin Demand Curves** | Full Paper · AMA Winter 2027 | **Submitted Aug 19, 2026** | Fidelity calibration: log-odds correction closes 57% of gap to human retest MAE benchmark. |
| 7 | **Personalizing POI Descriptions with LLMs: An Exploratory Study of User Perceptions** | Late Breaking Result · NordiCHI 2026 Adjunct | **Accepted** | First author (with C. Kumar, J. Blumenröther, M. Bâce). User perception study of LLM-generated personalized content — informs RQ1. |

---

## 4. Core Research Questions (RQ1 – RQ3)

### **RQ1: Simulation Design & Fidelity Calibration**

> *How can LLM-based multi-agent systems and AI persona simulation environments be designed to faithfully represent human perspectives in enterprise contexts, and what systematic response distortions and fidelity gaps emerge — and how can they be identified and mitigated — when such systems simulate human opinions, judgments, and behavioral decisions?*

- **Task 1 — System design & requirements:** Design principles for coherent LLM multi-agent collaboration and explainable reasoning in enterprise decision support (Papers 1, 5).
- **Task 2 — Simulation infrastructure:** Architecture and evaluation of an interactive virtual user lab deploying AI persona panels for ideation and product evaluation (Paper 3).
- **Task 3 — Distortion taxonomy:** Systematic identification of response skew, bias propagation, and contextualization effects; introduction of the Cross-Format Comparability Index (CFCI) (Papers 2, 4).
- **Task 4 — Fidelity calibration:** Measuring deviation between LLM-based digital twin responses and human retest benchmarks; evaluating correction strategies to restore predictive validity (Paper 6 — AMA Winter 2027 ✅).

### **RQ2: Platform Design & Evaluation**

> *What design requirements and evaluation criteria define a viable human digital twin platform for enterprise decision support, and how do stakeholder needs analysis, system architecture decisions, and deployment evidence inform platform design principles that move beyond conventional market research approaches?*

- **Task 1 — Requirements engineering:** Deriving design principles from published research and semi-structured stakeholder interviews (n=15–20) with enterprise innovation managers and market researchers (Papers 1, 5; P2).
- **Task 2 — Platform architecture:** Design, implementation, and deployment of Twinlytics — integrating twin memory engine, distortion calibration layer, and multi-agent simulation orchestration.
- **Task 3 — Deployment evaluation:** Empirical pilot comparing Twinlytics against traditional survey panels on speed, fidelity, usability, and insight quality (P2 — ECIS 2027 / ACM CHI 2027).

### **RQ3: Twin Data Economy**

> *What value creation architectures, consent mechanisms, and economic viability models characterize a user-owned digital twin data marketplace, and what enterprise use cases and ethical governance principles emerge from human-controlled AI simulation at scale?*

- **Task 1 — Use case taxonomy:** Formalizing enterprise and consumer applications for human digital twins — from reactive analytics to proactive AI-simulation-driven innovation pipelines (P3).
- **Task 2 — Economic architecture:** Designing consent-driven micro-licensing models, zero-knowledge data-sharing mechanisms, and direct user revenue payout structures (~10–20%) as a Fair-Trade Data paradigm (P3 — INFORMS Marketing Science 2027 / DESRIST 2027).
- **Task 3 — Viability & governance:** Assessing stakeholder value distribution, GDPR-compliant data sovereignty frameworks, and long-term market feasibility.

---

## 5. System Artifact: Twinlytics Platform Architecture

```
[ Stage 01: User Ingestion ]  ───►  [ Stage 02: Twin Memory Engine ]
   Client-side encrypted                 Dynamic state representation &
   reflective logs & choices             context retrieval pipelines
               │                                      │
               ▼                                      ▼
[ Stage 04: Analytics & Revenue ] ◄─── [ Stage 03: Simulation Orchestrator ]
   Direct ~10-20% revenue payout         Virtual User Lab executing multi-agent
   to users & enterprise reporting       survey panels with distortion calibration
```

1. **Stage 01 · User Signal Ingestion:** Personal reflective diary entries, survey history, and preference choices ingested and encrypted client-side.
2. **Stage 02 · Twin Memory Engine:** Vector embeddings and personal state modeling transform static logs into active, context-aware digital twin memory.
3. **Stage 03 · Simulation Orchestrator:** Multi-agent execution engine prompting and aggregating synthetic twin cohorts while applying distortion calibration.
4. **Stage 04 · Enterprise Analytics & Automated Payouts:** Statistical distributions, market signals, and direct revenue micro-payouts (~10–20%) back to participating user twins.

---

## 6. Planned Publications Roadmap (Papers 1–3)

```
┌──────────────────────────────┬──────────────────────────────┬──────────────────────────────┐
│ PAPER 1 (P1) ✅ SUBMITTED    │ PAPER 2 (P2)                 │ PAPER 3 (P3)                 │
│ Fidelity Calibration         │ Platform Eval & Requirements  │ Twin Economy & Use Cases     │
├──────────────────────────────┼──────────────────────────────┼──────────────────────────────┤
│ • Miscalibrated But          │ • 15–20 stakeholder           │ • Use case taxonomy          │
│   Correctable                │   interviews                  │ • Fair-Trade Data model      │
│ • AMA Winter 2027 ✅         │ • Pilot vs. traditional       │ • Consent & governance       │
│   Submitted Aug 19, 2026     │   panels                      │ • INFORMS Mktg Sci 2027      │
│                              │ • ECIS 2027 / CHI 2027        │   (Alt: DESRIST 2027)        │
│                              │   (Sub: Nov / Sep 2026)       │   (Sub: Jan 2027)            │
└──────────────────────────────┴──────────────────────────────┴──────────────────────────────┘
```

### **Paper 1: Miscalibrated But Correctable**
- **Status:** ✅ Submitted — AMA Winter Conference 2027 (Aug 19, 2026)
- **Focus:** Bias taxonomy in LLM-based digital twin demand curves; log-odds calibration closes 57% of gap to human retest MAE; introduces Cross-Format Comparability Index (CFCI).

### **Paper 2: Twinlytics Platform Design & Evaluation**
- **Status:** Planned — running in parallel with P3 (Q3–Q4 2026)
- **Primary Target:** ECIS 2027 (Luxembourg | **Deadline: Oct 30, 2026**)
- **Alternative:** ACM DIS 2027 (Deadline: Jan 18, 2027) / ACM UMAP 2027
- **Strategy:** Interviews-only submission for Oct 30 ECIS. Pilot study added in journal extension. Interviews must start immediately — 9 weeks to deadline.
- **Focus:** 15–20 semi-structured interviews with enterprise innovation managers and market researchers, producing validated design requirements for a human digital twin platform.

### **Paper 3: Twin Economy — Use Cases, Value Architecture & Governance**
- **Status:** Planned — **P3 completes BEFORE P2. Target draft: September 2026.**
- **Primary Target:** INFORMS Marketing Science 2027 (**Deadline: ~Jan 2027**)
- **Alternative:** DESRIST 2027 (best fit for the design science method used in P3; 2027 deadline not posted yet, likely near Jan 2027 based on the 2026 pattern) / PACIS 2027 (confirmed deadline March 1, 2027, safest fallback)
- **Step 0 (before writing):** Scopus + Web of Science gap search — 4 query strings, one afternoon, confirms novelty is clean before any writing begins.
- **Focus:** Design science study. Taxonomy (Nickerson et al.), maturity model (Becker et al., compared against Gartner/CMMI/NIST), Delphi expert validation (6–10 external experts), techno-economic model grounded in two-sided market theory (Rochet & Tirole), sensitivity analysis (10–20% revenue share), GDPR gap analysis (Articles 5, 7, 22, 25). Two theoretical claims: consent granularity and monetization are orthogonal dimensions; two-sided market theory extends to AI simulation markets.

---

## 7. PhD Execution Timeline (2026 – Mid 2027)

| Phase | Period | Key Tasks | Status |
|---|---|---|---|
| **Phase 0** | 2024–2026 | 5 foundational papers published across Springer, UMAP, CHI, IPDMC | ✅ Completed |
| **Phase 1** | Q3 2026 | P1 (Miscalibrated But Correctable) drafted and submitted to AMA Winter 2027 | ✅ Completed |
| **Phase 2** | Q3–Q4 2026 | Stakeholder interviews (n=15–20) for P2 — runs parallel to P3. Target: ECIS Oct 30, 2026 | 🔄 In Progress |
| **Phase 3** | Aug–Sep 2026 (draft) · Jan 2027 (submit) | P3 Twin Economy — desk research, taxonomy, maturity model, Delphi, economic model. **Completes before P2.** | 🔄 In Progress |
| **Phase 4** | Mid 2027 | Cumulative thesis collation, cross-study synthesis, oral defense | **Final Goal** |

---

## 8. Immediate Action Items

1. **P3 Gap Search (today):** Run Scopus + Web of Science search before writing P3. Query strings: "digital twin marketplace", "human digital twin consent monetization", "synthetic user platform pricing two-sided market", "fair data AI simulation". One afternoon — eliminates the biggest submission risk.
2. **Start P3 writing immediately:** Methodology is locked, no primary data needed. Target full draft September 2026. P3 completes before P2.
3. **Supervisor Meeting (this week):** Formally inform Prof. Hölzle of new title, locked RQs, 3-paper plan, and venue targets. Get approval before ECIS submission.
4. **P2 Interview Protocol (parallel):** Finalize semi-structured guide (n=15–20) and book first 5 interviews. ECIS deadline Oct 30 is 9 weeks away. Ethics clearance must start now if required.
5. **P2 Scope Decision (decide now):** Interviews-only for Oct 30 ECIS, or full pilot for Jan 2027 alternative. Cannot wait.
6. **P1 AMA Outcome:** Monitor review decision; prepare JMR / Marketing Science extension if accepted.
7. **RQ1 Thesis Chapter:** Write synthesis chapter using Papers 1–6. All material exists. Weeks of writing, no new empirical work.

### **Supervisory Committee Discussion Topics**
- Formal approval of revised thesis title and RQ framing.
- Stakeholder interview protocol review and ethics clearance timeline.
- P3 venue strategy: marketing science journal vs. IS conference.
- Differential privacy and data governance assumptions for P3.
