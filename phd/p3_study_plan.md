# P3 Study Plan and Methodology

## The Twin Economy: Use Cases, Value Architecture, and Governance of a Human Digital Twin Data Marketplace

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

## 3. Overall approach

This study is framed as design science research, following the method from Peffers and colleagues. This is the standard way information systems research builds and evaluates a working artifact, and it fits this paper naturally because Twinlytics is a real, working artifact, not a hypothetical concept.

The method has six steps. Problem identification, defining what a solution needs to do, designing the solution, demonstrating it, evaluating it, and communicating the result. Below is how each step of this paper maps onto that structure.

Problem identification: the four gaps described in section 2, plus the six published papers that already ground this thesis.

Objectives for a solution: a validated use case taxonomy, a workable economic model, and a governance assessment, as set out in RQ3.

Design: the taxonomy and the maturity model, described in sections 4 and 5 below.

Demonstration: a case study run on Twinlytics itself, described in section 7.

Evaluation: expert review of the taxonomy and model, plus the economic modeling with sensitivity testing, described in sections 6 and 7.

Communication: the paper itself.

---

## 4. Building the use case taxonomy

This is Task 1. The method used here is the taxonomy development method from Nickerson, Varshney, and Muntermann, a well established and widely cited method in information systems research.

**Step 1, set the meta-characteristic.** Before collecting any use cases, one central idea is defined that every use case and every category must trace back to. For this paper, the meta-characteristic is the value exchange configuration between the person contributing personal data through their digital twin and the enterprise consuming that data. Every dimension in the taxonomy has to relate back to this idea. This keeps the taxonomy focused instead of becoming a random list of interesting ideas.

**Step 2, gather real cases.** Use cases are pulled from real, existing systems. This includes Twinlytics itself, and known competitors and comparable platforms such as Simile AI, Listen Labs, Aaru, and Synthetic Users. It also includes the use cases already described in the Twinlytics white paper, and any relevant cases mentioned in the published literature.

**Step 3, build the taxonomy through repeated rounds, working in both directions.** One direction is empirical to conceptual, meaning categories are built up from patterns found in the real cases gathered in step 2. The other direction is conceptual to empirical, meaning categories are first proposed from the theory found in the literature review, then checked against the real cases to see if they hold up. Both directions are used across several rounds, and each round refines the categories.

**Step 4, stop only when clear conditions are met.** The taxonomy is not considered finished just because it feels complete. It stops when all of the following are true: no new categories emerge in the last round, every category has at least one real example behind it, no two categories overlap, and the taxonomy is judged concise enough to be useful and detailed enough to be meaningful.

The result of this phase is a structured taxonomy of human digital twin use cases, grouped into a small number of clear categories, each backed by real examples.

---

## 5. Building the maturity model

This connects the taxonomy to a staged view of how mature a human digital twin deployment is, similar in spirit to the stage model used in the LAIA squared paper from Fraunhofer IAO, but built through a more rigorous, named process rather than borrowed directly from an unrelated domain.

The method used here is the maturity model procedure from Becker, Knackstedt, and Pöppelreuter. It has the following phases.

Define the problem and the scope of the model. In this case, the scope is human digital twins used for market research and enterprise decision support, not digital twins in general.

Compare the proposed model against existing models. This includes the LAIA squared model itself, and any other digital twin or AI governance maturity models found in the literature review.

Decide how the model will be developed. This paper builds it iteratively, moving between the taxonomy from section 4 and expert feedback from section 6, rather than writing it in one pass.

Build the model iteratively, defining each stage clearly, from the simplest form of a digital twin, such as an ungrounded LLM persona with no consent structure, through to a fully consented, revenue sharing, economically autonomous twin.

Plan how the model will be evaluated and used. This paper evaluates it through the expert panel described in section 6, and demonstrates it through the case study in section 7.

Document the model clearly enough that someone outside the research team could apply it to a new case.

Evaluate the model against real feedback and decide whether it needs further refinement or is ready to publish.

---

## 6. Expert validation

This is where the taxonomy and the maturity model get checked against real expertise, rather than only against the researcher's own judgment.

The method is a two round Delphi study, a well established method for building structured consensus among a small group of experts.

**Panel.** Around six to ten experts, made up of the PhD supervision team, Twinlytics collaborators, and where possible one or two people with relevant outside expertise in data economy, market research, or platform design.

**Round one.** The draft taxonomy and maturity model are shared with the panel. Each expert rates and comments on the categories, the use cases within them, and the stage definitions, flagging anything unclear, missing, or wrongly placed.

**Round two.** The taxonomy and model are revised based on round one, then sent back to the same panel with a summary of how the group responded the first time. Experts are asked whether they agree with the revised version, and disagreements are discussed until the group reaches a reasonably stable position.

This gives the taxonomy and maturity model a documented, defensible validation step, rather than resting only on the researcher's own analysis.

---

## 7. Economic modeling and case demonstration

This is Task 2 and Task 3 together, the economic architecture and the viability assessment.

**Economic modeling.** For each use case identified in the taxonomy, a techno-economic model estimates the potential value created and captured. This follows the same logic as the LAIA squared paper, using real market data such as vendor pricing, typical enterprise research spend, and comparable platform pricing, which is already partly gathered from the Twinlytics white paper and the desk research done for this thesis.

Unlike a single point estimate, this paper adds a sensitivity analysis. Instead of reporting one return on investment number per use case, the model is run across a range of assumptions, varying the revenue share paid to data contributors between roughly 10 and 20 percent, the price charged per query, and the expected adoption rate. This shows a realistic range of outcomes rather than one number that depends entirely on assumptions nobody can verify in advance, and it answers the most obvious reviewer question before it gets asked.

**Case demonstration.** The taxonomy and maturity model are then demonstrated against a real case using Twinlytics itself. This follows the case study logic set out by Yin, where a single case is justified because it is the only fully built platform of its kind available to the research, not because it was picked at random. The demonstration walks through how a real or realistic scenario, such as an enterprise requesting market research insight through Twinlytics, plays out against the taxonomy categories and the maturity stages, showing where the platform currently sits and what would be needed to reach a higher stage.

This demonstration step is what turns the taxonomy and model from a purely conceptual exercise into something tested against a working system.

---

## 8. What ties the whole paper together

Each phase feeds the next one directly.

The taxonomy from section 4 defines what the use cases actually are.

The maturity model from section 5 shows how mature each use case configuration is in terms of consent, autonomy, and value sharing.

The expert panel in section 6 checks that both of these hold up against outside judgment, not just the researcher's own view.

The economic modeling and case demonstration in section 7 test whether the model is financially workable and whether it holds up against a real platform.

Together, this directly answers all three tasks under RQ3, using one coherent research design instead of three separate, disconnected pieces of work.

---

## 9. Why this design is defensible

Every stage of this plan is built on a named, citable method rather than an informal process. The taxonomy follows Nickerson, Varshney, and Muntermann. The maturity model follows Becker, Knackstedt, and Pöppelreuter. The expert validation follows the Delphi method. The case study follows Yin's logic for single case justification. The overall paper is framed using the design science research method from Peffers and colleagues, which is the standard approach expected at an information systems venue.

This matters for two reasons. First, it means every methodological choice in the paper has a clear answer if a reviewer questions it. Second, it means the paper draws a straight, defensible line from a real gap in the literature to a tested, working result, using Twinlytics as genuine evidence rather than a hypothetical example.

---

## 10. What this paper produces

A validated taxonomy of human digital twin use cases in enterprise and consumer contexts.

A maturity model showing how digital twin deployments progress from basic, ungrounded personas to fully consented, revenue sharing, economically autonomous twins.

An economic viability model for the twin data marketplace, tested against a realistic range of assumptions rather than a single guess.

A demonstration of the taxonomy and model against Twinlytics as a real, working platform.

Together, this gives the thesis a complete, evidence backed answer to RQ3, and gives the Twinlytics spin-off a validated academic foundation for its business model.
