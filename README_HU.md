# AI Workflow & Validation Portfólió — Almási Andor

**Szerepkör:** AI munkafolyamat- és validációs elemző  
**Nyilvános kiadás:** v3.3.1  
**Kiadási időbélyeg:** 2026-09-18 20:37:42 CEST

[Teljes magyar Master](portfolio/PORTFOLIO_MASTER_HU.md) · [English landing page](README.md) · [Technikai validációs jegyzék](technical-evidence/VALIDATION_MANIFEST.md)

## Rövid összefoglaló

Ez a repository **Almási Andor bizonyítékalapú AI workflow- és validációs portfólióját** tartalmazza. A munka az emberi döntéshozatal és a fejlett AI-rendszerek közötti gyakorlati működési rétegre összpontosít: strukturált munkafolyamat-tervezésre, LLM-kimenetek validációjára, human-in-the-loop kontrollra, többmodellű keresztellenőrzésre, auditálhatóságra és provenienciára, prototípusértékelésre és komplex projektstrukturálásra.

Az AI-modelleket különálló elemzési, fejlesztési, ellenőrzési és keresztvalidációs eszközökként használom. A központi elv: az AI-kimenet legyen hasznos, de maradjon tesztelhető, megkérdőjelezhető, visszakövethető és emberi döntési kontroll alatt.

## Kiemelt projektek

### RQV v2.7 — Response Quality Validator

Kísérleti Python-alapú keretrendszer meghatározott strukturális, lexikai és viselkedési LLM-tünetek jelzésére.

- Python-forrás: **1938 sor**
- Regressziós ellenőrzés: **115**
- Reprodukált eredmény: **115 PASS / 0 FAIL**
- Python compile: **PASS**
- SHA-256: `ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade`
- Dokumentált tünetosztályok között: `false_certainty`, `intent_drift`, `safety_overgeneralization`, `compression_pressure`.
- A mély szemantikai forrásellenőrzés külön validációs réteg.

### Human-in-the-Loop AI Workflow / AGI-LOOP

Futtatható state-machine és audit referencia-implementáció explicit állapotokkal, ellenőrzési kapukkal, emberi jóváhagyással és hash-kapcsolt auditlánccal. Reprodukált kimenetek: normál befejezés, tamper-detekció, policy HALT és emberi jóváhagyás hiányában REJECT.

### GEH-Core / StarLogic

Verziózott kísérleti kontroll-, audit- és kimenet-összehasonlító komponensek. Három megőrzött GEH-Core változat lefordult és egyenként teljesítette ugyanazt a **13/13 független alapfunkciós próbát**. A StarLogicRecenter v1.0.1 szerzői tesztje **48 PASS / 0 FAIL** eredménnyel reprodukálódott; jelenlegi összehasonlító logikája determinisztikus és elsősorban lexikai.

### MATRIX-SYS

Valós kínai-magyar technológiai együttműködési folyamat strukturálására alkalmazott keretrendszer. A MATRIX-00 a teljes A–J rendszertérképet szervezte, és érdemi írásos partneri felülvizsgálatot kapott. A MATRIX-A, B és C szakaszokat külön aláírt és céges pecséttel ellátott Üzleti Tartalom Megerősítő Levelek támasztják alá. A partnerazonosítók a nyilvános kiadásban nem kerülnek közlésre.

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

## Időbélyegzett kanonikus kiadási fájlok

A repository a GitHub-aliasok mellett az időbélyegzett kanonikus kiadási példányokat is tartalmazza:

- `README_EN_20260918_203742_CEST.md`
- `README_HU_20260918_203742_CEST.md`
- `portfolio/PORTFOLIO_MASTER_EN_v3.3.1_PUBLIC_20260918_203742_CEST.md`
- `portfolio/PORTFOLIO_MASTER_HU_v3.3.1_PUBLIC_20260918_203742_CEST.md`
- `technical-evidence/VALIDATION_MANIFEST_20260918_203742_CEST.md`
- `CHANGELOG_20260918_203742_CEST.md`

Az időbélyeg nélküli fájlnevek GitHub-aliasok az automatikus megjelenítéshez és a stabil belső linkekhez.

## Lehetséges együttműködési területek

AI-workflow elemzés, LLM-output QA, validációs rendszerek, human-in-the-loop folyamatok, multi-model comparison, AI-prototípusok ellenőrzése, failure-mode analysis, dokumentum- és forrásvalidáció, auditálhatóság és proveniencia, műszaki dokumentációelemzés és komplex projektstrukturálás.

Az együttműködés első lépése lehet egy jól körülhatárolt pilotfeladat vagy validációs probléma, amelynek eredménye közvetlenül megítélhető.
