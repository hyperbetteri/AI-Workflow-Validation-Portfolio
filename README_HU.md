# AI Workflow & Validation Portfólió — Almási Andor

**Szerepkör:** AI munkafolyamat- és validációs elemző  
**Nyilvános kiadás:** v3.4.1  
**Kiadási időbélyeg:** 2026-09-22 00:55:00 CEST

[Teljes magyar Master](portfolio/PORTFOLIO_MASTER_HU.md) · [GEH-Core nyilvános összefoglaló](portfolio/GEH_CORE_PUBLIC_OVERVIEW_HU.md) · [GEH-Core kutatási háttér](technical-evidence/GEH_CORE_RESEARCH_CONTEXT_HU.md) · [English landing page](README.md) · [Technikai validációs jegyzék](technical-evidence/VALIDATION_MANIFEST.md)

## Rövid összefoglaló

Ez a repository **Almási Andor bizonyítékalapú AI workflow- és validációs portfólióját** tartalmazza. A munka az emberi döntéshozatal és a fejlett AI-rendszerek közötti gyakorlati működési rétegre összpontosít: strukturált munkafolyamat-tervezésre, LLM-kimenetek validációjára, human-in-the-loop kontrollra, többmodellű keresztellenőrzésre, auditálhatóságra és provenienciára, prototípusértékelésre és komplex projektstrukturálásra.

Az AI-modelleket elkülönített szerepekben használom elemzésre, fejlesztésre, ellenőrzésre és többmodellű felülvizsgálatra. A központi elv: az AI-kimenet legyen hasznos, de maradjon tesztelhető, megkérdőjelezhető, visszakövethető és emberi döntési kontroll alatt.

## Kiemelt külső bizonyíték — MATRIX-SYS

A MATRIX-SYS projekt nyilvános vizuális bizonyítéka egy valós kínai–magyar technológiai együttműködési folyamatból származik: a kétnyelvű A–J rendszertérkép, valamint a maszkolt MATRIX-A, MATRIX-B és MATRIX-C Üzleti Tartalom Megerősítő Levelek együtt láthatók. A nyilvános bemutatásban a személynév és az aláírás maszkolt; a céges pecsétek láthatók maradnak.

[![MATRIX-SYS nyilvános bizonyíték — rendszertérkép és megerősítő levelek](portfolio/MATRIX_SYS_PUBLIC_EVIDENCE.jpg)](portfolio/MATRIX_SYS_PUBLIC_EVIDENCE.jpg)

**A képre kattintva megnyitható a teljes bizonyítéki nézet.**

## Kiemelt projektek

### RQV v2.7 — Response Quality Validator

Kísérleti Python-alapú keretrendszer meghatározott strukturális, lexikai és viselkedési LLM-tünetek jelzésére.

- Python-forrás: **1938 sor**
- Regressziós ellenőrzés: **115**
- Reprodukált eredmény: **115 PASS / 0 FAIL**
- Python compile: **PASS**
- SHA-256: `ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade`
- A projekt saját heurisztikus címkéi között: `false_certainty`, `intent_drift`, `safety_overgeneralization`, `compression_pressure`; ezek nem iparági standard taxonómiaként szerepelnek.
- A mély szemantikai forrásellenőrzés külön validációs réteg.

### Human-in-the-Loop AI Workflow / AGI-LOOP

Futtatható state-machine és audit referencia-implementáció explicit állapotokkal, ellenőrzési kapukkal, emberi jóváhagyással és hash-kapcsolt auditlánccal. Reprodukált kimenetek: normál befejezés, tamper-detekció, policy HALT és emberi jóváhagyás hiányában REJECT.

### GEH-Core / StarLogic

Verziózott kísérleti kontroll-, audit- és kimenet-összehasonlító komponensek. Három megőrzött GEH-Core változat lefordult és egyenként teljesítette ugyanazt a **13/13 külön alapfunkciós próbát** a dokumentált ellenőrzési folyamatban. A StarLogicRecenter v1.0.1 szerzői tesztje **48 PASS / 0 FAIL** eredménnyel reprodukálódott; jelenlegi összehasonlító logikája determinisztikus és elsősorban lexikai.

A nyilvános GEH-Core módszertan etikai alapú, többmotoros validációs keretrendszert ír le, amelynek fő elemei a bizonyítékelsőbbség, a kontextus- és feladatkörvédelem, az ABSTAIN / fail-closed működés, az emberi jóváhagyás és vétójog, a verziózott eseménynapló és a visszajátszható regressziós vizsgálat. A fejlesztési háttér mintegy öt év mesterségesintelligencia-rendszerekkel végzett gyakorlati munkára, ezen belül több mint három év intenzív, többmotoros LLM-működés és mély logikai viselkedés vizsgálatára épül. [Nyilvános összefoglaló](portfolio/GEH_CORE_PUBLIC_OVERVIEW_HU.md) · [Kutatási háttér](technical-evidence/GEH_CORE_RESEARCH_CONTEXT_HU.md)

### VDA-01 — Vészhelyzeti döntéstámogatás

Kísérleti, axiómaalapú vészhelyzeti döntéstámogató keretrendszer tudatosan védett implementációs határral. A megőrzött validációs állapot **35/35 meghatározott validációs ellenőrzést teljesített**. A forráskód, a részletes tesztvektorok és az implementáció visszafejtését segítő részletek nem részei a nyilvános repositorynak. [Nyilvános összefoglaló](portfolio/VDA01_PUBLIC_OVERVIEW_HU.md)

### MATRIX-SYS

Valós kínai-magyar technológiai együttműködési folyamat strukturálására alkalmazott keretrendszer. A MATRIX-00 a teljes A–J rendszertérképet szervezte, és érdemi írásos partneri felülvizsgálatot kapott. A MATRIX-A, B és C szakaszokat külön aláírt és céges pecséttel ellátott Üzleti Tartalom Megerősítő Levelek támasztják alá. A partnercég név szerint **Shenzhen Beisi Wujie Technology Co., Ltd.**; a felhatalmazott képviselő neve a nyilvános kiadásban továbbra sem kerül közlésre.

## Munkamódszer

1. A valódi probléma, feltételezések, terminológia, bizonyítékok és nyitott kérdések elkülönítése.
2. Komplex problémák külön vizsgálható egységekre bontása.
3. Több AI-rendszer eltérő szerepekben: elemzés, kritika, ellentmondáskeresés, dokumentum-összevetés, validáció.
4. Futtatható artefaktum esetén tényleges reprodukció: `forrás → hash → compile → runtime → ellenpróba → eredmény`.
5. A reprodukálható hiba fejlesztési bemenet, nem eltüntetendő kellemetlenség.
6. Proveniencia megőrzése: forrás, verzió, hash, futási eredmény, külső visszaigazolás, módosítási lánc.

## Bizonyíték és forráshozzáférés

A portfólió technikai eredményei meghatározott, verziózott forrásállapotokhoz és validációs rekordokhoz tartoznak. A nyilvános repository a portfóliót, a bizonyítéki összefoglalókat és a validációs jegyzéket tartalmazza, de nem automatikusan minden alapul szolgáló forrásfájlt vagy nyers üzleti dokumentumot.

A teljes validált forrásfájlok és egyes futtatási artefaktumok nem részei a nyilvános repositorynak. Bemutatásuk lehetősége egyedileg egyeztetett szakmai vagy technikai átvilágítás keretében mérlegelhető.

## Repository-struktúra

```text
AI-Workflow-Validation-Portfolio/
├── README.md
├── README_HU.md
├── portfolio/
│   ├── PORTFOLIO_MASTER_EN.md
│   ├── PORTFOLIO_MASTER_HU.md
│   ├── GEH_CORE_PUBLIC_OVERVIEW_EN.md
│   └── GEH_CORE_PUBLIC_OVERVIEW_HU.md
├── technical-evidence/
│   ├── VALIDATION_MANIFEST.md
│   ├── GEH_CORE_RESEARCH_CONTEXT_EN.md
│   └── GEH_CORE_RESEARCH_CONTEXT_HU.md
└── CHANGELOG.md
```

## Kiadástörténet

A fenti stabil fájlnevek az aktuális nyilvános változatot jelölik. Korábbi időbélyegzett pillanatképek archiválási céllal megmaradhatnak a repositoryban. A kiadási változások a [CHANGELOG.md](CHANGELOG.md) fájlban követhetők.

## Lehetséges együttműködési területek

AI-workflow elemzés, LLM-output QA, validációs rendszerek, human-in-the-loop folyamatok, multi-model comparison, AI-prototípusok ellenőrzése, failure-mode analysis, dokumentum- és forrásvalidáció, auditálhatóság és proveniencia, műszaki dokumentációelemzés és komplex projektstrukturálás.

Az együttműködés első lépése lehet egy jól körülhatárolt pilotfeladat vagy validációs probléma, amelynek eredménye közvetlenül megítélhető.
