# ALMÁSI ANDOR

**AI Workflow & Validation Analyst**  
**AI munkafolyamat- és validációs elemző**

- **Logical Object ID:** PORTFOLIO-MASTER-HU
- **Version:** v3.3.1 (Public GitHub Edition)
- **Parent version:** v3.3 Public GitHub draft
- **Release timestamp:** 2026-09-18 20:37:42 CEST
- **Portfolio owner:** Almási Andor
- **Preparation:** AI-assisted, cross-validated, human-reviewed

AI-támogatott munkafolyamat-tervezés · Human-in-the-loop validáció ·  
Többmodellű keresztellenőrzés · Auditálhatóság és proveniencia ·  
Prototípusértékelés · Hibamód-elemzés · Strukturált rendszerlogika

# VÁLTOZÁSNAPLÓ v3.3 → v3.3.1

1. MATRIX-A: az explicit kínai tartalmi megjelölés helyreállítva az eredeti vállalati dokumentum alapján.
2. MATRIX-SYS: a partner és képviselő nyilvános adatai transzparensen anonimizálva; fiktív adatok nélkül.
3. MATRIX-00: az írásos partneri felülvizsgálat és az A/B/C formális megerősítő dokumentumok bizonyítéktípusa elkülönítve.
4. Forráskód-hozzáférés: automatikus hozzáférési ígéret helyett egyedi szakmai/technikai egyeztetés.
5. GitHub-formázás: teljes Markdown- és fejezetszámozási tisztítás; generálási maradványok eltávolítva.
6. Nyelvi és szakmai túlállítások eltávolítva; a technikai sarokszámok konkrét verziókhoz kötve maradnak.

# A. RÉSZ — SZAKMAI PORTFÓLIÓ

## 1. SZAKMAI PROFIL

Munkám az emberi döntéshozatal és a fejlett AI-rendszerek közötti
gyakorlati működési rétegre összpontosít.

Az AI-modelleket nem egyszerű chatbotként használom, hanem különálló
elemzési, fejlesztési, ellenőrzési és keresztvalidációs eszközökként.

Munkáimban visszatérően az alábbi területekkel foglalkozom:

- strukturált AI-munkafolyamatok kialakítása;
- LLM-kimenetek validációja;
- human-in-the-loop kontroll;
- többmodellű keresztellenőrzés;
- hibamódok felismerése és dokumentálása;
- auditálhatóság és proveniencia;
- prototípusok gyakorlati vizsgálata;
- összetett műszaki és szervezeti problémák strukturált felbontása;
- dokumentumalapú szakmai munka;
- nemzetközi technológiai projektek strukturálása.

A központi működési elvem:

Az AI-kimenet legyen hasznos, de maradjon tesztelhető, megkérdőjelezhető,
visszakövethető és emberi döntési kontroll alatt.

Nem az a célom, hogy az AI minden esetben választ adjon.

A cél az, hogy az elkészült eredményről meg lehessen állapítani:

miből készült -> hogyan készült -> hogyan ellenőriztük ->
hol vannak a működési határai -> ki hozza meg a végső döntést.

## 2. ÖNIRÁNYÍTOTT SZAKMAI FEJLŐDÉS

Szakmai fejlődésem következetesen önirányított és problémavezérelt volt.

Nem képesítések megszerzése határozta meg, hogy milyen területtel foglalkozom,
hanem az, hogy egy műszaki vagy gyakorlati probléma megoldásához milyen
tudásra volt szükség.

A műszaki-elektronikai és villamos rendszerekkel kapcsolatos gyakorlati
problémamegoldástól jutottam el az AI-rendszerek, validációs folyamatok
és többmodellű munkamódszerek vizsgálatáig.

Jellemző tanulási módszerem:

probléma -> szükséges tudás azonosítása -> önálló feldolgozás ->
gyakorlati alkalmazás -> tesztelés -> korrekció

A hangsúly mindig az alkalmazható kompetencián volt.

## 3. KIEMELT PROJEKT — RQV v2.7
Structured LLM Output Validation and Failure-Symptom Detection Framework

Az RQV — Response Quality Validator Python-alapú kísérleti validációs
keretrendszer LLM-kimenetek meghatározott strukturális és viselkedési
jellemzőinek vizsgálatára.

Aktuális referencia: RQV v2.7

Ellenőrzött technikai adatok:

  Python-forrás:          1938 sor
  Regressziós ellenőrzés: 115
  Reprodukált eredmény:   115 PASS / 0 FAIL
  Python compile:         PASS
  SHA-256:
  ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade

A v2.7 forrás saját dokumentációja 115/115 PASS eredményt vár, és a verzió
fejlődési láncát is rögzíti.

A rendszer különálló funkciókra bontva kezeli többek között:

- relevanciaellenőrzést;
- scope-kontrollt;
- redundanciaelemzést;
- ASR-ellenőrzéseket;
- kontextuális tiltásokat;
- strukturált validációs eredményt;
- interference-proxy elemzést;
- inverse-reflection logikát.

Dokumentált tünetosztályok:

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

Gyakorlati cél:

Az RQV alapgondolata, hogy egy LLM-választ ne kizárólag a nyelvi
meggyőzőereje alapján értékeljünk. A válasz külön validációs logikán
futtatható át, amely strukturált jelzéseket ad további ellenőrzéshez.

Jelenlegi működési kör:

Az RQV jelenlegi formájában elsősorban strukturális, lexikai és viselkedési
tüneteket vizsgál. Amikor mély szemantikai forrásellenőrzés szükséges, azt
külön validációs rétegként kell kezelni.

Ez a szétválasztás a rendszer jelenlegi működési határát jelöli.

Korábbi ellenpróba során egy 48 V-os forrás és egy 72 V-os válasz eltérése
WARN / manuális forrásellenőrzési eredményt adott, miközben irreleváns válasz,
hamis bizonyosság és policy-stílusú beavatkozás FAIL eredményt váltott ki.

## 4. KIEMELT PROJEKT — HUMAN-IN-THE-LOOP AI WORKFLOW
State-Machine and Audit Prototype

Történeti belső projektnév: AGI-LOOP

A projekt futtatható Python referencia-implementációt tartalmaz olyan
AI-támogatott munkafolyamathoz, amelyben explicit állapotok, ellenőrzési
kapuk és emberi jóváhagyás szabályozza a továbblépést.

Reprodukált állapotlánc:

NONE -> INIT -> INTAKE -> DRAFT -> VERIFY -> REVIEW ->
HITL_GATE -> APPROVED -> EXECUTE -> COMPLETE

Reprodukált eredmények:

  NORMAL COMPLETE  ->  True / ok
  TAMPER           ->  hash fail at 4
  POLICY BLOCK     ->  HALT
  NO HUMAN         ->  REJECT

A referencia-implementáció demonstrálja:

- explicit állapotkezelést;
- hash-kapcsolt auditbejegyzéseket;
- auditmanipuláció felismerését;
- policy-blokkolást;
- emberi jóváhagyási kaput;
- emberi döntés hiányában fail-closed működést.

Fejlesztési állapot:

A reprodukció során egy konkrét kontrollfolyam-fejlesztési pontot
azonosítottunk. POLICY HALT után későbbi runner-hívások redundáns HALT
auditbejegyzéseket generálhatnak. A tiltott folyamat nem jut tovább, de
a HALT utáni kontrollfolyam egyszerűsítése egyértelmű következő fejlesztési
lépés.

Ez a projekt jól példázza a munkamódszeremet:

nem elrejteni a hibát, hanem reprodukálni, pontosan lokalizálni és
a következő verzió bemenetévé tenni.

## 5. KIEMELT PROJEKT — GEH-CORE / STARLOGIC
Kísérleti kontroll-, audit- és recenter rendszerkomponensek

A GEH / StarLogic fejlesztési ág több olyan komponenst tartalmaz, amelyek
az AI-folyamatok kontrollálhatóságát, auditálhatóságát, determinisztikus
vizsgálatát és több kimenet összehasonlítását célozzák.

### 5.1 GEH-Core

Három megőrzött implementáció került reprodukálásra:

- GEH Core base;
- GEH Core variant 1;
- GEH Core variant 2.

Mindhárom sikeresen lefordult és ugyanazon 13 / 13 független alapfunkciós
próbát teljesítette.

A vizsgált funkciók között szerepelt:

- auditintegritás;
- tamper-kezelés;
- recovery / self-heal ágak;
- determinisztikus replay;
- abort / override kezelés;
- policy-kontroll;
- etikai veto;
- KPI- és riportfunkciók.

A reprodukció egyúttal elkülönítette a már működő elemeket a még fejlesztés
alatt álló funkcióktól. Ilyen fejlesztési hook például:

  _detect_drift
  _detect_unsubstantiated_facts

Ez lehetővé teszi, hogy a GEH-Core-t ne pusztán elméleti elképzelésként,
hanem verziózott, futtatható és vizsgálható fejlesztési rendszerként kezeljük.

### 5.2 StarLogicRecenter v1.0.1

A StarLogicRecenter determinisztikus lexikai/recenter kontrollprototípus.

Regressziós eredmény: 48 PASS / 0 FAIL

Független challenge-próbában két tematikailag összetartozó kimenet mellé
szándékosan irreleváns, magas bizonyosságú outlier került. A rendszer ezt
azonosította a legerősebb eltérésként. Magas bizonyosságú konfliktus esetén
REGENERATE / HUMAN_GATE irányt adott.

A reprodukció azt is dokumentálja, hogy lexikailag erősen eltérő
parafrázisoknál alacsony alignment jelentkezhet.

A komponens használható:

- több kimenet összehasonlítására;
- eltérések jelzésére;
- recenter logika vizsgálatára;
- emberi eszkaláció kiváltására.

A jelenlegi működés determinisztikus és elsősorban lexikai; mély szemantikai
összehasonlítás külön rétegként kapcsolható hozzá.

### 5.3 StarLogic BLK5

A StarLogic fejlesztési ágból egy megőrzött matematikai
referencia-implementációt is reprodukáltunk.

Az ellenőrzés során:

- a történeti dokumentum hash-azonosságát vizsgáltuk;
- a beágyazott Python-kódot kiemeltük;
- szintaktikailag ellenőriztük;
- lefuttattuk;
- a dokumentált numerikus eredménysort függetlenül újraszámítottuk.

A 0-8 iteráció eredményei egyeztek a dokumentált értékekkel.

A BLK5 ebben a portfólióban elsősorban a reprodukálható műszaki-matematikai
munkamódszer példája.

## 6. KIEMELT PROJEKT — MATRIX-SYS
Strukturált nemzetközi technológiai projektkeret

A MATRIX-SYS egy valós kínai-magyar technológiai együttműködési folyamat
strukturálására készült.

A rendszer célja az volt, hogy egy sokszereplős, összetett nemzetközi projekt
ne egyetlen nagy és többértelmű tárgyalási csomagként működjön. Ezért a teljes
együttműködést külön-külön ellenőrizhető, megvitatható, módosítható és
jóváhagyható egységekre bontottam.

A rendszer: MATRIX-00 + A-J tematikus blokkok

A projekt többek között az alábbi területeket kezelte:

- együttműködési struktúra;
- szakmai autonómia és felelősség;
- bizalmi mechanizmusok;
- szervezeti felépítés;
- kompenzáció és induló erőforrások;
- munkatársak kiválasztása és integrációja;
- minőségbiztosítás;
- műszaki validáció;
- know-how;
- szellemi tulajdon;
- helyi működés;
- piaci koordináció;
- kínai-európai kulturális és üzleti közvetítés;
- transzparencia és hibamegelőzés.

A strukturálási logika:

külön ellenőrzés -> külön egyeztetés -> külön módosítás ->
külön jóváhagyás -> egységes teljes projekt

### 6.1 MATRIX-00 — teljes rendszertérkép

A MATRIX-00 tartalmazta a teljes A-J rendszerstruktúrát, valamint az
együttműködéshez javasolt működési, gondolkodási, vezetési és döntési keretet.

A kínai partner az anyagot megkapta, megvizsgálta és érdemben reagált rá.

A partner képviselője 2026. szeptember 1-jei részletes írásos válaszában jelezte,
hogy a MATRIX-00-t áttanulmányozta, és alapvetően egyetértettek azzal a logikával,
hogy a működési kereteket a végleges szerződés előtt lépésről lépésre kell
tisztázni.

Ez dokumentált külső partneri visszaigazolása annak, hogy a teljes
keretrendszer nem pusztán belső koncepció volt, hanem valós nemzetközi
együttműködési folyamatban ténylegesen felülvizsgálatra került.

A MATRIX-SYS együttműködés-strukturáló rendszerként készült. A dokumentum
elkészítésekor a felek közötti együttműködés tárgyalási és előkészítési
fázisban volt.

### 6.2 MATRIX-A / B / C — formális munkatartalom-megerősítések

A MATRIX projektszakaszokhoz külön formális Üzleti Tartalom Megerősítő
Levelek készültek.

Az eredeti dokumentumok:

- aláírtak;
- céges pecséttel ellátottak;
- az adott projektszakaszt explicit módon azonosítják;
- megnevezik a kibocsátó társaságot;
- megnevezik a felhatalmazott képviselőt;
- a MATRIX-SYS FŐ BLOKK TÉRKÉP v1.0 munkatartalmára hivatkoznak.

Kibocsátó:     Shenzhen-i technológiai vállalat — a vállalat neve a nyilvános változatban nem kerül közlésre
Képviselő:     Felhatalmazott vállalati képviselő / CEO — neve a nyilvános változatban nem kerül közlésre
Beosztás:      CEO (总裁)

Dokumentumdátumok:

  MATRIX-A  —  2026. szeptember 7.
  MATRIX-B  —  2026. szeptember 11.
  MATRIX-C  —  2026. szeptember 11.

Kínai tartalmi megjelölések:

- MATRIX-A: 合作关系中的独立性与信任机制
  (Az együttműködési kapcsolat függetlenségi és bizalmi mechanizmusa)
- MATRIX-B: 报酬与启动资源
  (Kompenzáció és induló erőforrások)
- MATRIX-C: 员工招聘与组织融入
  (Munkatársak toborzása és szervezeti integrációja)

A megerősítő levelek szövege szerint a munkatartalmat teljes
dokumentum-ellenőrzés, folyamat-felülvizsgálat és belső végső ellenőrzés
után erősítették meg.

Ez a portfólió legerősebb külső, vállalati eredetű bizonyítékai közé tartozik.

### 6.3 Technikai és piaci tanácsadói szerep

2026. szeptember 12-én a partner képviselője írásban közölte, hogy a kínai fél eredeti
együttműködési elképzelése szerint technikai és piaci tanácsadói szerepben
kívántak bevonni. Azt is jelezte, hogy a jövőbeli munkaterveim és szakmai
elképzeléseim megismerése alapján kívánják alakítani saját csapatstruktúrájukat
és munkamegosztásukat.

Ez további külső referencia arra, hogy a munkát nem egyszerű
dokumentumkészítésként értékelték, hanem egy szélesebb technikai, szervezeti
és piaci együttműködés részeként.

## 7. MUNKAMÓDSZER

### 7.1 A valódi probléma azonosítása

A feladat megkezdése előtt szétválasztom:

- a tényleges célt;
- a feltételezéseket;
- a terminológiát;
- a rendelkezésre álló bizonyítékokat;
- a még nyitott kérdéseket.

### 7.2 Strukturált problémabontás

Nagy problémák esetén kisebb, külön vizsgálható egységeket hozok létre.
Ez csökkenti annak kockázatát, hogy egyetlen hibás feltételezés az egész
eredményt eltorzítsa.

### 7.3 Több AI-motor eltérő szerepekben

A különböző AI-modelleket nem feltétlenül ugyanarra a kérdésre adott
"második véleményként" használom. Külön szerepeket is kaphatnak:

- elsődleges elemzés;
- ellenőrzés;
- kritika;
- ellentmondáskeresés;
- dokumentum-összevetés;
- terminológiai kontroll;
- fordításellenőrzés;
- technikai keresztvalidáció.

A jelenlegi Plus-Claude keresztvalidációs munkamódszer kézi, promptszintű
koordinációval működik; a szintézist és a végső döntést az emberi operátor
végzi. A különböző motorok válaszait nem egyesítem automatikusan.
Az eltérés maga is információ.

### 7.4 Futtatás és reprodukció

Ha futtatható artefaktum áll rendelkezésre, előnyben részesítem a tényleges
futtatást a pusztán szöveges értékeléssel szemben.

Ahol lehetséges: forrás -> hash -> compile -> runtime -> ellenpróba -> eredmény

### 7.5 A hiba a fejlesztési folyamat része

Egy negatív teszteredmény nem eltüntetendő kellemetlenség. Ha egy detektor
nem működik megfelelően, egy edge case átcsúszik vagy egy workflow hibásan
viselkedik, azt dokumentálni kell. A reprodukálható hiba értékes információ,
mert pontos fejlesztési célt ad.

### 7.6 Bizonyíték és proveniencia

Fontos állítások esetén igyekszem megtartani:

- az eredeti dokumentumot;
- a forrásfájlt;
- a verziót;
- a hash-t;
- a futási eredményt;
- a külső visszaigazolást;
- a módosítási láncot.

Így az eredmény később is ellenőrizhető.

## 8. ÍRÁSOS, STRUKTURÁLT MUNKAFORMA

Elsősorban írásos, strukturált kommunikációval dolgozom. Ez számomra nem
egyszerű adminisztratív forma, hanem minőségbiztosítási módszer.

Írásos megbízásnál:

- a feladat pontosan rögzíthető;
- az eredeti követelmény később visszakereshető;
- a forrásanyag külön ellenőrizhető;
- a módosítások nyomon követhetők;
- az eredmény közvetlenül összevethető az eredeti megbízással.

Jellemző munkafolyamat:

írásos megbízás -> forrásellenőrzés -> strukturált AI-támogatott elemzés ->
keresztellenőrzés és validáció -> dokumentált eredmény ->
szükség esetén korrekció

Szakmailag érzékeny területeken is dolgoztam ilyen formában, többek között:

- jogi dokumentációval;
- orvosi dokumentációval;
- műszaki anyagokkal;
- nemzetközi üzleti dokumentumokkal.

Megbízók és szakmai partnerek — köztük ügyvédek, orvosok és vállalati
szereplők — elfogadták az AI-támogatott munkamódszer alkalmazását, amikor
átlátható volt számukra, hogy nem ellenőrizetlen chatbot-generálás történik.

A munka lényege:

strukturált input -> kontrollált AI-használat -> validáció ->
emberi ellenőrzés -> ellenőrizhető output

A teljesítés minőségét nem az határozza meg, hogy AI-eszköz részt vett-e
a munkában, hanem az, hogy a leadott eredmény pontos, ellenőrizhető és
használható-e.

Nemzetközi projektekben AI-támogatott többnyelvű írásos kommunikációt,
terminológiai ellenőrzést és keresztvalidációt is alkalmazok.

## 9. SZAKMAI POZICIONÁLÁS

Elsődleges szakmai megnevezés:

  AI Workflow & Validation Analyst
  AI munkafolyamat- és validációs elemző

Fő működési területek:

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

Ez a megnevezés azt a munkát írja le, amelyet a dokumentált projektek,
futtatások és külső bizonyítékok ténylegesen alátámasztanak.

## 10. LEHETSÉGES EGYÜTTMŰKÖDÉSI TERÜLETEK

A legerősebb illeszkedést olyan szervezeteknél látom, amelyek már használnak
AI-rendszereket, de szükségük van strukturáltabb ellenőrzési, dokumentációs
vagy emberi kontrollfolyamatokra.

Lehetséges területek:

- AI-workflow elemzés;
- LLM-output QA;
- validációs rendszerek;
- human-in-the-loop folyamatok;
- multi-model comparison;
- AI-prototípusok ellenőrzése;
- failure-mode analysis;
- dokumentum- és forrásvalidáció;
- auditálhatóság és proveniencia;
- műszaki dokumentációelemzés;
- komplex projektstrukturálás;
- nemzetközi technológiai együttműködések strukturálása;
- kísérleti AI-governance és kontrollmechanizmusok.

Az együttműködés első lépése lehet egy jól körülhatárolt pilotfeladat
vagy validációs probléma. Ez lehetőséget ad arra, hogy a munkamódszer
értéke konkrét eredményen keresztül legyen megítélhető.

# B. RÉSZ — TECHNIKAI BIZONYÍTÉKI FÜGGELÉK

## 11. A REPRODUKCIÓS ELLENŐRZÉS MÓDJA

A technikai projektek egy részét a Plus-Claude keresztvalidációs folyamat
során külön ellenőriztük.

A reprodukció célja az volt, hogy ahol lehetséges:

- a forrás ténylegesen rendelkezésre álljon;
- a kód leforduljon;
- a teszt ténylegesen lefusson;
- a dokumentált eredmény és a reprodukált eredmény összevethető legyen;
- a hibák is reprodukálhatók legyenek.

A reprodukció nem Andor személyes kézi futtatásaként történt. Az RQV v2.7
és az AGI-LOOP referencia-implementáció futtatása a Plus-Claude
keresztvalidációs folyamat részeként, AI-motor végrehajtási környezetben
valósult meg. Az eredmények a keresztvalidáció dokumentált kimenetei.

### Forráskód és validációs artefaktumok hozzáférhetősége

A jelen portfólióban szereplő technikai eredmények meghatározott, verziózott
forrásállapotokhoz és validációs rekordokhoz tartoznak.

A teljes validált forrásfájlok és egyes futtatási artefaktumok nem részei a
nyilvános repositorynak. Bemutatásuk lehetősége egyedileg egyeztetett szakmai
vagy technikai átvilágítás keretében mérlegelhető.

## 12. RQV v2.7 — BIZONYÍTÉKI REKORD

Forrás:               response_validator_v2_7.py
Forrásméret:          1938 sor
Regressziós teszt:    115 ellenőrzés
Reprodukált eredmény: 115 PASS / 0 FAIL
Python compile:       PASS
SHA-256:
ce7401ce03f3c064915c8c7465e426b613be0b13cbc22b95212f548984706ade

A forrás saját dokumentációja a v2.7-et közvetlenül futtatható modulnak írja
le, és 115/115 regressziós eredményt vár.

Ellenpróba:

- hosszú irreleváns válasz              ->  FAIL
- hamis bizonyosság                     ->  FAIL
- policy-stílusú beavatkozás            ->  FAIL
- 48 V-os forrás / 72 V-os válasz       ->  WARN / manuális forrásellenőrzés

Ez pontosan meghatározza a rendszer jelenlegi működési körét.

## 13. HUMAN-IN-THE-LOOP / AGI-LOOP — BIZONYÍTÉKI REKORD

A történeti referencia-kód verbatim kiemelés után futtatásra került.

Nominális működés:
  NORMAL COMPLETE  ->  (True, 'ok')

Auditmanipuláció:
  TAMPER           ->  (False, 'hash fail at 4')

Policy stop:
  POLICY_BLOCK     ->  HALT

Emberi jóváhagyás hiánya:
  NO_HUMAN         ->  REJECT

Független hash-ellenőrzővel egy köztes auditblokk módosítása
detektálható volt.

A referencia demonstrálja:

- auditláncot;
- tamper detectiont;
- human gate-et;
- policy stopot;
- fail-closed működést.

A POLICY HALT utáni redundáns HALT rekordok dokumentált következő
fejlesztési pontot jelentenek.

## 14. GEH-CORE — BIZONYÍTÉKI REKORD

Vizsgált változatok:

  GEH Core base
  GEH Core variant 1
  GEH Core variant 2

Mindhárom változat ugyanazon 13 / 13 független alapfunkciós próbát
teljesítette.

Tesztelt funkcióterületek:

- audit integrity;
- tamper handling;
- recovery;
- self-heal ágak;
- deterministic replay;
- RS abort / override;
- ISV / ethical veto;
- policy gate;
- KPI reporting.

A későbbi verziókban jelen lévő egyes detektorhookok további implementációt
igényelnek. Ez a verzióállapot a fejlesztési dokumentáció explicit része.

## 15. STARLOGICRECENTER — BIZONYÍTÉKI REKORD

Verzió:               v1.0.1
Regressziós eredmény: 48 PASS / 0 FAIL

Független challenge-tesztben az irreleváns, magas bizonyosságú outlier
a legerősebb eltérésként került azonosításra.

Konfliktus esetén a rendszer REGENERATE / HUMAN_GATE irányt adott.

A lexikai és mély szemantikai hasonlóság kezelése elkülöníthető
további validációs rétegként.

## 16. STARLOGIC BLK5 — BIZONYÍTÉKI REKORD

A történeti dokumentumba ágyazott Python-kód:

- visszanyerésre került;
- szintaktikailag ellenőrzött;
- futtatásra került.

A dokumentált numerikus táblát külön számítással ellenőriztük.

  Iterációk: 0-8
  Eredmény:  teljes egyezés

A BLK5 bizonyítéka a referencia-implementáció reprodukálhatóságára és a
dokumentált numerikus eredmények ellenőrizhetőségére vonatkozik.

## 17. MATRIX-SYS — KÜLSŐ BIZONYÍTÉKI REKORD

### 17.1 MATRIX-00

A MATRIX-00:

- a teljes A-J rendszertérképet tartalmazta;
- a kínai partnerhez eljutott;
- érdemi partneri felülvizsgálaton esett át;
- 2026. szeptember 1-jén részletes írásos partneri visszajelzés érkezett rá;
- a lépésenkénti működési tisztázás alaplogikájával a partneroldal
  alapvetően egyetértett.

A MATRIX-00 rendszertérképre 2026. szeptember 1-jén részletes írásos partneri
visszajelzés érkezett. A későbbi MATRIX-A, MATRIX-B és MATRIX-C
projektszakaszokhoz külön formális, aláírt és céges pecséttel ellátott
munkatartalom-megerősítő dokumentumok állnak rendelkezésre.

A nyilvános portfólió a különböző bizonyítéktípusokat elkülönítve kezeli:
a MATRIX-00 esetében az írásos partneri felülvizsgálatot, az A/B/C szakaszok
esetében pedig a formális vállalati megerősítő dokumentumokat.

### 17.2 MATRIX-A / B / C

A MATRIX-A/B/C projektszakaszokhoz formális, aláírt és céges pecséttel
ellátott Üzleti Tartalom Megerősítő Levelek állnak rendelkezésre.

Mindhárom a MATRIX-SYS FŐ BLOKK TÉRKÉP v1.0 munkatartalmára hivatkozik.

Kibocsátó:  Shenzhen-i technológiai vállalat — a vállalat neve a nyilvános változatban nem kerül közlésre
Képviselő:  Felhatalmazott vállalati képviselő / CEO — neve a nyilvános változatban nem kerül közlésre
Beosztás:   CEO (总裁)

MATRIX-A — 2026. szeptember 7.
  Kínai tartalmi megjelölés: 合作关系中的独立性与信任机制
  (Az együttműködési kapcsolat függetlenségi és bizalmi mechanizmusa)

MATRIX-B — 2026. szeptember 11.
  Kínai tartalmi megjelölés: 报酬与启动资源
  (Kompenzáció és induló erőforrások)

MATRIX-C — 2026. szeptember 11.
  Kínai tartalmi megjelölés: 员工招聘与组织融入
  (Munkatársak toborzása és szervezeti integrációja)

A munkatartalmat teljes dokumentum-ellenőrzésre, folyamat-felülvizsgálatra
és belső végső ellenőrzésre hivatkozva erősítették meg.

## 18. KÜLSŐ SZAKMAI KÖRNYEZET ÉS AI-HASZNÁLAT

A munkamódszerem szempontjából lényeges tapasztalat, hogy szakmai partnerek
nem önmagában az AI-eszköz használatát értékelik, hanem a végeredmény
minőségét és ellenőrizhetőségét.

Ügyvédek, orvosok és vállalati szereplők előtt is transzparensen kezeltem,
hogy AI-rendszereket használok a munkafolyamatban.

A különbség az ellenőrizetlen generáláshoz képest:

- a feladat strukturált;
- a forrás elkülönül;
- a modellek külön szerepet kapnak;
- a kimenet keresztellenőrizhető;
- a korrekció dokumentálható;
- a végső döntés emberi kontroll alatt marad.

Ez a működés több szakmai környezetben elfogadhatónak és használhatónak
bizonyult.

## 19. PORTFÓLIÓ-ÖSSZEFOGLALÓ

Almási Andor — AI Workflow & Validation Analyst

Munkám strukturált AI-munkafolyamatokat, emberi kontroll alatt működő
validációt, többmodellű keresztellenőrzést, reprodukálható technikai
vizsgálatot és bizonyítékalapú projektstrukturálást kapcsol össze.

A portfólió mögött nem kizárólag koncepciók állnak.

Rendelkezésre állnak:

- futtatható Python-artefaktumok;
- reprodukált regressziós tesztek;
- forráshash-ek;
- független ellenpróbák;
- dokumentált hibák és verziójavítások;
- többmotoros keresztvalidáció;
- valós üzleti projektanyagok;
- külső vállalati visszajelzések;
- aláírt és céges pecséttel ellátott megerősítő dokumentumok.

A munkamódszerem lényege:

A komplex problémát strukturálni.
Az AI-t intenzíven használni.
Az eredményt nem vakon elfogadni.
A hibát megtalálni és dokumentálni.
A bizonyítékot megőrizni.
A végső döntést emberi kontroll alatt tartani.

Ezt a munkamódszert olyan konkrét AI-, validációs vagy komplex
rendszerproblémákon tudom alkalmazni, ahol a megbízó számára fontos az
ellenőrizhetőség, a dokumentálhatóság és az emberi döntési kontroll.

# VERZIÓREGISZTER

- **v3.0 — 2026-09-18 — Plus motor:** első teljes magyar Master.
- **v3.1 — 2026-09-18 — Plus motor:** kommunikációs, MATRIX-szétválasztási és zárási javítások.
- **v3.2 — 2026-09-18 — Claude motor:** MATRIX-00 szerződéses implikáció pontosítása; reprodukciós környezet tisztázása; MATRIX-A bizonyítási szintjének korábbi jelölése.
- **v3.3 — 2026-09-18 — Claude motor:** Public GitHub draft; transzparens anonimizálás, MATRIX-00 bizonyítéktípusok elkülönítése, forráskód-hozzáférési szöveg.
- **v3.3.1 — 2026-09-18 20:37:42 CEST — Plus–Claude keresztvalidált kiadás:** MATRIX-A explicit kínai megjelölésének korrekciója; Markdown- és számozási hibák javítása; túlállítások eltávolítása; nyilvános GitHub-kiadás véglegesítése.
