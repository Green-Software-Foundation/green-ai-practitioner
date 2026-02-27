Green Software Foundation · Green AI Committee

#### Green AI Practitioner

Content Audit

*Living Document — Maintained by Project Lead & GSF Staff*

  **PURPOSE**   *This is a living document. It is not part of the course initiation — it is an ongoing activity that begins at project kickoff and is updated as new source material is contributed by SMEs and GAIC members. Its purpose is to ensure every Knowledge Unit has a named source before authorship begins, and to surface gaps that require SME input.*

## 1. Source Authority Principle

Every claim in every Knowledge Unit must be traceable to one of the following three source types. Content that cannot meet this bar is flagged ⚠️ SOURCE NEEDED and held from publication until resolved.

  **Source type**                            **What qualifies**                                                                                                                                                                  **How to cite**

  **Ratified GSF spec or position paper**    A specification or position paper approved by the GSF Steering Committee. Includes SCI for AI (ratified December 2025) and the Green AI Position Paper (ratified September 2024).   *Spec name + section number, e.g. SCI for AI §8.1*

  **Peer-reviewed research cited by GAIC**   Academic or industry research that has been explicitly cited in a GAIC discussion or meeting. Not general web sources.                                                              *Author, title, year, and GAIC session where cited*

  **Named SME contribution**                 A claim made by a named SME from a GAIC member organisation, reviewed and agreed by a second named SME. Must be documented in the content audit.                                    *SME name + organisation + second reviewer name*

## 2. Available Source Material

### 2.1 Ratified GSF Specifications

  **Document**                      **What it provides for the course**                                                                                                                                                                                                           **Status**

  **SCI for AI Specification**      Measurement framework for carbon; consumer/provider boundary; functional units by AI system type; worked LLM and Computer Vision examples; agentic AI compounding requirement (§8.1); Consumer SCI of 0.13 g CO₂e per million tokens (§9.1)   *✓ Ratified December 2025 — ready to use*

  **Green AI Position Paper**       Authoritative definition of Green AI; lifecycle scope; what is in and out of scope for Green AI content                                                                                                                                       *✓ Ratified September 2024 — ready to use*

  **GSF Green Software Patterns**   Existing pattern library applicable to AI inference contexts; patterns catalogue to be extended with SCI for AI-linked entries                                                                                                                *✓ Existing — to be extended alongside course development*

### 2.2 SCI for AI Spec — Directly Usable Content

The following elements from the SCI for AI specification are directly usable as Knowledge Unit source material without additional SME input:

  **Spec section**                   **Submodule(s) it informs**                                          **What it provides**

  **§6.1 — Consumer Boundary**     *Why Your API Calls Have a Carbon Cost*                              Defines exactly what is in scope for a Consumer SCI calculation — API calls, orchestration, scaling, observability, storage, client-side UX, model tool connectors. Definitional anchor for Application Developer content.

  **§8.1 — Functional Units**      *Why Your API Calls Have a Carbon Cost · Choosing the Right Model*   Normative table of functional units by AI system type: per token (LLMs), per workflow execution (agentic), per image, per second (video), per inference (classical ML). Directly usable in submodule content.

  **§8.1 — Agentic compounding**   *Why Your API Calls Have a Carbon Cost*                              Normative requirement: agentic workflows must account for all triggered operations including model executions, tool usage, retrieval steps, and model-to-model exchanges. Source authority for teaching compounding carbon cost.

  **§9.1 — Worked LLM example**    *Why Your API Calls Have a Carbon Cost*                              Complete worked Consumer SCI calculation: 0.13 g CO₂e per million tokens. Ready-made baseline figure for learners. Computer Vision contrast: 0.08 g CO₂e per inference.

### 2.3 GAIC Member SME Contributions

  **TO BE COMPLETED AT KICKOFF**   *This section will be populated at the project kickoff session. Each GAIC member is invited to declare talks, research, case studies, or domain expertise they can contribute as named SME source material. All contributions require a second named reviewer before they can be used in a Knowledge Unit.*

  **Contributor**           **Organisation**   **Contribution type**      **Submodule(s) it informs**   **Second reviewer**

  *e.g. Vincent Caldeira*   *BNP Paribas*      *Talk: semantic routing*   *Routing Mechanisms*          *TBC*

## 3. Content Gaps

The following gaps have been identified after reviewing the SCI for AI specification. Each requires SME input before the relevant Knowledge Units can be authored. Gaps are tracked here with an assigned owner — unresolved gaps block the relevant submodule from progressing past outline.

  **\#**   **Gap**                                         **Why it matters**                                                                                                                                                                                                        **Submodule blocked**                     **Owner**

  **G1**   **Routing pattern effectiveness data**          Which routing strategies (semantic routing, cascade routing) demonstrably reduce Consumer SCI, and by approximately how much. The spec establishes the measurement framework but does not provide reduction benchmarks.   *Routing Mechanisms*                      ⚠️ Unassigned

  **G2**   **Vendor transparency benchmarking**            Which API providers currently publish sufficient data for a Consumer SCI calculation, and what to do when they do not. This is a practical barrier for learners applying the spec.                                        *Why Your API Calls Have a Carbon Cost*   ⚠️ Unassigned

  **G3**   **Real-world Application Developer scenario**   A before/after case study from an actual system, showing the Consumer SCI calculation pre- and post-optimisation. The spec provides the methodology; a member organisation should contribute the scenario.                *Why Your API Calls Have a Carbon Cost*   ⚠️ Unassigned

## 4. Revision History

  **Date**        **Version**      **Updated by**     **Changes**

  February 2026   v0.1 — Draft   GSF Staff          Initial draft. Spec-grounded sources from SCI for AI review. Three content gaps identified. SME contributions section to be populated at kickoff.