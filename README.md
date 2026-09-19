# AI Workflow & Validation Portfolio — Almási Andor

**Role:** AI Workflow & Validation Analyst  
**Public release:** v3.3.1  
**Release timestamp:** 2026-09-18 20:37:42 CEST

[Full English Master](portfolio/PORTFOLIO_MASTER_EN.md) · [Magyar belépőoldal](README_HU.md) · [Technical Validation Manifest](technical-evidence/VALIDATION_MANIFEST.md)

## Executive Summary

This repository contains the evidence-backed AI workflow and validation portfolio of **Almási Andor**. The work focuses on the practical operating layer between human decision-making and advanced AI systems: structured workflow design, LLM-output validation, human-in-the-loop control, multi-model cross-checking, auditability and provenance, prototype evaluation, and complex project structuring.

AI models are used as separate analytical, development, verification and cross-validation tools. The central principle is that AI output may be useful, but should remain testable, challengeable, traceable and under human decision control.

## Selected Projects

### RQV v2.7 — Response Quality Validator

Experimental Python-based framework for detecting defined structural, lexical and behavioural symptoms in LLM outputs.

- Python source: **1,938 lines**
- Regression checks: **115**
- Reproduced result: **115 PASS / 0 FAIL**
- Python compile: **PASS**
- SHA-256: `ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade`
- Documented symptom classes include `false_certainty`, `intent_drift`, `safety_overgeneralization` and `compression_pressure`.
- Deep semantic source verification is treated as a separate validation layer.

### Human-in-the-Loop AI Workflow / AGI-LOOP

Runnable state-machine and audit reference implementation with explicit states, review gates, human approval and a hash-linked audit chain. Reproduced outcomes include normal completion, tamper detection, policy HALT and rejection when human approval is absent.

### GEH-Core / StarLogic

Versioned experimental control, audit and output-comparison components. Three preserved GEH-Core variants compiled and each completed the same **13/13 independent basic-function probe**. StarLogicRecenter v1.0.1 reproduced **48 PASS / 0 FAIL** in its author suite; its current comparison logic is deterministic and primarily lexical.

### MATRIX-SYS

A structured framework applied to a real Chinese-Hungarian technology cooperation process. MATRIX-00 organised the overall A–J system map and received substantive written partner review. Separate MATRIX-A, B and C stages are supported by signed and company-sealed Business Content Confirmation Letters. Partner identities are withheld in the public edition.

## Working Method

1. Identify the real problem, assumptions, terminology, evidence and open questions.
2. Decompose complex problems into separately reviewable units.
3. Use multiple AI systems in differentiated roles such as analysis, critique, contradiction search, document comparison and validation.
4. Prefer execution and reproduction when runnable artefacts are available: `source → hash → compile → runtime → challenge test → result`.
5. Treat reproducible errors as development input rather than hiding them.
6. Preserve provenance: source, version, hash, runtime result, external confirmation and modification chain.

## Evidence and Source Access

The technical results in this portfolio belong to specific, versioned source states and validation records. The public repository contains the portfolio, evidence summaries and validation manifest, but not automatically every underlying source file or raw business document.

The complete validated source files and selected runtime artefacts are not part of the public repository. Their presentation may be considered within an individually agreed professional or technical review.

## Repository Structure

```text
almasi-andor-ai-validation-portfolio/
├── README.md
├── README_HU.md
├── portfolio/
│   ├── PORTFOLIO_MASTER_EN.md
│   └── PORTFOLIO_MASTER_HU.md
├── technical-evidence/
│   └── VALIDATION_MANIFEST.md
└── CHANGELOG.md
```

## Timestamped Canonical Release Files

The repository also contains timestamped canonical copies of the release files:

- `README_EN_20260918_203742_CEST.md`
- `README_HU_20260918_203742_CEST.md`
- `portfolio/PORTFOLIO_MASTER_EN_v3.3.1_PUBLIC_20260918_203742_CEST.md`
- `portfolio/PORTFOLIO_MASTER_HU_v3.3.1_PUBLIC_20260918_203742_CEST.md`
- `technical-evidence/VALIDATION_MANIFEST_20260918_203742_CEST.md`
- `CHANGELOG_20260918_203742_CEST.md`

The non-timestamped filenames are GitHub aliases for automatic rendering and stable internal links.

## Collaboration Areas

Potential areas include AI-workflow analysis, LLM-output QA, validation systems, human-in-the-loop processes, multi-model comparison, AI-prototype evaluation, failure-mode analysis, document/source validation, auditability and provenance, technical documentation analysis, and complex project structuring.

A practical first step can be a clearly defined pilot task or validation problem whose result can be reviewed directly.
