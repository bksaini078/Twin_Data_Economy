# P3 Study Plan and Methodology — Version 2

## The Twin Economy: Use Cases, Value Architecture, and Governance of a Human Digital Twin Data Marketplace

**Target:** Draft complete September 2026. Submission to INFORMS Marketing Science 2027 (primary, deadline near Jan 2027). Alternatives: DESRIST 2027 (best fit for the design science method, exact 2027 deadline not posted yet) or PACIS 2027 (confirmed deadline March 1, 2027). P3 runs in parallel with P2 stakeholder interviews.

---

## 0. Before writing begins: literature gap search

Before a single section of the paper is written, run a focused literature gap search on Scopus and Web of Science to confirm the novelty claim is still clean. This is one afternoon of work and it eliminates a serious submission risk. A paper close to this one already existing and going undetected is the most damaging outcome possible at review stage.

Search the following four combined query strings:

1. "digital twin marketplace" AND ("data economy" OR "personal data")
2. "human digital twin" AND ("consent" OR "monetization" OR "revenue sharing")
3. "synthetic user" AND ("platform pricing" OR "two-sided market" OR "data cooperative")
4. "fair data" AND ("AI simulation" OR "digital twin" OR "LLM persona")

Check results in both Scopus and Web of Science. Read any paper that sounds relevant. If a paper close to this one exists, identify what it does not do (the gap it leaves) and update the positioning in section 2 of this plan accordingly. If nothing close exists, proceed to section 1.

Do this before drafting begins. Not after.

---

## 1. What this paper answers

This paper answers RQ3 of the thesis.

RQ3: What value creation architectures, consent mechanisms, and economic viability models characterize a user-owned digital twin data marketplace, and what enterprise use cases and ethical governance principles emerge from human-controlled AI simulation at scale?

The paper has three parts, matching the three tasks already set under RQ3.

Task 1. Build a use case taxonomy for human digital twins in enterprise and consumer contexts.

Task 2. Design the economic architecture, meaning the revenue model, consent mechanism, and pricing logic.

Task 3. Assess viability and governance, meaning whether the model actually works financially and whether it respects data protection rules.

---

## 2. Why this paper is needed

I checked the existing literature before designing this study. Four things stood out.

The data cooperative literature is theoretical. The main recent paper in this space is a conceptual review. It compares governance models on paper but never tests one. It openly says the open question is how to design fair incentive structures, and it does not answer that question with real data.

The personal data valuation literature does not cover AI agents. The main paper here, by Spiekermann and Korunovska, studies what people think their data is worth, but has no discussion anywhere of AI agents, automated systems, or digital twins. That field was built before this technology existed.

The two-sided data platform literature is analytical, not tested. There are solid papers modeling how such platforms should price themselves, but they are built on theory and mathematics, not on real use cases or real numbers.

The human digital twin governance literature stops at naming the problem. Recent papers map out the risks around consent and monetization in detail, but do not propose or test a working model. One paper calls directly for empirical work on whether governance mechanisms for these systems actually function.

So the gap is clear. Nobody has built and tested a concrete use case taxonomy and economic model for a human digital twin marketplace. This paper does that, using Twinlytics as the real platform behind the analysis, instead of a hypothetical one.

---

## 3. Theoretical contribution

Beyond the practical outputs, this paper makes two theoretical claims that the empirical work tests.

First, in a human digital twin marketplace, consent structure and monetization mechanism are orthogonal dimensions. That is, a platform can offer high consent granularity with low revenue share, or low consent granularity with high revenue share. These two dimensions vary independently rather than trading off against each other, as existing theory on personal data markets tends to assume. The taxonomy tests whether this orthogonality holds across real platforms.

Second, the pricing logic of a human digital twin marketplace follows two-sided market theory (Rochet and Tirole, 2003; Parker and Van Alstyne, 2005), where the platform subsidizes data contributors on one side and charges enterprise buyers on the other. The economic model tests whether this logic produces a financially viable equilibrium under realistic assumptions about adoption and revenue share. If it does, this provides the first empirically grounded confirmation that two-sided market theory extends to AI simulation markets, not only to content platforms and payment networks where the theory was originally developed.

These two theoretical claims give the paper a contribution that goes beyond describing Twinlytics, and they are falsifiable.

---

## 4. Overall approach

This study is framed as design science research, following the method from Peffers and colleagues. This is the standard way information systems research builds and evaluates a working artifact, and it fits this paper naturally because Twinlytics is a real, working artifact, not a hypothetical concept.

The method has six steps. Problem identification, defining what a solution needs to do, designing the solution, demonstrating it, evaluating it, and communicating the result. Below is how each step of this paper maps onto that structure.

Problem identification: the four gaps described in section 2, plus the two theoretical claims in section 3 that existing work cannot test because no working platform existed before Twinlytics.

Objectives for a solution: a validated use case taxonomy, a workable economic model, and a governance assessment, as set out in RQ3.

Design: the taxonomy and the maturity model, described in sections 5 and 6 below.

Demonstration: a case study run on Twinlytics itself, described in section 8.

Evaluation: expert review of the taxonomy and model via Delphi, plus the economic modeling with sensitivity testing, described in sections 7 and 8.

Communication: the paper itself.

---

## 5. Building the use case taxonomy

This is Task 1. The method used here is the taxonomy development method from Nickerson, Varshney, and Muntermann, a well established and widely cited method in information systems research.

**Step 1, set the meta-characteristic.** Before collecting any use cases, one central idea is defined that every use case and every category must trace back to. For this paper, the meta-characteristic is the value exchange configuration between the person contributing personal data through their digital twin and the enterprise consuming that data. Every dimension in the taxonomy has to relate back to this idea. The dimensions expected to emerge include consent granularity, data ownership structure, monetization mechanism, simulation scope, and enterprise decision context. Pre-specifying these expected dimensions keeps the taxonomy grounded in theory rather than driven by whatever happened to be prominent in one platform.

**Step 2, gather real cases.** Use cases are pulled from real, existing systems. This includes Twinlytics itself, and known competitors and comparable platforms such as Simile AI, Listen Labs, Aaru, and Synthetic Users. It also includes the use cases already described in the Twinlytics white paper, and any relevant cases mentioned in the published literature. The target is a minimum of twenty distinct use cases across platforms before the first taxonomy round begins.

**Step 3, coding protocol.** Each use case is coded independently by two researchers, meaning the doctoral candidate and one co-supervisor with relevant expertise. Coding assigns each use case to an initial category based on the meta-characteristic and the expected dimensions from Step 1. After independent coding, agreement is measured using Cohen's kappa. A kappa above 0.7 is treated as sufficient agreement. Cases where the two coders disagree are discussed until a shared interpretation is reached, and the disagreement is documented as a note on boundary cases.

**Step 4, build the taxonomy through repeated rounds, working in both directions.** One direction is empirical to conceptual, meaning categories are built up from patterns found in the real cases gathered in Step 2. The other direction is conceptual to empirical, meaning categories are first proposed from the theory found in the literature review, then checked against the real cases to see if they hold up. Both directions are used across several rounds, and each round refines the categories.

**Step 5, stop only when clear conditions are met.** The taxonomy is not considered finished just because it feels complete. It stops when all of the following are true: no new categories emerge in the last round, every category has at least one real example behind it, no two categories overlap, and the taxonomy is judged concise enough to be useful and detailed enough to be meaningful.

The result of this phase is a structured taxonomy of human digital twin use cases, grouped into a small number of clear categories, each backed by real examples and verified by two independent coders.

---

## 6. Building the maturity model

This connects the taxonomy to a staged view of how mature a human digital twin deployment is. The primary dimension from the taxonomy that maps onto maturity is consent granularity combined with data sovereignty level. This choice is deliberate. Higher maturity in a human digital twin deployment is not primarily a technical question of capability, it is a governance question of how much control the data contributor retains and how well the platform enforces that control. This makes consent and sovereignty the natural axis along which maturity progresses, from the simplest form at Stage 1 to the most autonomous form at Stage 5.

The method used here is the maturity model procedure from Becker, Knackstedt, and Pöppelreuter. It has the following phases.

Define the problem and the scope of the model. In this case, the scope is human digital twins used for market research and enterprise decision support, not digital twins in general.

Compare the proposed model against existing models. Three existing models are directly relevant and will be compared. The Gartner AI Maturity Model assesses organizational readiness for AI but does not address data ownership or consent. The CMMI Data Management Maturity model addresses governance but was built for enterprise data assets, not personal data held by individual contributors. The NIST Privacy Framework maturity model addresses data protection but does not address the economic dimension of data markets. None of the three covers the combination of consent, economic value sharing, and simulation fidelity that defines a human digital twin deployment. This gap justifies the proposed model.

Decide how the model will be developed. This paper builds it iteratively, moving between the taxonomy from section 5 and expert feedback from section 7, rather than writing it in one pass.

Build the model iteratively, defining each stage clearly, from Stage 1 (an ungrounded LLM persona with no consent structure and no revenue sharing) through Stage 5 (a fully consented, autonomously responding, revenue-sharing twin with verifiable simulation fidelity and GDPR-compliant data sovereignty).

Plan how the model will be evaluated and used. This paper evaluates it through the expert panel described in section 7, and demonstrates it through the case study in section 8.

Document the model clearly enough that someone outside the research team could apply it to a new platform or deployment context.

Evaluate the model against real feedback and decide whether it needs further refinement or is ready to publish.

---

## 7. Expert validation

This is where the taxonomy and the maturity model get checked against real expertise, rather than only against the researcher's own judgment.

The method is a two round Delphi study, a well established method for building structured consensus among a small group of experts.

**Panel composition.** Six to ten experts. Independence is the key criterion for panel selection. The supervision team and Twinlytics collaborators review the instruments before the panel begins, but they do not sit on the Delphi panel itself because they are invested in the outcome. The Delphi panel is composed predominantly of external experts, meaning at minimum four of the six to ten panel members have no involvement in the research or in Twinlytics. Selection criteria for external experts: demonstrated expertise in at least one of the following areas, data economy or personal data market design, market research methodology, platform governance, or enterprise AI adoption. Recruitment will target practitioners and academics from ESOMAR (market research professional association), the Data Stewardship Alliance, and relevant IS and marketing faculty at other institutions.

**Consensus threshold.** Agreement is defined as 70 percent or more of panelists rating a category or stage as correctly placed, on a five-point scale where the top two positions count as agreement. If a category or stage falls below this threshold in Round 2, it is flagged as contested and either revised or removed with documented reasoning.

**Round one.** The draft taxonomy and maturity model are shared with the panel, along with the base assumptions of the economic model (price per query range, revenue share range, adoption rate assumptions). Each expert rates and comments on the taxonomy categories, the use cases within them, the stage definitions, and the economic assumptions, flagging anything unclear, missing, or wrongly placed.

**Round two.** The taxonomy, maturity model, and revised economic assumptions are sent back to the same panel with a summary of how the group responded the first time. Experts are asked whether they agree with the revised version, and disagreements are discussed until the group reaches a position at or above the consensus threshold.

By including the economic model assumptions in Round 1, the expert panel serves double duty: it validates the taxonomy and maturity model, and it also provides a documented expert check on whether the economic assumptions are plausible, without requiring a separate data collection step.

---

## 8. Economic modeling and case demonstration

This is Task 2 and Task 3 together, the economic architecture and the viability assessment.

**Theoretical grounding.** The economic model is structured using two-sided market theory (Rochet and Tirole, 2003; Parker and Van Alstyne, 2005). In this framework, Twinlytics is a two-sided platform connecting data contributors on one side and enterprise buyers on the other. Platform theory predicts that the optimal strategy is to subsidize the contributor side (lower prices, revenue sharing) to build supply, while charging a higher price to the enterprise buyer side, which values the insight produced. This is precisely the 10 to 20 percent revenue share model that Twinlytics proposes. By grounding the model in this theory, the paper connects the practical economic architecture to a body of established pricing literature, rather than presenting it as an ad hoc design choice.

**Economic modeling.** For each use case identified in the taxonomy, a techno-economic model estimates the potential value created and captured. This uses real market data such as vendor pricing, typical enterprise research spend, and comparable platform pricing, drawn from the Twinlytics white paper, published desk research, and industry sources such as ESOMAR's annual market research spend report and published pricing from Synthetic Users and Listen Labs.

Unlike a single point estimate, this paper adds a sensitivity analysis. Instead of reporting one return on investment number per use case, the model is run across a range of assumptions, varying the revenue share paid to data contributors between 10 and 20 percent, the price charged per query, and the expected adoption rate. This shows a realistic range of outcomes rather than one number that depends entirely on unverifiable assumptions.

**Governance assessment.** Task 3 requires assessing whether the model respects data protection rules. This is done through a structured mapping exercise. The proposed consent mechanism and revenue sharing architecture are mapped against the key GDPR obligations: Article 5 (data minimization and purpose limitation), Article 7 (conditions for consent), Article 22 (rights related to automated decision-making), and Article 25 (data protection by design). For each article, the mapping identifies whether the current Twinlytics design satisfies the obligation, partially satisfies it, or leaves a gap, and what design change would close the gap. This is a desk-based analysis using publicly available GDPR guidance and existing Twinlytics technical documentation.

**Case demonstration.** The taxonomy and maturity model are then demonstrated against a real case using Twinlytics itself. This follows the case study logic set out by Yin, where a single case is justified because it is the only fully built platform of its kind available to the research, not because it was picked at random. The demonstration walks through one concrete scenario end to end: an enterprise requests market research insight on product feature preferences from a cohort of digital twins. The demonstration shows which taxonomy category this use case falls into, what stage of the maturity model the Twinlytics deployment currently sits at for this scenario, what the economic model estimates the platform would earn and the contributor would receive per query, and what governance changes would be needed to move the platform to the next maturity stage.

This end-to-end walkthrough is what turns the taxonomy and model from a purely conceptual exercise into something tested against a working system.

---

## 9. What ties the whole paper together

Each phase feeds the next one directly.

The taxonomy from section 5 defines what the use cases actually are, and identifies consent granularity and data sovereignty as the primary maturity dimension.

The maturity model from section 6 uses that primary dimension to build a five-stage progression, anchored in a comparison against three existing models that do not cover this combination of governance and economic value sharing.

The expert panel in section 7 checks that both the taxonomy and the maturity model hold up against outside judgment, and simultaneously validates the economic model assumptions, removing the need for a separate validation step.

The economic modeling in section 8 is grounded in two-sided market theory, tested against real market data, and stress-tested through sensitivity analysis across the key assumptions.

The governance assessment in section 8 applies a structured GDPR mapping rather than a general discussion, giving the paper a specific, actionable output rather than a list of principles.

The case demonstration in section 8 walks one complete scenario through all four components, from taxonomy to maturity stage to economic estimate to governance gap.

Together, this directly answers all three tasks under RQ3, using one coherent research design instead of three separate, disconnected pieces of work.

---

## 10. Why this design is defensible

Every stage of this plan is built on a named, citable method rather than an informal process. The taxonomy follows Nickerson, Varshney, and Muntermann. The maturity model follows Becker, Knackstedt, and Pöppelreuter. The expert validation follows the Delphi method. The economic model is grounded in two-sided market theory (Rochet and Tirole; Parker and Van Alstyne). The governance assessment follows a structured GDPR article mapping. The case study follows Yin's logic for single case justification. The overall paper is framed using the design science research method from Peffers and colleagues.

Every methodological choice in the paper has a clear answer if a reviewer questions it. The coding protocol (Step 3 in section 5) provides inter-rater reliability that standard taxonomy papers lack. The Delphi panel is designed around independence rather than convenience. The maturity model is compared against three named alternative models and explains what it adds. The economic model goes beyond sensitivity analysis to a named theoretical foundation. The governance assessment produces a gap analysis, not a principles list.

---

## 11. Limitations

This paper has four limitations that should be acknowledged.

Single case study. The case demonstration uses Twinlytics as the only platform. This limits the generalizability of the maturity staging, since no comparison case exists to show whether the stage definitions hold for a differently designed platform.

Convenience element in the expert panel. Even with the independence criteria, the external experts are recruited from networks accessible to the research team. This introduces a selection bias that cannot be fully eliminated with the resources available for a doctoral study.

Desk research coverage for use cases. The taxonomy draws on publicly available descriptions of competitor platforms. Proprietary or emerging use cases that are not publicly described will not appear in the taxonomy, which means the taxonomy captures the current visible frontier, not the full possibility space.

Estimated market data. The economic model uses publicly available pricing and market spend data as proxies. Actual platform economics for comparable systems are not publicly disclosed, so the model works with approximations rather than verified figures. The sensitivity analysis is designed to mitigate this limitation, but it cannot eliminate it.

---

## 12. What this paper produces

A validated taxonomy of human digital twin use cases in enterprise and consumer contexts, coded by two independent researchers and validated by an external Delphi panel.

A maturity model showing how digital twin deployments progress from Stage 1 (ungrounded persona with no consent structure) to Stage 5 (fully consented, revenue-sharing, economically autonomous twin), grounded in comparison against three existing maturity frameworks.

Two theoretical claims tested against real data: that consent granularity and monetization mechanism are orthogonal dimensions in a digital twin marketplace, and that two-sided market theory extends to AI simulation platforms.

An economic viability model grounded in two-sided market theory, tested against realistic market data, and stress-tested through sensitivity analysis.

A structured GDPR gap analysis showing where the current Twinlytics design satisfies, partially satisfies, or falls short of key data protection obligations.

A case demonstration walking one complete scenario through the taxonomy, maturity model, economic estimate, and governance assessment.

Together, this gives the thesis a complete, evidence-backed answer to RQ3, and gives the Twinlytics spin-off a validated academic foundation for its business model and governance architecture.
