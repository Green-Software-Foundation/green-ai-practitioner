# Green AI Practitioner - Course Initiation Document

A Course for Practitioners Building AI Systems

**Document Control**

  **Status**             DRAFT - For Committee Review

  **Owner**              Green AI Committee (GAIC)

  **Sponsor**            Russ Trow, Director of Operations, GSF

  **Platform**           GSF Movement Platform

  **Date**               February 2026

  **Version**            0.1

## 1. Purpose

This document initiates the Green AI Practitioner course on the GSF Movement Platform. It defines the problem we are solving, the target audience, the scope of the MVP, the source foundations the content will be built on, and the decisions the Green AI Committee needs to ratify before production begins.

This is a co-creation document. It is not a final course outline. The committee is invited to challenge, refine, and approve the scope before any content is authored.

## 2. Problem Statement

AI's environmental impact is growing rapidly. Data centre emissions are predicted to rise from 180 Mt to 300 Mt by 2035 in the base case scenario, driven largely by AI workloads. Yet practitioners building AI-enabled systems today face a significant guidance gap:

### Gap 1
*No clear, trustworthy guidance on which technical decisions materially change AI emissions. Not all decisions matter equally — practitioners need signal, not noise.*

### Gap 2
*No consistent way to connect measurement concepts to reduction actions. The SCI for AI specification provides a measurement framework, but practitioners lack a bridge to actionable change.*

### Gap 3
*No practical patterns that survive vendor churn. Model capabilities, pricing, and APIs change constantly. Practitioners need decision frameworks, not tool-specific recipes that go stale.*

### The result
Practitioners who want to build greener AI systems don't know where to start, and organisations that have committed to sustainability targets cannot translate those commitments into engineering decisions.

The Green AI Practitioner course closes this gap — in a way that is shippable, maintainable by a volunteer-led committee, and authoritative because it is grounded in GSF standards.

## 3. Strategic Context

This initiative was anticipated in the Green AI Committee's position paper, published May 2025, which identified the Green AI for Practitioners Course as a priority project alongside the SCI for AI Standard extension. The position paper states directly:

| *"Practitioners and users currently lack clear guidance and knowledge on how to measure, reduce, and report AI impacts. This absence limits public awareness and hinders efforts to address AI's environmental footprint."* |
|                                                                                                                                                                                                                                |
| — Green AI Position Paper, GSF, May 2025                                                                                                                                                                                     |

This course directly delivers on that committee commitment. It also supports GSF's broader strategic goals: driving adoption of the SCI for AI specification, demonstrating member value through high-quality practical education, and growing the Movement Platform as the authoritative home for green software learning. Identifying a project lead for this initiative is the first decision the committee is asked to make (see Section 12).

## 4. How This Course Fits the Broader Ecosystem

### 4.1 The GSF Measurement Framework

The Green Software Foundation is building a measurement framework organised along two axes: impact type and subject domain. Understanding this architecture is essential for scoping the course correctly and positioning it for long-term growth.

| **Level**                                       | **🌍 CARBON**                       | **⚡ ENERGY**                    | **💧 WATER**                     |
| **Top-level ISO Specification**                 | **SCI**                             | **SEE**                          | **SWE**                          |
|                                                 |                                     |                                  |                                  |
|                                                 | *Software Carbon Intensity*         | *Software Energy Efficiency*     | *Software Water Efficiency*      |
|                                                 |                                     |                                  |                                  |
|                                                 | **ISO/IEC 21031:2024 — Ratified** | **In development**               | **Not yet started**              |
| **AI Domain Specification**                     | **SCI for AI**                      | SEE for AI                       | SWE for AI                       |
|                                                 |                                     |                                  |                                  |
|                                                 | **Ratified December 2025**          | *Pending SEE ratification*       | *Pending SWE ratification*       |
| **Practitioner Course Content ← THIS DOCUMENT** | **★ Carbon submodules**             | Energy submodules                | Water submodules                 |
|                                                 |                                     |                                  |                                  |
|                                                 | MVP — grounded in SCI for AI      | *Future — awaiting SEE for AI* | *Future — awaiting SWE for AI* |

The top-level ISO specifications (SCI, SEE, SWE) define the methodology for each impact type. The domain specifications (SCI for AI, SEE for AI, SWE for AI) apply that methodology to the specific characteristics of AI systems. The practitioner course content sits one level below the domain specs — translating them into role-specific, actionable guidance for practitioners.

Carbon comes first because SCI for AI is the only ratified AI domain specification. Energy and water submodules will follow as SEE for AI and SWE for AI are ratified. The course is designed so that when they arrive, they slot into the existing structure without requiring a rebuild.

### 4.2 Immediate Deliverables: How This Course Relates to Other GAIC Work

Within the Green AI practitioner education effort, three distinct deliverables are in play. This document covers only the third:

  **Deliverable**                                   **What it covers**                                                                                                                                                                                                       **Led by**                                **Status**

  SCI for AI Fundamentals Course                    Introduces the SCI for AI specification in depth: methodology, provider/consumer model, how to apply it. Measurement-focused.                                                                                            Asim Hussain / Standards Working Group    *In development — not covered by this document*

  Green AI Patterns                                 Bite-sized, actionable patterns linked to the SCI for AI. Each pattern shows which part of the SCI it impacts and how. Extension of existing patterns catalogue.                                                         GAIC in collaboration with Standards WG   *Existing catalogue to be extended and updated*

  **Green AI Practitioner Track ← THIS DOCUMENT**   Foundation + persona-based tracks. Bridges the measurement framework and patterns through the lens of a practitioner role. Starts with carbon; designed to expand to energy and water as AI domain specs are ratified.   GAIC — project lead to be confirmed     *Initiation stage*

The practitioner track is the bridge layer. It assumes learners will encounter the SCI for AI fundamentals course, and it points to specific patterns in the patterns catalogue. It does not replace either — it connects them through the lens of a specific practitioner persona. As SEE for AI and SWE for AI are ratified, equivalent fundamentals courses and pattern extensions will follow, and this practitioner track will expand accordingly.

## 5. Course Definition

### 5.1 Course Type

Type 2: Practitioner (Implementation). The goal is to equip learners to make concrete, impact-reducing decisions in the AI systems they build — not to raise general awareness.

Success looks like: a learner who completes the course can make a specific decision differently on Monday — a model choice, a routing strategy, an infrastructure configuration — and knows why it reduces environmental impact. They can also explain what Green AI means, what is in and out of scope, and how to measure the environmental impact of their decisions using the GSF measurement framework.

### 5.2 Overarching Purpose

Help practitioners understand what Green AI means and how to measure the full environmental impact of AI systems — then reduce that impact through practical, evidence-based decisions relevant to their specific role. The course starts with carbon because SCI for AI is the first ratified AI domain specification. It is designed to expand naturally to energy (SEE for AI) and water (SWE for AI) as those specifications are ratified.

### 5.3 The Three-Pillar Measurement Architecture

The GSF measures the environmental impact of software across three pillars. Each pillar has a top-level ISO methodology and a corresponding AI domain specification. The practitioner course is designed to teach all three — in sequence, as the domain specs become available.

  **Pillar**            **What it measures**                                      **AI domain spec**                          **Course submodules**   **Status**

  **🌍 Carbon (SCI)**   gCO₂e emitted per functional unit of AI work              **SCI for AI — Ratified December 2025**   **★ MVP**               **In scope now**

  **⚡ Energy (SEE)**   kWh consumed per functional unit of AI work               SEE for AI — Pending SEE ratification     Future                  *Awaiting spec*

  **💧 Water (SWE)**    Water consumed/withdrawn per functional unit of AI work   SWE for AI — Pending SWE ratification     Future                  *Awaiting spec*

  **IMPORTANT**   *The course must not make specific claims about what SEE for AI or SWE for AI will measure or require. The Foundation module can name them as forthcoming standards and explain the framework logic — but no content about their methodology may be included until the respective domain specs are ratified. The same SOURCE NEEDED principle applies: we do not assert what we cannot substantiate.*

### 5.4 Two-Layer Structure

The course is built in two layers. Every learner completes Layer 1 before self-selecting into Layer 2 based on their role.

  **Layer**     **Name**                                   **What it covers**                                                                                                                                                                                                                                                                           **Completion model**

  **Layer 1**   **Foundation: Introduction to Green AI**   What Green AI is (and is not); the AI lifecycle; the three-pillar measurement framework (carbon, energy, water); the consumer/provider lens; why carbon is the starting point; how the GSF spec family is designed to grow. Expands on the GSF position paper for a practitioner audience.   **Mandatory prerequisite for all persona modules**

  **Layer 2**   **Persona Modules**                        Role-specific submodules organised by both persona and impact pillar. Each track starts with carbon (SCI for AI), with energy and water submodules added as domain specs are ratified. Tracks build independently and grow over time.                                                        Self-selected by role after completing the Foundation. Tracks are parallel — a learner completes their track, not all tracks.

This structure is deliberate. The Foundation ensures every practitioner shares a common understanding of Green AI and the three-pillar framework before encountering role-specific content. The persona modules then deliver actionable guidance without requiring learners to wade through material that does not apply to them — and each track grows systematically as new domain specs are ratified.

### 5.5 Why This Structure Works

-   Shippable: the Foundation module and first carbon submodule can go live now, independently of the full course

-   Maintainable: individual submodules can be updated as tooling or specs evolve without touching the Foundation or other tracks

-   Volunteer-friendly: authorship can be distributed by persona module and impact pillar — each has its own content lead and SME reviewer

-   Extensible by design: energy and water submodules slot into existing tracks when SEE for AI and SWE for AI are ratified — no structural rebuild required

### 5.6 Scope Discipline

All content must be consistent with the Green AI definition ratified by the Steering Committee in September 2024:

  **DEFINITION**   *Green AI focuses on reducing the environmental impact of AI systems throughout their lifecycle. It emphasizes the standardization of measurement and metrics to ensure transparency, strengthen confidence in AI technologies, and drive continual improvement.*

In scope: environmental impact of AI systems — energy, emissions, water, hardware. Out of scope: AI for sustainability, Responsible AI, AI safety. Modules must not drift into adjacent domains.

### 5.7 Coordination with the Standards Working Group

  **COORDINATION NOTE**   *Asim Hussain and the Standards Working Group are developing SCI for AI Fundamentals (and will develop equivalent courses as SEE and SWE specs mature). The Foundation module in this track must not duplicate that work — its purpose is to introduce the three-pillar framework at the level needed to contextualise persona modules, not to provide deep specification tutorials. The committee should coordinate with the Standards WG on (a) where the fundamentals courses end and practitioner tracks begin, and (b) timing of SEE for AI and SWE for AI ratification so energy and water submodules can be scoped proactively.*

### 5.8 Content Architecture: Building for Humans and AI

This course is designed to be consumed by humans today. But the rise of AI-assisted development — vibe coding, agentic programming, AI pair programmers embedded in the software development lifecycle — means that within the lifespan of this course, AI systems will be as important an audience as the human practitioners we are building for now.

This creates a design constraint that must be established at the start: the underlying course knowledge must be structured so that it can be rendered for either audience without rebuilding the content from scratch.

### 5.9 Content Hierarchy

The course is structured across four levels. Understanding this hierarchy is essential before any content authorship begins — it defines what a volunteer is asked to produce, and how their contribution fits into the larger structure.

  **Level**                  **Term**                  **What it is**                                                                                                                                                                                                                                                                                  **Example**

  **1 — Course**           **Course**                The whole thing. One course, multiple modules. Has a single title, a single tagline, and one set of overarching learning outcomes.                                                                                                                                                              *Green AI Practitioner*

  **2 — Module**           **Module**                A major section of the course. Either the Foundation (mandatory for all learners) or a persona module (role-specific, self-selected). A module is the sum of its submodules — it has no fixed length ceiling. A learner 'completes a module' when they have completed all its submodules.   *Foundation: Introduction to Green AI · Application Developer module · Infrastructure & Operations module*

  **3 — Submodule**        **Submodule**             A single, completable video unit. The atomic learner-facing deliverable. Has one learning objective, one video (3–5 minutes), and one quiz assessment. This is what gets published, completed, and certified.                                                                                  *Why Your API Calls Have a Carbon Cost · Choosing the Right Model · Routing Mechanisms*

  **4 — Knowledge Unit**   **Knowledge Unit (KU)**   A structured content artifact that underpins a submodule. Not visible to learners — it is the source of truth from which the video script and AI ruleset are derived. A submodule is typically built from 3–6 Knowledge Units. A volunteer can author one KU in a lunch break.               *Principle: prefer smaller models for classification tasks · Condition: task is token classification or extraction · Decision: route to a model under 7B parameters · Rationale: SCI for AI §8.1*

This hierarchy is the shared vocabulary for all authorship, review, and committee discussions. When a volunteer is assigned a piece of work, it will always be at the Knowledge Unit level — the smallest, most tractable unit of contribution.

### 5.10 The Knowledge Unit

The fundamental building block of this course is not a video script. It is a Knowledge Unit — a structured, machine-readable record that captures a single principle, decision, or pattern with enough precision to be rendered as either a human-facing lesson or an AI-consumable ruleset.

Each Knowledge Unit captures the following fields:

  **Field**             **What it contains**                                                                         **Why it matters**

  **Principle**         A single, precisely stated rule or recommendation                                            *The atomic unit of knowledge — unambiguous enough for an AI to act on*

  **Condition**         When the principle applies — persona, context, system type                                 *Enables routing: an AI or human selects relevant Knowledge Units for their situation*

  **Decision**          The recommended action                                                                       *The actionable output — what to do, not just what to know*

  **Rationale**         Why, with explicit spec citation (e.g. SCI for AI §8.1)                                      *Enables source traceability for both human learners and AI systems*

  **Trade-offs**        What is gained and what is given up                                                          *Prevents over-application; teaches judgment not just compliance*

  **Impact**            How this moves the SCI (or SEE / SWE) score, with reference data where available             *Connects decision to measurable outcome — the course's core promise*

  **Pattern link**      Which Green AI Pattern this Knowledge Unit corresponds to, if any                            *Connects the course to the patterns catalogue — the AI distribution layer*

  **Rendering notes**   Guidance for Claude when deriving the video script and AI ruleset from this Knowledge Unit   *Allows the same Knowledge Unit to be expressed appropriately in each format*

### 5.11 From Knowledge Units to Rendered Outputs

A submodule is a sequenced collection of Knowledge Units, authored for a specific persona. Once the Knowledge Units have been authored and SME-approved, Claude is used to derive the rendered outputs — no re-authoring of the underlying content required:

  **Output**                       **Audience**                                 **What the Knowledge Unit becomes**

  **Video script + quiz**          Human learner                                *Narrative explanation of the principle, decision, and trade-offs. Derived from approved Knowledge Units by Claude (AI), reviewed by the content lead before production.*

  **Green AI Pattern**             Human developer (reference)                  *The principle and decision fields become the pattern statement; impact and rationale become the pattern evidence*

  **System prompt ruleset**        AI coding assistant (e.g. Claude, Copilot)   *Principles and decisions rendered as policy rules injected into an agent's context — 'prefer smaller models for classification tasks'*

  **MCP tool / policy document**   AI agent in a development workflow           *A structured document an agent can query to evaluate whether a proposed architectural decision is green-software compliant*

  **Fine-tuning signal**           Future AI models                             *Well-structured, citable Knowledge Units become part of the training signal that bakes green software principles into future coding models*

  **STRATEGIC NOTE**   *The Green AI Patterns catalogue is the natural AI distribution layer for this course. Patterns are already structured and discrete — they are, in effect, Knowledge Units rendered for a developer reference audience. The course and the patterns catalogue should be designed in coordination: Knowledge Units authored for the course should feed the patterns catalogue, and patterns should link back to the relevant submodule. In both cases, Claude derives the rendered output from the approved Knowledge Unit — keeping humans in the authorship and review loop while using AI for the conversion work. This is not two separate outputs — it is one knowledge base with two human-facing renderings and an expanding set of AI-facing ones.*

## 6. Target Audience

### 6.1 The Consumer/Provider Distinction

The SCI for AI specification frames the AI ecosystem through a consumer/provider lens. This distinction is foundational for the course:

  **Term**              Who they are

  **Provider**          Organisations that operate AI infrastructure and expose it as a service — cloud AI APIs, model hosting platforms, inference infrastructure operators

  **Consumer**          Organisations and individuals who call those services to build AI-enabled products — developers, engineers, architects integrating AI via APIs

This course targets AI consumers. Specifically, it targets the technical practitioners within consumer organisations who make the decisions that determine how AI is used — not the providers who build the underlying infrastructure, and not general end-users who interact with finished AI products through a chat interface.

  **FROM THE COMMITTEE**   *"People who just send prompts to ChatGPT — what are you going to influence? Nothing much. People who actually make active difference right now would be application developers who are building with AI. They can actually take meaningful decisions that have a huge impact." — Vincent Caldeira, GAIC (February 2026)*

### 6.2 Persona Definition: A Committee Decision

Deciding which personas the course serves — and in what priority order — is a committee decision, not a content decision. It determines what gets built, in what sequence, and where volunteer effort is directed. It must be made explicitly and documented before any submodule outline work begins.

The committee should evaluate each candidate persona against three criteria:

  **Criterion**         The question to answer

  **Impact**            How large and direct is this persona's influence over the environmental impact of AI systems? Can they actually move the SCI score?

  **Reach**             How many people occupy this role across GSF member organisations? Does this persona represent a large enough audience to justify the investment?

  **Readiness**         Is there sufficient source material, SME availability, and spec grounding to produce high-quality Knowledge Units for this persona now?

### 6.3 Proposed Persona Prioritisation

The following personas are proposed for committee ratification. The priority order reflects impact, reach, and readiness. The committee should confirm, reorder, or amend this list as part of its review of this document.

  **\#**        **Persona**                                **Primary decisions in scope**                                                                                                       **Rationale for priority**

  **1 ★ MVP**   **Application Developer (AI Consumer)**    Model selection · Prompt design · Response caching · Request batching · Model routing · Fallback strategy · When not to use AI       *Highest direct impact on Consumer SCI — every API call is a decision. Largest reachable audience across GSF members. SCI for AI spec fully covers this persona. Cost and carbon reduction are the same decision — strong practitioner motivation. Identified by committee as the correct starting point (Vincent Caldeira, February 2026).*

  **2**         **Infrastructure & Operations Engineer**   Serving infrastructure · Hardware selection · Deployment environments · Edge AI vs. cloud AI · Scaling policies · FinOps alignment   *High infrastructure-level leverage over operational emissions. Strong overlap with GSF Hardware Standards WG work. Reaches a distinct audience from Application Developers.*

  **3**         **ML / AI Engineer**                       Fine-tuning · Evaluation · Quantisation · Model optimisation · Training efficiency                                                   *Training emissions can dwarf inference at scale — but this persona has a narrower audience and the source material is more specialist. Better positioned as track 3 once the pattern for Knowledge Unit authorship is established.*

  **4**         **Architect / System Designer**            Full-stack carbon reduction · Layered efficiency strategies · System-level design patterns · Build vs. buy decisions                 *High leverage over long-term system architecture, but decisions are more contextual and harder to reduce to discrete Knowledge Units. Well-suited to a mature course once the authorship model is proven.*

*⚠️ Committee decision required: Confirm or amend this prioritisation. Once ratified, it becomes the sequencing plan for track development and volunteer recruitment.*

### 6.4 MVP Persona Detail: The Application Developer (AI Consumer)

The Application Developer is a practitioner who integrates AI capabilities into products and services primarily by calling model APIs. This persona was explicitly identified by the committee as the highest-impact starting point. Their decisions directly determine how AI resources are consumed at scale — and reducing carbon cost and reducing API spend are usually the same decision.

  **Persona**                 Application Developer (AI Consumer)

  **Primary activity**        Calling model APIs (OpenAI, Anthropic, Google, Hugging Face, etc.) to build AI-enabled features and applications

  **Key decisions**           Model selection, prompt design, response caching, request batching, model routing, fallback strategy, when to use AI vs. a simpler solution

  **Carbon levers**           Model size vs. task fit, inference volume, routing to smaller models, cache hit rate, geographic region, quantised vs. full-precision models for dev/test contexts

  **Cost alignment**          Most decisions that reduce carbon cost also reduce API spend — a feature, not a coincidence

  **Prerequisites assumed**   Comfortable with APIs, REST/HTTP, basic software architecture; no ML training or infrastructure background required

  **Does NOT include**        Model training, fine-tuning, infrastructure provisioning, hardware selection, serving infrastructure

Vincent Caldeira provided a concrete example of the kind of decision this persona can make: semantic model routing — training a small language model to identify when a request does not need to be routed to a large, general-purpose model. This single architectural decision, learnable in roughly 5 minutes, can significantly reduce overall model resource consumption. This is the type of content this track will deliver.

### 6.5 Agentic AI: In-Scope, Not a Future Extension

The SCI for AI specification explicitly covers agentic AI as a first-class paradigm within the Consumer boundary, with per-workflow-execution as its functional unit. The spec notes that emissions from agentic systems must account for all triggered operations — model executions, tool usage, retrieval steps, and model-to-model exchanges.

Many Application Developers are already building agentic systems. A RAG pipeline, a tool-calling agent, or a multi-step reasoning workflow can compound inference costs in ways that are not intuitively obvious from a per-API-call mental model. The course must address this — even in the MVP — or risk teaching a simplified model that breaks down for the majority of real-world applications.

The committee should decide whether to address agentic AI within the first carbon submodule (as a complexity flag), as a dedicated second submodule, or as a routing/design consideration in a later submodule. All three are valid; the spec gives us the source authority for any of them.

## 7. Authorship Flow and MVP Scope

### 7.1 The Full Authorship Flow

The course is built through a repeatable, six-phase flow. Each phase has a clear owner and a defined gate before the next phase begins. This structure ensures that volunteer effort is always directed at well-defined, bite-sized pieces of work — and that nothing gets built before the upstream decisions that should inform it have been made.

  **\#**   **Phase**                       **What is decided or produced**                                                                                                                                                                                                             **Owner / gate**

  **1**    **Initiation**                  Course purpose, structure, constraints, Knowledge Unit schema, and decisions required. This document.                                                                                                                                       *Committee approves before any other phase begins*

  **2**    **Course outline**              A single-page expression of the course: title, tagline, target audience, prerequisites, overarching learning outcomes, high-level module structure, and what success looks like. The shared reference point for all subsequent decisions.   *Project lead drafts · Committee approves · Becomes the public-facing course description and the internal anchor for all content decisions*

  **3**    **Persona definition**          Which personas does the course serve? Evaluated against impact, reach, and readiness criteria. Priority order agreed.                                                                                                                       *Committee decision — documented and ratified. Unlocks track development in priority sequence.*

  **4**    **Submodule definition**        For each persona, what submodules does its track need? What is the candidate list of submodules across all impact pillars (carbon, energy, water)?                                                                                          *Project lead proposes · Committee ratifies. Submodules are named and scoped before any outline work begins.*

  **5**    **Submodule prioritisation**    Given the full candidate submodule list across all personas and pillars, what is the sequenced delivery roadmap? What ships in the MVP? What ships next?                                                                                    *Project lead proposes · Committee ratifies. Produces the live roadmap — public commitment to volunteers and members.*

  **6**    **Submodule outline**           For a prioritised submodule: which Knowledge Units will it contain, in what sequence? Scope confirmed before authorship begins. Small enough for a volunteer to complete in a session.                                                      *Content lead produces · SME reviewer approves*

  **7**    **Knowledge Unit authorship**   Volunteer authors one Knowledge Unit at a time: principle, condition, decision, rationale, trade-offs, impact, pattern link, rendering notes. The source of truth.                                                                          *Content lead assigns · SME reviewer approves each KU · Gate before any rendering begins*

  **8**    **Human rendering**             Claude derives the video script from approved Knowledge Units. Content lead reviews the output. GSF staff check for course standards, terminology, and scope compliance. SME sign-off before production.                                    *Claude (AI) derives script · Content lead reviews · GSF staff standards check · SME sign-off before production*

  **9**    **AI rendering**                Claude derives the structured ruleset from approved Knowledge Units. Suitable for system prompt, MCP tool, or pattern entry. Published alongside the video.                                                                                 *Claude (AI) derives ruleset · GSF staff review and publish · Coordinated with patterns catalogue*

Phases 1–5 are committee decisions. Phases 6–9 are content execution — the work volunteers actually do. The distinction matters: no volunteer should ever be asked to define what a submodule is. That decision should already be made when they pick up a Knowledge Unit assignment.

### 7.2 MVP Scope: What This Document Initiates

This document initiates Phase 1 (Initiation) and proposes the outputs of Phases 2, 3, 4, and 5 for committee ratification. If the committee approves this document, Phase 6 (Submodule outline) can begin immediately for the Foundation module and the first Application Developer carbon submodule.

  **MVP DEFINITION**   *The MVP is: the Foundation module and the first Application Developer carbon submodule live on the Movement Platform. Both pass through the full authorship flow — outline, Knowledge Units, human rendering, AI rendering, production, publication. Done when published with quiz assessment and structured ruleset.*

### 7.3 Proposed MVP Submodules (Phases 3–5 outputs, for committee approval)

The following represents the proposed output of Phases 3, 4, and 5 for the MVP. The committee should confirm, amend, or reject each element.

| **Layer / Track**                        | **Submodule**                                                                                                         | **🌍 Carbon (SCI for AI)**        | **⚡ Energy (SEE for AI)**        | **💧 Water (SWE for AI)**         |
| **LAYER 1 FOUNDATION**                   | **★ Introduction to Green AI \[MVP\]**                                                                                | ✓ Introduces SCI for AI framework | *Names SEE for AI as forthcoming* | *Names SWE for AI as forthcoming* |
|                                          |                                                                                                                       |                                   |                                   |                                   |
|                                          | *Green AI definition · AI lifecycle · Three-pillar framework intro · Consumer/provider lens · Why carbon comes first* |                                   |                                   |                                   |
| **LAYER 2 APPLICATION DEVELOPER TRACK**  | **★ Why Your API Calls Have a Carbon Cost \[MVP\]**                                                                   | **★ MVP**                         | *Future — SEE for AI*           | *Future — SWE for AI*           |
|                                          |                                                                                                                       |                                   |                                   |                                   |
|                                          | *Consumer SCI · Per-token FU · Worked LLM example · Agentic compounding*                                              |                                   |                                   |                                   |
|                                          | Choosing the Right Model \[future\]                                                                                   | *Future carbon*                   | *Future — SEE for AI*           | *Future — SWE for AI*           |
|                                          |                                                                                                                       |                                   |                                   |                                   |
|                                          | *Model size vs. task fit · Right-sizing · When not to use AI · Quantisation*                                          |                                   |                                   |                                   |
|                                          | Routing Mechanisms \[future\]                                                                                         | *Future carbon*                   | *Future — SEE for AI*           | *Future — SWE for AI*           |
|                                          |                                                                                                                       |                                   |                                   |                                   |
|                                          | *Semantic routing · Cascade routing · Small model routing*                                                            |                                   |                                   |                                   |
| **LAYER 2 INFRA & OPS TRACK \[future\]** | *Submodules TBD by committee*                                                                                         | *Future carbon*                   | *Future — SEE for AI*           | *Future — SWE for AI*           |
|                                          |                                                                                                                       |                                   |                                   |                                   |
|                                          | *Serving infra · Hardware selection · Deployment environments · Edge vs. cloud · Scaling · FinOps*                    |                                   |                                   |                                   |
| **LAYER 2 FURTHER TRACKS \[future\]**    | *ML / AI Engineer · Architect / System Designer · others as GAIC work develops*                                       | *Future*                          | *Future*                          | *Future*                          |

★ = MVP scope. Carbon column: green = active/ratified spec. Energy column: amber = SEE pre-draft, SEE for AI not yet started. Water column: blue = SWE not yet started, SWE for AI not yet started. No content may be authored for energy or water submodules until the respective AI domain specification is ratified.

### 7.4 Foundation Module Specification

The Foundation module is the conceptual anchor for the entire course. It establishes the vocabulary and measurement framework that every persona module builds on — and it must introduce all three pillars even though only carbon has a ratified AI domain spec today.

  **Learning objective**   Explain what Green AI is (and is not), describe the three-pillar environmental measurement framework (carbon, energy, water), and articulate why carbon is the starting point for practitioners today

  **Source**               GSF Green AI Position Paper (May 2025) · SCI for AI specification §2–6 · SEE specification (pre-draft) — for framing only, no methodology claims

  **Key topics**           The ratified Green AI definition · What is in scope and out of scope · The AI lifecycle stages · The three-pillar framework: SCI, SEE, SWE and their AI domain specs · Consumer vs. provider boundary · What a functional unit is and why it matters · Why carbon has the ratified spec today · What energy and water submodules will cover when domain specs are available

  **Tone**                 Conceptual but grounded — this is not an awareness course. By the end, learners should understand the measurement framework well enough to place their persona module within it, and know what is coming next.

  **Measurement depth**    Introduces the three-pillar framework at orientation level. Carbon (SCI for AI) gets the most depth — enough to contextualise the first persona submodule. Energy and water are named and framed but not taught in detail. Does not duplicate the SCI for AI Fundamentals course (Standards WG). See Section 5.7.

  **Estimated length**     5–8 minutes — slightly longer than a standard submodule given the conceptual breadth, but still bite-sized

### 7.5 What Is Out of Scope for the MVP

-   Model training and fine-tuning (ML Engineer persona — future track)

-   Infrastructure and hardware decisions (Infrastructure & Operations persona — future track)

-   The remaining Application Developer submodules — Choosing the Right Model and Routing Mechanisms — are defined in the architecture but not authored for MVP

-   Certification or badging — quiz assessment only for v1

-   Multi-language delivery

## 8. Course Outline

The course outline is produced in Phase 2 of the authorship flow — after this initiation document is approved and before persona and submodule decisions are made. It is a separate, standalone document designed to be shared with members, volunteers, and prospective learners without requiring them to read the full initiation document.

  **SEPARATE DOCUMENT**   *The Green AI Practitioner Course Outline is a companion document to this initiation. It covers: title, tagline, course type, target audience, prerequisites, overarching learning outcomes, course structure, delivery format, grounding, and success measure — all on a single page. Committee decision required: approve the course outline before submodule work begins.*

The outline is stable by design — it should not need to change as individual submodules are added or updated. If the committee needs to amend it, that is a signal that the course scope or purpose has changed, and this initiation document should be updated accordingly.

## 9. Content Audit

A content audit is required before Knowledge Unit authorship begins for any submodule. Its purpose is to inventory what source material already exists — from GSF specifications, position papers, GAIC member talks, and SME contributions — and map it to the submodules it can inform. This prevents duplication, identifies gaps that need SME input, and gives content leads a starting point rather than a blank page.

  **SEPARATE DOCUMENT**   *The Green AI Practitioner Content Audit is a living document maintained by the project lead and GSF staff. It is not part of this initiation — it is an ongoing activity that begins at kickoff and is updated as new source material is contributed. It covers: available now (ratified specs, position papers, GAIC talks), source authority for each claim type, identified content gaps requiring SME input, and gap owners.*

The source authority principle applies across all content: every claim in every Knowledge Unit must be traceable to a ratified GSF specification, peer-reviewed research cited by the GAIC, or a named SME contribution reviewed by a second SME. Content that cannot meet this bar is flagged ⚠️ SOURCE NEEDED and held from publication until resolved.

## 9. Course Standards

All submodules in the Green AI Practitioner course will comply with the following GSF standards. These are non-negotiable and apply to all content regardless of who authors it.

  **Standard**              **Requirement**

  **Submodule length**      3–5 minutes per submodule (\~390–650 words at 130wpm). No submodule to exceed 6 minutes. A module (Foundation or persona module) is the sum of its submodules and has no fixed length ceiling.

  **Learning objectives**   One per submodule. Must use a Practitioner action verb: Calculate, Distinguish, Select, Design, Apply, Implement.

  **Terminology**           SCI (not 'carbon score'), functional unit, embodied emissions, operational emissions, carbon intensity — as defined in the SCI specification.

  **Scope discipline**      No content on AI for sustainability, Responsible AI, or AI safety. Any content that drifts must be flagged and removed.

  **Assessment**            5–7 quiz questions per submodule. One correct answer, two plausible distractors. Pass mark: 70%.

  **Source integrity**      No unsubstantiated assertions. ⚠️ SOURCE NEEDED flags all gaps. Nothing ships without source resolution.

  **Tone**                  Authoritative, precise, practitioner-level. Direct. No corporate jargon.

## 10. Delivery Model

### 10.1 Platform

The GSF Movement Platform. Submodules will be published as standalone, completable units within each module of the Green AI Practitioner course. Learners can complete modules independently or in sequence.

### 10.2 Authorship Model

Volunteer-led, committee-reviewed. The full authorship flow is defined in Section 7.1 — eight phases from initiation through AI rendering, with explicit gates between each phase. The key principle is that volunteer content work (phases 5–8) only begins once committee decisions (phases 1–4) have been made and documented.

Each submodule has three named roles throughout its authorship:

  **Role**              Responsibility

  **Content lead**      Authors the submodule outline and Knowledge Units. Reviews the video script derived by Claude from approved Knowledge Units. Named GAIC member.

  **SME reviewer**      Reviews each Knowledge Unit for technical accuracy before rendering begins. Must be distinct from the content lead. Signs off before any script is written.

  **GSF staff**         Verifies spec citations in Knowledge Units. Reviews Claude-derived scripts for course standards compliance. Coordinates Claude-derived AI rendering (structured ruleset). Manages platform publication.

No script may be written before the Knowledge Units for that submodule have been SME-approved. No module may be published without content lead approval, SME reviewer sign-off, and GSF staff standards clearance.

### 10.3 Maintenance Commitment

The committee commits to reviewing each live module on a six-month cycle. When content changes are required — due to spec updates, tooling evolution, or new vendor data — the Knowledge Units are updated first, and all renderings (video script, structured ruleset, pattern entries) are re-derived from the updated Knowledge Units. This keeps all output formats in sync from a single source of truth.

A named update owner will be assigned within 30 days of any material change being identified.

## 11. Proposed Timeline

  **Phase**                                        **Target**         **Activities**

  **Initiation (Phase 1)**                         Week 1–2          Committee reviews and approves this document. Persona prioritisation, MVP submodule definition, and Knowledge Unit schema ratified (Phases 2–4). Project lead and content leads assigned.

  **Submodule outlines (Phase 5)**                 Week 3–4          Content leads produce outlines for the Foundation module and first Application Developer carbon submodule — the list of Knowledge Units each contains, sequenced. Committee confirms scope before authorship begins.

  **Knowledge Unit authorship (Phase 6)**          Week 4–7          Volunteers author Knowledge Units one at a time in structured markdown. SME reviewers approve each. GSF staff verify spec citations. No script written until all KUs for a submodule are approved.

  **Human rendering: scripts (Phase 7)**           Week 7–9          Content leads derive video scripts from approved Knowledge Units. GSF staff review for course standards, terminology, and scope discipline.

  **AI rendering: structured ruleset (Phase 8)**   Week 8–9          GSF staff derive machine-readable ruleset from approved Knowledge Units. Coordinated with patterns catalogue. Published alongside the video module.

  **Production**                                   Week 9–11         Scripts recorded and edited. Quiz questions authored and reviewed. Pattern links confirmed.

  **Publish**                                      Week 11–13        Foundation module and first Application Developer submodule live on Movement Platform. Structured ruleset published. Internal GAIC announcement. External comms planned.

## 12. Decisions Required from the Green AI Committee

The committee is asked to review and resolve the following before content development begins:

  **\#**   **Decision**                                                                                                                                                   **Options / Notes**

  **1**    Appoint a project lead for the Green AI Practitioner track                                                                                                     *Named GAIC member responsible for driving the track from initiation through publication and maintenance*

  **2**    Approve the two-layer course structure and full authorship flow (Section 7.1) as defined                                                                       *Approve as-is / Amend structure / Propose alternative*

  **3**    Approve the Knowledge Unit authorship model and schema (Section 5.9) — structured artifacts as the source of truth for all renderings                        *Approve as-is / Modify the schema / Revert to traditional script-first authorship*

  **4**    Ratify the persona prioritisation (Section 6.3) — Application Developer first, then Infrastructure & Operations, ML/AI Engineer, Architect/System Designer   *Confirm order / Resequence / Add or remove personas*

  **5**    Ratify the MVP submodule definition — Foundation module + first Application Developer carbon submodule as the first delivery                                 *Confirm / Change first submodule / Add a second MVP submodule*

  **6**    Ratify the proposed Application Developer track submodule list as the carbon-pillar roadmap for that track                                                     *Approve outline / Amend submodule titles or scope / Add or remove submodules*

  **7**    Approve the three-pillar framework framing in the Foundation module — carbon now, energy and water as AI domain specs are ratified                           *Approve as-is / Limit Foundation to carbon only / Propose alternative framing*

  **8**    Approve the Foundation module scope: Green AI concepts + three-pillar intro + introductory SCI for AI measurement, mandatory prerequisite                      *Approve as-is / Limit to conceptual only / Split into two foundation modules*

  **9**    Confirm self-selection as the persona module model                                                                                                             *Approve / Require recommended-track guidance / Committee prescribes track per role*

  **10**   Assign a content lead and SME reviewer for the Foundation module                                                                                               *Must be distinct roles; content lead authors Knowledge Units, SME reviewer signs off technical accuracy*

  **11**   Assign a content lead and SME reviewer for the first Application Developer carbon submodule                                                                    *Must be distinct roles; can overlap with Foundation assignments if capacity allows*

  **12**   Agree coordination approach with Standards WG on scope boundary and SEE/SWE for AI timing                                                                      *Russ Trow to facilitate with Asim Hussain and Standards WG before Foundation KUs are drafted*

  **13**   Confirm source material inventory and flag gaps                                                                                                                *Committee to review at kickoff session*

  **14**   Approve the maintenance model (6-month review cycle, KUs updated first)                                                                                        *Approve as-is / Propose alternative cadence*

## 13. Next Steps

Once the committee has reviewed this document, the following will proceed:

1.  Committee review and feedback on this initiation document (async, via GitHub or email, suggested 10 working days)

2.  Kickoff session with content leads and SME reviewers to walk through standards and timeline

3.  Source material inventory — committee members share relevant talks, papers, and internal content

4.  Module outline drafts produced for committee review before scripts are written

5.  First module scripts drafted, reviewed, and approved

## Appendix: Key References

-   Green AI Position Paper — greensoftware.foundation/articles/green-ai-position-paper

-   SCI Specification — sci.greensoftware.foundation

-   Green Software Patterns — patterns.greensoftware.foundation

-   GSF Movement Platform — grnsft.org/mov-plat-gsp

-   GSF Green AI Committee — directory.greensoftware.foundation/committees

-   GAIC Definition of Green AI (ratified September 2024) — see Section 4.4 of this document

greensoftware.foundation