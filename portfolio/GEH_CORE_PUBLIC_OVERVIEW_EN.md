# GEH-Core

## Ethics-Based Multi-Model Artificial Intelligence Validation Framework

**Public Professional Overview**

**Version:** 0.2-EN – Pre-Approval Version  
**Date:** September 22, 2026  
**Document timestamp:** 2026-09-22T00:26:01+02:00  
**Author:** Almási Andor Aladár

## 0. Executive Summary

GEH-Core is a logical, ethical, and validation framework designed to make the cooperation of different large language models and agent tools more verifiable, consistent, and human-centered.

The system examines the same task using multiple engines that are, as far as reasonably possible, independent from one another. It separates evidence from model assumptions, protects the operator’s original intent and the scope of the task, detects contradictions, and may withhold execution when uncertainty remains unresolved.

The main elements of the methodology are:

- an internally built ethical and logical foundation;
- multi-model cross-validation;
- evidence priority;
- context and task-scope protection;
- ABSTAIN and fail-closed operation;
- human approval and veto authority;
- versioned event logging;
- replayable regression testing;
- separation of model, agent, permission, and operator responsibility.

The development background of GEH-Core is based on approximately five years of practical work with artificial intelligence systems, including more than three years of intensive work examining multi-model LLM operation, deep logical behavior, context management, failure patterns, model handoffs, and human–AI collaborative workflows.

This work has included continuous observation in real-world workflows, comparison across multiple model families, repeated debugging and regression checking, documented multi-model cross-validation, and practical experience in technical, legal, documentation, and business environments.

The framework is not tied to a single model or vendor.

The internal logical core, detailed rule structure, parameterization, and operational know-how are not part of the public documentation.

## 1. What Is the Project About?

GEH-Core is a logical, ethical, and validation methodology designed to make the cooperation of different large language models and agent tools more verifiable, consistent, and human-centered.

The methodology is not based on an externally imposed prohibition system, but on an ethical and logical foundation built from within.

The system does not automatically treat the answer of a single artificial intelligence model as correct. It compares the outputs of multiple engines that are, as far as reasonably possible, independent from one another, manages discrepancies, and requests human decision-making in defined situations of uncertainty or contradiction.

## 2. What Problem Does It Address?

Many current artificial intelligence systems attempt to manage the risks of already existing capabilities through external rules and execution constraints. By itself, this does not always ensure coherent operation.

GEH-Core applies the reverse approach: ethical, logical, and validation principles are treated not as restrictions added afterward, but as part of the initial operating structure.

The methodology is intended, among other things, to reduce the following problems:

- loss or distortion of operator intent;
- context and task-scope drift;
- weakening of mandatory conditions during summarization or model handoff;
- treatment of incorrect model assumptions as evidence;
- mutually reinforcing or correlated model errors;
- uncontrolled model or agent switching;
- execution under uncertain or contradictory conditions;
- untraceable decision paths;
- critical decisions made without human review;
- workflows that cannot be replayed or reproduced.

## 3. Core Capabilities of the System

### 3.1. Multi-Model Cross-Validation

The same task may be processed by multiple large language models or agent tools that are, as far as reasonably possible, independent from one another.

The system does not use simple majority voting. It examines:

- substantive agreement between outputs;
- the causes of discrepancies;
- the evidence used;
- preservation of context;
- fulfillment of the operator’s objective;
- uncertainty;
- possible error correlation between models.

The output of a single engine does not become a reference solely on the basis of that engine’s own assertion.

### 3.2. Evidence Priority

Verified direct evidence and explicit operator constraints take precedence over unverified model assumptions.

The system distinguishes between:

- directly available data;
- verified external sources;
- facts or constraints defined by the operator;
- model inference;
- unverified assumptions;
- contradictions between different sources.

When evidence conflicts, human review is required.

### 3.3. Context and Task-Scope Protection

The system checks whether a response or proposed execution complies with:

- the original task;
- the operator’s explicit objective;
- the defined scope;
- applicable ethical and data-protection conditions;
- the available evidence;
- the approved operational state.

Arbitrary expansion of the task, reinterpretation of the objective, or disregard of operator-defined constraints is treated as deviation.

### 3.4. ABSTAIN and Fail-Closed Operation

If a contradiction cannot be resolved with sufficient confidence, the system does not force an artificial result.

In such cases it may:

- withhold execution;
- request additional evidence;
- initiate human expert review;
- place the task into a safely closed or pending state.

ABSTAIN means that the system is capable of stating that the available information is insufficient to produce a sufficiently reliable result.

Fail-closed operation means that under uncertain or unverified conditions, the system does not perform an irreversible action.

### 3.5. Auditability

Every decision step is logged and replayable.

The purpose of auditability is to make it possible to determine afterward:

- what input data was available;
- what result each engine produced;
- what discrepancies appeared;
- what evidence or rule supported the decision;
- when human approval, correction, or veto occurred;
- which system and rule version was active at the examined time;
- at which handoff or execution point an error appeared.

### 3.6. Human Decision Authority

The role of the human operator is not an optional addition.

At every critical decision point, the system preserves:

- the possibility of human approval;
- the right to stop execution;
- review of the decision;
- the possibility of correction and veto;
- clear assignment of the responsibility point.

Artificial intelligence may serve a decision-support and validation role, but it does not eliminate human responsibility.

## 4. Ethical and Logical Foundation

The logical foundation of the system includes a thirty-point ethical code and a related objective function.

The ethical code is not a simple prohibition list. It forms a coherent system of principles intended to support:

- protection of human dignity and decision authority;
- reduction of harm;
- separation of evidence from assumption;
- preservation of proportionality;
- data minimization;
- recognition of abuse and logical conflicts;
- verifiable operation;
- separation of responsibility levels.

In the event of incorrect operation, merely selecting another engine is not sufficient: the operational framework must be rebuilt and validated while preserving the ethical and logical foundation.

The detailed ethical code, the objective function, and the associated execution rules are not part of this public documentation.

## 5. Application Areas

The methodology may be applied or examined in the following areas:

- validation of artificial-intelligence-based workflows;
- multi-model quality assurance;
- verification of cooperation between agent tools;
- substantive comparison of complex documentation;
- multi-model analysis of legal and medical documents, with mandatory human expert review;
- technical troubleshooting and decision support;
- research and scientific data handling;
- management of complex multi-party collaborative processes;
- verification of data-protection and permission layers;
- civil-protection and emergency decision support in a separate module under development.

The methodology does not replace expert decisions required in medical, legal, safety-related, or other regulated fields.

## 6. Development Status

GEH-Core is not a finalized standard and is not a completed commercial product.

Its current state is:

- a functioning methodological prototype;
- a multi-model workflow applied to real tasks;
- a system developed through repeated debugging and cross-validation;
- an architecture that is partly automatable and partly dependent on human supervision;
- continuously versioned and reviewed development.

The development background of GEH-Core is based on approximately five years of practical work with artificial intelligence systems, including more than three years of intensive work examining multi-model LLM operation, deep logical behavior, context management, failure patterns, model handoffs, and human–AI collaborative workflows.

This work includes continuous observation in real-world workflows, comparison across multiple model families, repeated debugging and regression checking, documented multi-model cross-validation, and practical experience in technical, legal, documentation, and business environments.

## 7. Development and External Application Background

The methodology did not emerge from laboratory assumptions, but from active technical, documentation, data-management, and multi-model collaborative workflows.

Shenzhen Beisi Wujie Technology Co., Ltd. confirmed the use of the cooperation framework in an official business document.

This constitutes external business application confirmation, not independent technical certification.

Further development is intended to address:

- formalization of the rule structure;
- standardization of logging and version-control requirements;
- separation of model, agent, permission, and operator responsibility;
- development of replayable regression testing;
- making multi-model cross-validation measurable;
- preparation for external professional and security review.

## 8. Research Background and Problems That Remain Open

The detailed research background is provided in a separate document:

[GEH-Core — Research Background and Problems That Remain Open](../technical-evidence/GEH_CORE_RESEARCH_CONTEXT_EN.md)

## 9. What Is Not Made Public?

The public documentation does not contain:

- the internal logical core;
- the complete ethical code and objective function;
- the executable rule structure;
- detailed decision conditions;
- thresholds and weighting parameters;
- internal rule identifiers;
- the complete structured data model;
- operational prompts;
- the specific integration procedure;
- the full structure of validation tests;
- detailed emergency operation;
- know-how that would enable reproduction of the methodology.

The purpose of the public material is to present the essence of the development, its application areas, and its validation principles, not to enable reproduction of the technology.

## 10. Intellectual Property Protection and Publication Status

This public documentation contains only a high-level professional presentation.

The novelty, protectability, ownership relationships, and appropriate intellectual property protection strategy of the development are planned to be examined with the involvement of patent attorney Dr. Dávid Rozsnyói.

Until the preliminary intellectual property review has been completed, no additional technical detail will be made public from which the protected methodology or its operational know-how could be materially reconstructed.

## 11. Limitation Statement

This document:

- is not a technical specification;
- is not a standard;
- is not a conformity certification;
- is not a patent application;
- is not a legal, medical, or safety expert opinion;
- does not grant permission to reproduce the methodology;
- does not contain all information required to operate the complete system.

The document is solely a public professional overview of the development.

## 12. Author and Contact

**Author:** Almási Andor Aladár  
**Contact:** hyperbetteri@gmail.com  
**Document version:** 0.2-EN  
**Date:** September 22, 2026  
**Timestamp:** 2026-09-22T00:26:01+02:00

The content of this document is the intellectual work of Almási Andor Aladár. The internal logical core, executable rule structure, and reproducible operational know-how are not part of the public disclosure.
