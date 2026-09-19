# ALMÁSI ANDOR

**AI Workflow & Validation Analyst**

- **Logical Object ID:** PORTFOLIO-MASTER-EN
- **Version:** v3.3.1 (Public GitHub Edition)
- **Parent version:** v3.3 Public GitHub draft
- **Release timestamp:** 2026-09-18 20:37:42 CEST
- **Portfolio owner:** Almási Andor
- **Preparation:** AI-assisted, cross-validated, human-reviewed

AI-assisted workflow design · Human-in-the-loop validation ·  
Multi-model cross-validation · Auditability and provenance ·  
Prototype evaluation · Failure-mode analysis · Structured systems logic

# CHANGELOG v3.3 → v3.3.1

1. MATRIX-A: restored the explicit Chinese content identification from the original corporate document.
2. MATRIX-SYS: partner and representative information transparently anonymised in the public edition, without fictitious substitutions.
3. MATRIX-00: separated written partner review from the formal A/B/C corporate confirmation evidence.
4. Source access: replaced automatic access language with individually agreed professional/technical review wording.
5. GitHub formatting: cleaned Markdown, section numbering and generation artefacts.
6. Removed unsupported overclaims while retaining version-bound technical metrics and hashes.

# PART A — PROFESSIONAL PORTFOLIO

## 1. PROFESSIONAL PROFILE

My work focuses on the practical operating layer between human decision-making
and advanced AI systems.

I do not use AI models as simple chatbots, but as separate analytical,
development, verification and cross-validation tools.

My work repeatedly involves the following areas:

- structured AI workflow design;
- LLM output validation;
- human-in-the-loop control;
- multi-model cross-validation;
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

## 2. SELF-DIRECTED PROFESSIONAL DEVELOPMENT

My professional development has consistently been self-directed and
problem-driven.

What determined the areas I worked in was not the acquisition of formal
qualifications, but what knowledge was required to solve a technical or
practical problem.

I progressed from practical problem-solving involving electronic and electrical
systems to the study of AI systems, validation processes and multi-model
working methods.

My typical learning process is:

problem -> identify required knowledge -> independent study ->
practical application -> testing -> correction

The emphasis has always been on applicable competence.

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

This makes it possible to treat GEH-Core not merely as a theoretical concept,
but as a versioned, runnable and examinable development system.

### 5.2 StarLogicRecenter v1.0.1

StarLogicRecenter is a deterministic lexical/recenter control prototype.

Regression result: 48 PASS / 0 FAIL

In an independent challenge test, an intentionally irrelevant high-confidence
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
- the documented numerical result sequence was independently recalculated.

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

This is documented external partner confirmation that the complete framework
was not merely an internal concept, but was actually reviewed in a real
international cooperation process.

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

Issuer:         Shenzhen-based technology company — identity withheld in the public edition
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

This is among the strongest external, company-originating evidence in the
portfolio.

### 6.3 Technical and market advisory role

On 12 September 2026, the partner representative stated in writing that the
Chinese side's original cooperation concept was to involve me in a technical
and market advisory role. She also indicated that they intended to shape their own team
structure and division of work based on understanding my future work plans and
professional ideas.

This is an additional external reference showing that the work was not viewed
merely as document preparation, but as part of a broader technical,
organisational and market cooperation.

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

### 7.3 Different roles for multiple AI motors

I do not necessarily use different AI models simply as a "second opinion" on
the same question. They may be assigned different roles:

- primary analysis;
- verification;
- critique;
- contradiction search;
- document comparison;
- terminology control;
- translation checking;
- technical cross-validation.

The current Plus-Claude cross-validation working method operates through manual,
prompt-level coordination; synthesis and the final decision are performed by
the human operator. I do not automatically merge the outputs of the different
motors. The divergence itself is information.

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

Clients and professional counterparts — including lawyers, physicians and
corporate actors — accepted the use of AI-assisted working methods when it was
transparent to them that this was not unchecked chatbot generation.

The essence of the work:

structured input -> controlled AI use -> validation ->
human review -> verifiable output

The quality of delivery is not determined by whether an AI tool participated in
the work, but by whether the delivered result is accurate, verifiable and
usable.

In international projects, I also use AI-assisted multilingual written
communication, terminology checking and cross-validation.

## 9. PROFESSIONAL POSITIONING

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

This title describes the work that is actually supported by the documented
projects, executions and external evidence.

## 10. POTENTIAL COLLABORATION AREAS

I see the strongest fit with organisations that already use AI systems but need
more structured verification, documentation or human-control processes.

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

Some of the technical projects were separately checked during the Plus-Claude
cross-validation process.

The objective of reproduction was, where possible, to ensure that:

- the source was actually available;
- the code compiled;
- the test actually ran;
- the documented result could be compared with the reproduced result;
- errors could also be reproduced.

The reproduction was not performed as Andor's personal manual execution. The
RQV v2.7 and AGI-LOOP reference implementations were executed as part of the
Plus-Claude cross-validation process in an AI-motor execution environment. The
results are documented outputs of the cross-validation process.

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

Using an independent hash checker, modification of an intermediate audit block
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

All three versions completed the same 13 / 13 independent basic-function probe.

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

In an independent challenge test, the irrelevant high-confidence outlier was
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

Issuer:          Shenzhen-based technology company — identity withheld in the public edition
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

## 18. EXTERNAL PROFESSIONAL CONTEXT AND AI USE

A significant experience in my working method is that professional counterparts
do not evaluate the use of AI tools in itself, but the quality and verifiability
of the final result.

I have been transparent before lawyers, physicians and corporate actors that I
use AI systems in the workflow.

The difference compared with unchecked generation is that:

- the task is structured;
- the source is separated;
- the models receive different roles;
- the output can be cross-checked;
- corrections can be documented;
- the final decision remains under human control.

This operating method has proved acceptable and usable in multiple professional
environments.

## 19. PORTFOLIO SUMMARY

Almási Andor — AI Workflow & Validation Analyst

My work combines structured AI workflows, human-controlled validation,
multi-model cross-validation, reproducible technical examination and
evidence-based project structuring.

The portfolio is backed by more than concepts alone.

Available evidence includes:

- runnable Python artefacts;
- reproduced regression tests;
- source hashes;
- independent challenge tests;
- documented errors and version corrections;
- multi-model cross-validation;
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

I can apply this working method to concrete AI, validation or complex systems
problems where verifiability, documentation and human decision control are
important to the client.

# VERSION REGISTER

- **v3.0 — 2026-09-18 — Plus motor:** first complete Hungarian Master.
- **v3.1 — 2026-09-18 — Plus motor:** communication, MATRIX separation and closing revisions.
- **v3.2 — 2026-09-18 — Claude motor:** MATRIX-00 contractual implication clarified; reproduction environment clarified; earlier evidentiary wording for MATRIX-A added.
- **v3.3 — 2026-09-18 — Claude motor:** Public GitHub draft; transparent anonymisation, MATRIX-00 evidence-type separation and source-access wording.
- **v3.3.1 — 2026-09-18 20:37:42 CEST — Plus–Claude cross-validated release:** MATRIX-A explicit Chinese identification corrected; Markdown and numbering errors fixed; overclaims removed; public GitHub edition finalised.
