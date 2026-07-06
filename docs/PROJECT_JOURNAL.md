# AI QA Framework - Project Journal

## Session 006

**Date**

2026-07-06

**Goal**

Review the complete first draft of the AI QA Framework and start consolidating glossary terms in `docs/fundamentals/AI_Glossary.md`.

**Completed**

- Created the daily note for Session 006.
- Reviewed the role of the glossary in supporting the main framework document.
- Kept the title `AI Glossary for Quality Assurance`.
- Updated the Purpose section of the glossary.
- Aligned the definition of `AI Quality Assurance` with the main framework document.
- Added and refined key glossary terms, including:
  - `AI-based system`
  - `AI component`
  - `AI QA Lifecycle`
  - `AI-specific risk`
  - `Artefact`
  - `Bias`
  - `Data drift`
  - `Decision record`
  - `Evidence`
  - `Fallback mechanism`
  - `Hallucination`
  - `Human oversight`
  - `Model degradation`
  - `Prompt injection`
  - `Quality dimension`
  - `Residual risk`
- Confirmed that the glossary uses practical QA-oriented definitions rather than replacing formal standards or certification definitions.
- Committed the glossary update and Session 006 daily note.

**Key Decisions**

- The glossary will support consistent terminology across the AI QA Framework.
- Glossary definitions should be practical, QA-oriented and aligned with the main framework document.
- The glossary does not claim to replace formal definitions from standards, regulations or certification bodies.
- The glossary will evolve incrementally as new framework documents, templates and examples are created.

**Review Notes**

- The glossary is now better aligned with `docs/framework/AI_QA_Framework.md`.
- The first set of terms covers the most central concepts used in the framework.
- The alphabetic structure is suitable for future expansion.
- Further review will be needed after additional templates and examples are created.

**Next Session**

Review the complete glossary against the main framework document and identify any missing or inconsistent terms before starting reusable framework templates.

<br>

## Session 005

**Date**

2026-07-06

**Goal**

Review the Purpose section and draft the Scope section of the AI QA Framework, then continue developing the remaining core sections of the main framework document.

**Completed**

- Drafted the `Purpose` section.
- Drafted the `Scope` section.
- Drafted the `Framework Principles` section.
- Drafted the `AI System Quality Dimensions` section.
- Drafted the `AI QA Lifecycle` section.
- Drafted the `QA Activities by Lifecycle Stage` section.
- Drafted the `Evidence and Artefacts` section.
- Drafted the `Roles and Responsibilities` section.
- Drafted the `Governance and Decision Records` section.
- Drafted the `References and Influences` section.
- Reviewed coherence from the definition through the lifecycle section.
- Adjusted terminology to prefer `AI-based system` for the overall system and `AI component` for AI-related parts of the system.
- Added governance distinction between Architecture Decision Records and QA Decision Records.
- Completed the first full draft of `docs/framework/AI_QA_Framework.md`.

**Key Decisions**

- The AI QA Framework will use `AI-based system` as the preferred term for the complete system.
- The term `AI component` will be used when referring to a specific AI-related part of the system.
- The framework will remain vendor-independent and adaptable to different AI contexts.
- Evidence is treated as central to making quality decisions observable, reviewable and traceable.
- Governance should remain proportional, evidence-based and risk-based.
- References are treated as conceptual influences, not as copied source material.
- The framework does not claim compliance with any standard or regulation unless a dedicated mapping is created separately.

**Review Notes**

- The first full draft is coherent as a foundation document.
- The sequence Definition, Purpose, Scope, Principles, Quality Dimensions, Lifecycle, Activities, Evidence, Roles, Governance and References is logical.
- The document is practical, QA-oriented and independent of specific tools or vendors.
- Some sections are intentionally broad and should be refined after the glossary, templates and examples are created.
- Several glossary terms should be added or refined in `docs/fundamentals/AI_Glossary.md`.

**Next Session**

Review the complete first draft of `docs/framework/AI_QA_Framework.md`, identify glossary terms and begin updating `docs/fundamentals/AI_Glossary.md`.

<br>

## Session 004

**Date**

2026-07-06

**Goal**

Review and refine the working definition of AI Quality Assurance and draft the Purpose section of the main AI QA Framework document.

**Completed**

- Created the daily note for Session 004 under `docs/journal/daily/`.
- Reviewed the working definition of AI Quality Assurance.
- Refined the main framework document structure where needed.
- Drafted the `Purpose` section of `docs/framework/AI_QA_Framework.md`.
- Checked consistency between the AI Quality Assurance definition and the Purpose section.
- Committed the framework document and daily note changes.

**Key Decisions**

- The `Purpose` section should explain why the AI QA Framework exists before expanding into scope, principles or lifecycle activities.
- The framework will continue to be developed incrementally, one section at a time.
- The working definition of AI Quality Assurance remains the conceptual anchor for the next sections.

**Review Notes**

- The Purpose section should remain practical, vendor-independent and aligned with QA practice.
- The wording should avoid sounding like a copied standard or certification definition.
- The Purpose section should support later expansion into Scope, Framework Principles and AI QA Lifecycle.

**Next Session**

Review the `Purpose` section and begin drafting the `Scope` section of `docs/framework/AI_QA_Framework.md`.

<br>

## Session 003

**Date**

2026-07-05

**Goal**

Start the first development session of the AI QA Framework by creating a working definition of AI Quality Assurance.

**Completed**

- Created the first AI QA Framework daily note under `docs/journal/daily/`.
- Confirmed the transition from setup mode to development mode.
- Added the first working definition of AI Quality Assurance to `docs/framework/AI_QA_Framework.md`.
- Created the initial structure of the main framework document.
- Marked the remaining framework sections as `_To be drafted._`.

**Key Decisions**

- The project has moved from setup mode to development mode.
- The first development artefact is a working definition of AI Quality Assurance.
- The definition was added before drafting the Purpose section.
- The main framework document will be developed incrementally, one section at a time.

**Review Notes**

- The definition is practical and vendor-independent.
- The definition is not copied from an external source.
- The definition supports the future Purpose, Scope and Principles sections.
- The framework structure is intentionally incomplete at this stage.

**Next Session**

Review and refine the working definition of AI Quality Assurance, then begin drafting the `Purpose` section of `docs/framework/AI_QA_Framework.md`.

<br>

## Session 002

**Date**

2026-07-04

**Goal**

Review the repository structure and clarify the separation between AI QA Framework project documentation and CT-AI study materials.

**Completed**

- Reviewed the existing repository structure.
- Confirmed that `docs/journal/` should be reserved for AI QA Framework project notes.
- Confirmed that CT-AI study notes should be separated from the framework project journal.
- Created ADR 0001 to document the decision to separate framework and study journals.
- Created the `study-journal/` folder at the repository root.
- Created the following study journal structure:
  - `study-journal/daily/`
  - `study-journal/weekly/`
  - `study-journal/monthly/`
  - `study-journal/study-packs/`
- Moved CT-AI daily notes to `study-journal/daily/`.
- Moved CT-AI study packs to `study-journal/study-packs/`.

**Key Decisions**

- AI QA Framework project notes will remain under `docs/journal/`.
- CT-AI study materials will be maintained under `study-journal/`.
- The decision was formally documented in `docs/adr/0001-separate-framework-and-study-journals.md`.

**Rationale**

Separating project work from certification study materials improves repository clarity and reduces ambiguity as both workstreams evolve.

**Next Session**

Start the first AI QA Framework daily note under `docs/journal/daily/` and begin drafting the `Purpose` section of `docs/framework/AI_QA_Framework.md`.

<br>

## Session 001

**Date**

2026-07-02

**Goal**

Create the initial project structure.

**Completed**

- Repository created.
- Initial folder structure created.
- Milestone v1.0 created.
- Initial Epics created.
- AI QA Framework document created.
- Standards section created.

**Key Decisions**

- Build an original AI Quality Assurance Framework.
- Focus on Quality Engineering instead of only AI Testing.
- Follow a technology-agnostic approach.
- One small step at a time.

**Next Session**

Create the AI QA Glossary.
