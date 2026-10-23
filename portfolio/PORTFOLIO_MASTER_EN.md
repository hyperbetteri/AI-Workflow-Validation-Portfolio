# ALMÁSI ANDOR

**AI Workflow & Validation Analyst**

- **Logical Object ID:** PORTFOLIO-MASTER-EN
- **Version:** v3.4.1 (Public GitHub Edition)
- **Parent version:** v3.4.0 Public GitHub Edition
- **Release timestamp:** 2026-09-22 00:55:00 CEST
- **Portfolio owner:** Almási Andor
- **Preparation:** AI-assisted, cross-model reviewed, human-reviewed

AI-assisted workflow design · Human-in-the-loop validation ·  
Multi-model review · Auditability and provenance ·  
Prototype evaluation · Failure-mode analysis · Structured systems logic

# PART A — PROFESSIONAL PORTFOLIO

## 1. PROFESSIONAL PROFILE

My work focuses on the practical operating layer between human decision-making
and advanced AI systems.

I use AI models in distinct roles for analysis, development, verification and
cross-model review.

My work repeatedly involves the following areas:

- structured AI workflow design;
- LLM output validation;
- human-in-the-loop control;
- multi-model review;
- failure-mode identification and documentation;
- auditability and provenance;
- practical evaluation of prototypes;
- structured decomposition of complex technical and organisational problems;
- document-based professional work;
- structuring international technology projects.

My central operating principle is:

AI output should be useful, but remain testable, challengeable, traceable and
under human decision control.

The objective is not for AI to provide an answer in every case.

The objective is to be able to determine about the final result:

what it was based on -> how it was produced -> how it was checked ->
where its operating boundaries are -> who makes the final decision.

## 2. PROFESSIONAL DEVELOPMENT

My professional development is problem-driven and self-directed. I build knowledge around concrete technical or operational problems, then test it through implementation, reproduction and correction.

My background includes practical work with electronic and electrical systems and later AI workflows, validation methods and multi-model review.

This portfolio emphasizes demonstrable work, documented evidence, reproducible checks and explicit operating limits.

## 3. SELECTED PROJECT — RQV v2.7
Structured LLM Output Validation and Failure-Symptom Detection Framework

RQV — Response Quality Validator is a Python-based experimental validation
framework for examining defined structural and behavioural characteristics of
LLM outputs.

Current reference: RQV v2.7

Verified technical data:

  Python source:          1938 lines
  Regression checks:     115
  Reproduced result:     115 PASS / 0 FAIL
  Python compile:        PASS
  SHA-256:
  ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade

The v2.7 source documentation itself expects a 115/115 PASS result and also
records the version-development chain.

The system separates several functions, including:

- relevance checking;
- scope control;
- redundancy analysis;
- ASR checks;
- contextual bans;
- structured validation output;
- interference-proxy analysis;
- inverse-reflection logic.

Documented symptom classes:

  compression_pressure
  template_pressure
  safety_overgeneralization
  premature_closure
  branch_suppression
  false_certainty
  logic_path_truncation
  policy_style_intrusion
  intent_drift
  operator_context_loss

These are project-defined heuristic labels used by RQV; they are not presented as an industry-standard taxonomy.

Practical objective:

The basic idea of RQV is that an LLM response should not be evaluated solely
on the basis of its linguistic persuasiveness. The response can be passed
through a separate validation logic that provides structured signals for
further review.

Current operating scope:

In its current form, RQV primarily examines structural, lexical and behavioural
symptoms. When deep semantic source verification is required, that must be
handled as a separate validation layer.

This separation marks the current operating boundary of the system.

In an earlier challenge test, a discrepancy between a 48 V source and a 72 V
answer produced a WARN / manual source-check result, while an irrelevant answer,
false certainty and policy-style intrusion triggered FAIL results.

## 4. SELECTED PROJECT — HUMAN-IN-THE-LOOP AI WORKFLOW
State-Machine and Audit Prototype

Historical internal project name: AGI-LOOP

The project contains a runnable Python reference implementation for an
AI-assisted workflow in which explicit states, review gates and human approval
control progression.

Reproduced state chain:

NONE -> INIT -> INTAKE -> DRAFT -> VERIFY -> REVIEW ->
HITL_GATE -> APPROVED -> EXECUTE -> COMPLETE

Reproduced results:

  NORMAL COMPLETE  ->  True / ok
  TAMPER           ->  hash fail at 4
  POLICY BLOCK     ->  HALT
  NO HUMAN         ->  REJECT

The reference implementation demonstrates:

- explicit state handling;
- hash-linked audit records;
- detection of audit tampering;
- policy blocking;
- human approval gates;
- fail-closed behaviour when human decision is absent.

Development status:

The reproduction identified a concrete control-flow development point. After a
POLICY HALT, later runner calls may generate redundant HALT audit records. The
blocked process does not progress, but simplifying the post-HALT control flow is
a clear next development step.

This project is a good example of my working method:

not hiding an error, but reproducing it, localising it precisely and turning it
into an input for the next version.

## 5. SELECTED PROJECT — GEH-CORE / STARLOGIC
Experimental control, audit and recenter system components

The GEH / StarLogic development branch contains several components aimed at
controllability, auditability, deterministic examination of AI processes and
comparison of multiple outputs.

### 5.1 GEH-Core

GEH-Core is also documented as an ethics-based, multi-model artificial-intelligence validation framework. Its public methodology is built around evidence priority, context and task-scope protection, ABSTAIN and fail-closed operation, human approval and veto authority, versioned event logging, replayable regression testing, and separation of model, agent, permission and operator responsibility.

Its development background is based on approximately five years of practical work with artificial intelligence systems, including more than three years of intensive examination of multi-model LLM operation, deep logical behaviour, context management, failure patterns, model handoffs and human–AI collaborative workflows.

Public documentation: [GEH-Core Public Overview](GEH_CORE_PUBLIC_OVERVIEW_EN.md) · [Research Background](../technical-evidence/GEH_CORE_RESEARCH_CONTEXT_EN.md)

Three preserved implementations were reproduced:

- GEH Core base;
- GEH Core variant 1;
- GEH Core variant 2.

All three compiled successfully and completed the same 13 / 13 independent
basic-function probe.

The examined functions included:

- audit integrity;
- tamper handling;
- recovery / self-heal branches;
- deterministic replay;
- abort / override handling;
- policy control;
- ethical veto;
- KPI and reporting functions.

The reproduction also separated already functioning elements from functions
still under development. Examples of development hooks include:

  _detect_drift
  _detect_unsubstantiated_facts

The documented state distinguishes implemented behaviour from development hooks and keeps the current operating scope explicit.

### 5.2 StarLogicRecenter v1.0.1

StarLogicRecenter is a deterministic lexical/recenter control prototype.

Regression result: 48 PASS / 0 FAIL

In an separate challenge test, an intentionally irrelevant high-confidence
outlier was placed next to two thematically aligned outputs. The system
identified it as the strongest deviation. In a high-confidence conflict, it
returned a REGENERATE / HUMAN_GATE direction.

The reproduction also documents that lexically very different paraphrases may
produce low alignment.

The component can be used for:

- comparing multiple outputs;
- signalling deviations;
- examining recenter logic;
- triggering human escalation.

The current operation is deterministic and primarily lexical; deep semantic
comparison can be connected as a separate layer.

### 5.3 StarLogic BLK5

A preserved mathematical reference implementation from the StarLogic
development branch was also reproduced.

During verification:

- the historical document hash consistency was examined;
- the embedded Python code was extracted;
- syntax was checked;
- the code was executed;
- the documented numerical result sequence was recalculated separately.

The results for iterations 0-8 matched the documented values.

In this portfolio, BLK5 primarily serves as an example of a reproducible
technical-mathematical working method.

## 6. SELECTED PROJECT — MATRIX-SYS
Structured International Technology Project Framework

MATRIX-SYS was created to structure a real Chinese-Hungarian technology
cooperation process.

The purpose of the system was to prevent a multi-party, complex international
project from functioning as one large and ambiguous negotiation package. The
entire cooperation was therefore divided into units that could be separately
reviewed, discussed, modified and approved.

The system: MATRIX-00 + A-J thematic blocks

The project addressed, among other areas:

- cooperation structure;
- professional autonomy and responsibility;
- trust mechanisms;
- organisational structure;
- compensation and startup resources;
- staff selection and integration;
- quality assurance;
- technical validation;
- know-how;
- intellectual property;
- local operations;
- market coordination;
- Chinese-European cultural and business mediation;
- transparency and error prevention.

The structuring logic:

separate review -> separate discussion -> separate modification ->
separate approval -> one coherent overall project

### 6.1 MATRIX-00 — overall system map

MATRIX-00 contained the full A-J system structure together with the proposed
operating, thinking, leadership and decision-making framework for the
cooperation.

The Chinese partner received the material, reviewed it and responded to it
substantively.

In a detailed written response of 1 September 2026, the partner representative
stated that MATRIX-00 had been reviewed and that they fundamentally agreed with
the logic that the operating frameworks should be clarified step by step before
the final contract.

This documents that the framework was reviewed within an active international cooperation process.

MATRIX-SYS was created as a cooperation-structuring system. At the time the
document was prepared, cooperation between the parties was in the negotiation
and preparation phase.

### 6.2 MATRIX-A / B / C — formal work-content confirmations

Separate formal Business Content Confirmation Letters were issued for the
MATRIX project stages.

The original documents:

- are signed;
- bear the company seal;
- explicitly identify the relevant project stage;
- name the issuing company;
- name the authorised representative;
- refer to the work content of MATRIX-SYS MAIN BLOCK MAP v1.0.

Issuer:         Shenzhen Beisi Wujie Technology Co., Ltd.
Representative: Authorised company representative / CEO — identity withheld in the public edition
Position:       CEO (总裁)

Document dates:

  MATRIX-A  —  7 September 2026
  MATRIX-B  —  11 September 2026
  MATRIX-C  —  11 September 2026

Chinese content identifications:

- MATRIX-A: 合作关系中的独立性与信任机制
  (Independence and trust mechanism within the cooperation relationship)
- MATRIX-B: 报酬与启动资源
  (Compensation and startup resources)
- MATRIX-C: 员工招聘与组织融入
  (Employee recruitment and organisational integration)

According to the confirmation letters, the work content was confirmed after
complete document verification, process review and internal final review.


### 6.3 Technical and market advisory role

On 12 September 2026, the partner representative stated in writing that the
Chinese side's original cooperation concept was to involve me in a technical
and market advisory role. She also indicated that they intended to shape their own team
structure and division of work based on understanding my future work plans and
professional ideas.

This correspondence documents a proposed role extending beyond document preparation to technical, organisational and market-facing work.

## 7. WORKING METHOD

### 7.1 Identifying the real problem

Before starting a task, I separate:

- the actual objective;
- assumptions;
- terminology;
- available evidence;
- still-open questions.

### 7.2 Structured problem decomposition

For large problems, I create smaller, separately examinable units. This reduces
the risk that a single incorrect assumption distorts the entire result.

### 7.3 Different roles for multiple AI models

I do not necessarily use different AI models simply as a "second opinion" on
the same question. They may be assigned different roles:

- primary analysis;
- verification;
- critique;
- contradiction search;
- document comparison;
- terminology control;
- translation checking;
- technical cross-checking.

The current multi-model review workflow uses manual, prompt-level coordination; synthesis and the final decision remain with the human operator. Outputs are not merged automatically, and disagreements are retained as review signals.

### 7.4 Execution and reproduction

When a runnable artefact is available, I prefer actual execution over purely
textual evaluation.

Where possible: source -> hash -> compile -> runtime -> challenge test -> result

### 7.5 Error as part of the development process

A negative test result is not something to hide. If a detector does not operate
properly, an edge case slips through or a workflow behaves incorrectly, it
should be documented. A reproducible error is valuable information because it
provides a precise development target.

### 7.6 Evidence and provenance

For important claims, I aim to preserve:

- the original document;
- the source file;
- the version;
- the hash;
- the runtime result;
- the external confirmation;
- the modification chain.

This keeps the result verifiable later.

## 8. WRITTEN, STRUCTURED WORKING FORMAT

I primarily work through written, structured communication. For me, this is not
simply an administrative format, but a quality-assurance method.

With a written assignment:

- the task can be recorded precisely;
- the original requirement can be retrieved later;
- the source material can be checked separately;
- modifications can be tracked;
- the result can be compared directly with the original assignment.

My typical workflow:

written assignment -> source verification -> structured AI-assisted analysis ->
cross-checking and validation -> documented result ->
correction if required

I have also worked in this format in professionally sensitive areas, including:

- legal documentation;
- medical documentation;
- technical materials;
- international business documentation.

I have applied AI-assisted workflows in legal, healthcare, technical and international business documentation contexts. Where relevant, the use of AI tooling was disclosed and the resulting work remained subject to human review.

The essence of the work:

structured input -> controlled AI use -> validation ->
human review -> verifiable output

The quality of delivery is not determined by whether an AI tool participated in
the work, but by whether the delivered result is accurate, verifiable and
usable.

In international projects, I also use AI-assisted multilingual written
communication, terminology checking and cross-model review.

## 9. PROFESSIONAL FOCUS

Primary professional title:

  AI Workflow & Validation Analyst

Core working areas:

- AI-assisted workflow design
- LLM output validation
- human-in-the-loop control
- multi-model cross-checking
- auditability and provenance
- prototype evaluation
- failure-mode analysis
- structured systems thinking
- complex problem decomposition
- evidence-based technical documentation

This title is used here as a concise description of the documented work.

## 10. POTENTIAL COLLABORATION AREAS

Relevant collaboration contexts include organisations that already use AI systems and need more structured verification, documentation or human-control processes.

Potential areas:

- AI workflow analysis;
- LLM output QA;
- validation systems;
- human-in-the-loop processes;
- multi-model comparison;
- evaluation of AI prototypes;
- failure-mode analysis;
- document and source validation;
- auditability and provenance;
- technical documentation analysis;
- complex project structuring;
- structuring international technology cooperation;
- experimental AI governance and control mechanisms.

A first step in cooperation can be a clearly defined pilot task or validation
problem. This provides an opportunity to evaluate the value of the working
method through a concrete result.

# PART B — TECHNICAL EVIDENCE APPENDIX

## 11. REPRODUCTION VERIFICATION METHOD

Some of the technical projects were separately checked within a documented multi-model review workflow.

The objective of reproduction was, where possible, to ensure that:

- the source was actually available;
- the code compiled;
- the test actually ran;
- the documented result could be compared with the reproduced result;
- errors could also be reproduced.

The RQV v2.7 and AGI-LOOP reference implementations were executed in AI-tool environments as part of the documented review workflow; they were not manual local runs by the portfolio owner. The reported results refer to those recorded executions.

## 12. RQV v2.7 — EVIDENCE RECORD

Source:               response_validator_v2_7.py
Source size:          1938 lines
Regression test:      115 checks
Reproduced result:    115 PASS / 0 FAIL
Python compile:       PASS
SHA-256:
ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade

The source documentation itself describes v2.7 as a directly runnable module
and expects a 115/115 regression result.

Challenge test:

- long irrelevant answer                   ->  FAIL
- false certainty                          ->  FAIL
- policy-style intrusion                   ->  FAIL
- 48 V source / 72 V answer                ->  WARN / manual source check

This precisely defines the current operating scope of the system.

## 13. HUMAN-IN-THE-LOOP / AGI-LOOP — EVIDENCE RECORD

The historical reference code was executed after verbatim extraction.

Nominal operation:
  NORMAL COMPLETE  ->  (True, 'ok')

Audit tampering:
  TAMPER           ->  (False, 'hash fail at 4')

Policy stop:
  POLICY_BLOCK     ->  HALT

Absence of human approval:
  NO_HUMAN         ->  REJECT

Using a separate hash checker, modification of an intermediate audit block
was detectable.

The reference demonstrates:

- audit chain;
- tamper detection;
- human gate;
- policy stop;
- fail-closed behaviour.

The redundant HALT records after POLICY HALT are a documented next development
point.

## 14. GEH-CORE — EVIDENCE RECORD

Examined versions:

  GEH Core base
  GEH Core variant 1
  GEH Core variant 2

All three versions completed the same 13 / 13 separate basic-function probe.

Tested functional areas:

- audit integrity;
- tamper handling;
- recovery;
- self-heal branches;
- deterministic replay;
- RS abort / override;
- ISV / ethical veto;
- policy gate;
- KPI reporting.

Some detector hooks present in later versions require further implementation.
This version state is an explicit part of the development documentation.

## 15. STARLOGICRECENTER — EVIDENCE RECORD

Version:              v1.0.1
Regression result:    48 PASS / 0 FAIL

In an separate challenge test, the irrelevant high-confidence outlier was
identified as the strongest deviation.

In a conflict, the system returned a REGENERATE / HUMAN_GATE direction.

Handling lexical and deep semantic similarity can be separated into an
additional validation layer.

## 16. STARLOGIC BLK5 — EVIDENCE RECORD

The Python code embedded in the historical document was:

- recovered;
- syntax-checked;
- executed.

The documented numerical table was verified through separate calculation.

  Iterations: 0-8
  Result:     full match

The BLK5 evidence concerns the reproducibility of the reference implementation
and the verifiability of the documented numerical results.

## 17. MATRIX-SYS — EXTERNAL EVIDENCE RECORD

### 17.1 MATRIX-00

MATRIX-00:

- contained the complete A-J system map;
- reached the Chinese partner;
- underwent substantive partner review;
- received detailed written partner feedback on 1 September 2026;
- the partner side fundamentally agreed with the core logic of step-by-step
  clarification of the operating framework.

Substantive written partner feedback was received regarding the MATRIX-00
system map on 1 September 2026. Separate formal, signed and company-sealed
work-content confirmation documents are available for the subsequent MATRIX-A,
MATRIX-B and MATRIX-C project stages.

The public portfolio treats the different evidence types separately: written
partner review for MATRIX-00, and formal corporate confirmation documents for
stages A/B/C.

### 17.2 MATRIX-A / B / C

Formal, signed and company-sealed Business Content Confirmation Letters are
available for the MATRIX-A/B/C project stages.

All three refer to the work content of MATRIX-SYS MAIN BLOCK MAP v1.0.

Issuer:          Shenzhen Beisi Wujie Technology Co., Ltd.
Representative:  Authorised company representative / CEO — identity withheld in the public edition
Position:        CEO (总裁)

MATRIX-A — 7 September 2026
  Chinese content identification: 合作关系中的独立性与信任机制
  (Independence and trust mechanism within the cooperation relationship)

MATRIX-B — 11 September 2026
  Chinese content identification: 报酬与启动资源
  (Compensation and startup resources)

MATRIX-C — 11 September 2026
  Chinese content identification: 员工招聘与组织融入
  (Employee recruitment and organisational integration)

The work content was confirmed with reference to complete document verification,
process review and internal final review.

## 18. PROFESSIONAL CONTEXT AND AI USE

AI-assisted workflows have been used in legal, healthcare, technical and international business documentation contexts. Where relevant, AI use was disclosed to professional counterparts and the final output remained subject to human review.

The control model used in this portfolio separates source material, model roles, review steps and final human decision authority. Corrections and material changes are documented when they affect the evidence record.

## 19. PORTFOLIO SUMMARY

Almási Andor — AI Workflow & Validation Analyst

My work combines structured AI workflows, human-controlled validation, multi-model review, reproducible technical examination and evidence-based project structuring.

The portfolio includes the following evidence:

- runnable Python artefacts;
- reproduced regression tests;
- source hashes;
- separate challenge tests;
- documented errors and version corrections;
- multi-model review;
- real business project materials;
- external corporate feedback;
- signed and company-sealed confirmation documents.

The essence of my working method:

Structure the complex problem.
Use AI intensively.
Do not accept the result blindly.
Find and document the error.
Preserve the evidence.
Keep the final decision under human control.

The method is applicable to AI, validation and complex systems problems where verifiability, documentation and human decision control are material requirements.

