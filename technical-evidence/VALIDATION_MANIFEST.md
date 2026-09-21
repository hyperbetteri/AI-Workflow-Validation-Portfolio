# VALIDATION MANIFEST — Almási Andor AI Workflow & Validation Portfolio

**Public release:** v3.4.1  
**Manifest timestamp:** 2026-09-22 00:55:00 CEST

This manifest records version-bound validation artefacts and reproduced results used in the portfolio. Hashes below identify specific archived artefacts; they do not imply that every underlying file is published in this repository. Here, “separate probe” means a separately executed check within the documented review workflow, not an external third-party audit.

## RQV v2.7

- Source file: `response_validator_v2_7.py`
- Source size: **1,938 lines**
- Regression checks: **115**
- Reproduced result: **115 PASS / 0 FAIL**
- Python compile: **PASS**
- Source SHA-256: `ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade`
- Challenge behaviour: irrelevant answer → FAIL; false certainty → FAIL; policy-style intrusion → FAIL; 48 V source / 72 V answer → WARN / manual source check.

## Human-in-the-Loop / AGI-LOOP

- Nominal reproduced result: `(True, 'ok')`
- Tamper result: `(False, 'hash fail at 4')`
- Policy block: `HALT`
- Missing human approval: `REJECT`
- Nominal-run output SHA-256: `16690212cf61670f2fabfe12a2e7179e139943cd42a9afe3799da7c961205909`
- Separate-probe output SHA-256: `0f49b370711ca2e6247a39bda3d689d964756d626f49adfd9752466ee6ecc2ae`
- Separate-probe source SHA-256: `5267b868d8cd578a043df2e09753e8b6348976b11ac39141ed9fe6c42fb9a97a`

## GEH-Core

- Public methodology overview: [EN](../portfolio/GEH_CORE_PUBLIC_OVERVIEW_EN.md) · [HU](../portfolio/GEH_CORE_PUBLIC_OVERVIEW_HU.md)
- Research context: [EN](GEH_CORE_RESEARCH_CONTEXT_EN.md) · [HU](GEH_CORE_RESEARCH_CONTEXT_HU.md)
- Public methodology document version: **0.2** — dated **2026-09-22**
- Separate probe source SHA-256: `4fda8a875ae1020da7b8e73850736084d2b99f5dac8b746ae4cc6a5912286084`
- Base variant output: **13/13** — SHA-256 `b93ce96642fa79bbfb4e699fe85eeefdcdae236335b543572de5d81a14361d6c`
- Variant 1 output: **13/13** — SHA-256 `1d48b7be3f08696568d4ef127ae98bb411afc32cd76121c5014b6ddfee711183`
- Variant 2 output: **13/13** — SHA-256 `37860f6e1398afa7854f53d31c0a750414a002db01565ace39bc6dda5f0e13bb`

## StarLogicRecenter v1.0.1

- Author suite: **48 PASS / 0 FAIL**
- Author-suite output SHA-256: `9d8e90b4691002c5bbbaf44f2843b613b331ef7410dfb85a0afdad654b951e64`
- Separate-probe output SHA-256: `ced4021cba7d35a8de0b8099a45aaf2799f0312b502a09cabd813b6c07f38fae`
- Separate-probe source SHA-256: `d1b4ea54300a9bba3a75176e102d44e120c5b42c2bdcb255593752247aa2b619`
- Current scope: deterministic and primarily lexical; deep semantic comparison is a separate layer.

## StarLogic BLK5

- Historical DOCX SHA-256: `abb442c9cf5f7653f26c28035bd63a011bb4055d98b8a73b1f6e0b2602db0e78`
- Extracted Python SHA-256: `cff2118a1df8f3add6443fd2b443a548909bc0ecdcea6cbf37c41afa17623961`
- Built-in numeric-run output SHA-256: `2c53624d92a17e7f561439caf25fbaf69460110117f0092da2c494edcc6a545c`
- Separate drift-sweep output SHA-256: `b0ccccffa4eb17794823fb88a662af164b50e5ecebfa8844a2e908a9961d64ba`
- Separate drift-probe source SHA-256: `9368a29fecf22be8d9bba96d223e816b673055df683498a39f5d1d1c1e361b2a`
- Numeric verification: iterations **0–8**, full match with documented values.

## MATRIX-SYS External Evidence

- MATRIX-00: substantive written partner review received **2026-09-01**.
- MATRIX-A Business Content Confirmation Letter: **2026-09-07**, signed and company-sealed.
- MATRIX-B Business Content Confirmation Letter: **2026-09-11**, signed and company-sealed.
- MATRIX-C Business Content Confirmation Letter: **2026-09-11**, signed and company-sealed.
- MATRIX-A Chinese content identification: `合作关系中的独立性与信任机制`.
- MATRIX-B Chinese content identification: `报酬与启动资源`.
- MATRIX-C Chinese content identification: `员工招聘与组织融入`.
- Partner company: **Shenzhen Beisi Wujie Technology Co., Ltd.** The authorised representative’s name remains omitted in the public edition.

## Public-Repository Scope

The public repository contains portfolio documents and validation summaries. Complete source files, raw runtime material and confidential business evidence are not automatically public. Their presentation may be considered within an individually agreed professional or technical review.
