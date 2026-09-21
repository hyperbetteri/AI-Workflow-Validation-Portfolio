# GEH-Core — Kutatási háttér és jelenleg is nyitott problémák

**Kapcsolódó fő dokumentum:** [GEH-Core — Nyilvános szakmai összefoglaló](../portfolio/GEH_CORE_PUBLIC_OVERVIEW_HU.md)  
**Verzió:** 0.2-HU  
**Keltezés:** 2026. szeptember 22.  
**Dokumentum-időbélyeg:** 2026-09-22T00:26:01+02:00  
**Szerző:** Almási Andor Aladár

## 8. Kutatási háttér és jelenleg is nyitott problémák

A GEH-Core fejlesztési iránya több olyan problématerülethez kapcsolódik, amelyekre a mesterségesintelligencia-kutatás jelenleg is megbízható, általánosan alkalmazható megoldást keres.

Az alábbi tanulmányok közvetlenül dokumentálják ezeket a problémákat. A hivatkozások nem a GEH-Core független műszaki tanúsításai, hanem annak bizonyítékai, hogy a rendszer által kezelt problémák valósak, mérhetők és tudományosan aktuálisak.

### 8.1. Kötelező feltételek meggyengülése az agentek közötti átadáskor

**When “Must” Becomes “Maybe”: Constraint Weakening in LLM Agent Workflows**  
Közvetlen forrás: https://arxiv.org/abs/2608.24569

A kutatás 1296 ellenőrzött kísérleti epizódban vizsgálta, mi történik, amikor egy agent által azonosított kötelező feltétel összefoglaláson, tervkészítésen vagy másik agentnek történő átadáson megy keresztül.

Az eredmények szerint a feltétel szöveges tartalma megmaradhat úgy is, hogy közben elveszíti kötelező működési erejét. A normál összefoglaló átadás során a vizsgált korlátozások 100 százaléka deaktiválódott, és az esetek 54,2 százalékában tiltott végrehajtás történt.

A tanulmány szerint a szemantikai megőrzés önmagában nem garantálja a működési állapot megőrzését.

**GEH-Core-kapcsolat:**

- operátori szándék megőrzése;
- kötelező állapotmezők;
- kontextus- és feladatkörvédelem;
- végrehajtási feltételek elkülönített kezelése;
- fail-closed működés;
- átadási állapotok ellenőrzése.

A GEH-Core strukturált állapotkezelése közvetlenül erre a dokumentált problémára ad működési választ.

Forrásminőség: erős kontrollált preprint, nagy kísérletszámmal; független replikáció még szükséges.

### 8.2. Minőségvesztés különböző modellek közötti feladatátadáskor

**The Handoff Tax: Continuing Non-Native Trajectories in LLM Agents**  
Közvetlen forrás: https://arxiv.org/abs/2608.24358

A kutatás azt vizsgálta, hogyan változik a teljesítmény, amikor egy hosszú agentes munkafolyamatot az egyik nyelvi modellről egy másikra adnak át.

Az eredmények szerint az erősebb modellre történő váltás önmagában nem állítja helyre automatikusan a minőséget. A teljes korábbi munkafolyamat átadása az elveszett teljesítménykülönbség kevesebb mint felét hozta vissza, miközben jelentős többletköltséget okozott.

A tanulmány kimutatja, hogy a modellváltás nem semleges művelet: az előző motor gondolkodási és munkafolyamati nyoma korlátozhatja a következő motor működését.

**GEH-Core-kapcsolat:**

- motorváltási állapot rögzítése;
- forrásmotor és ellenőrző motor elkülönítése;
- strukturált, minimális állapotátadás;
- a korábbi motor feltételezéseinek leválasztása;
- független újraértékelés;
- átadási torzulás felismerése.

A GEH-Core többmotoros működése nem feltételezi, hogy a teljes előzmény mechanikus átadása megőrzi a feladat eredeti jelentését és minőségét.

Forrásminőség: több modellcsaládon végzett összehasonlító preprint; elsősorban kódoló agentekre vizsgálták.

### 8.3. A saját értékelés nem elegendő a rendszer fejlődésének igazolására

**Aspire: Can Models Self-Evolve from Vague Goals?**  
Közvetlen forrás: https://arxiv.org/abs/2608.31111

Az ASPIRE kutatás 520 rejtett, szakértők által létrehozott feladaton vizsgálta, hogy az agentek képesek-e homályosan meghatározott célból saját fejlesztési és értékelési folyamatot kialakítani.

A kutatás szerint az agentek gyakran nem megfelelő adatokat választottak, túlzottan megbíztak saját szűk értékeléseikben, és a helyi javulás nem ment át a rejtett ellenőrzésre. A további önfejlesztés korábban elért eredményeket is eltörölhetett.

A tanulmány alapján egy motor saját értékelése nem használható önmagában végső referenciaként.

**GEH-Core-kapcsolat:**

- egyetlen motor nem lehet saját működésének kizárólagos hitelesítője;
- független többmotoros keresztvalidáció;
- rejtett vagy elkülönített ellenőrző feladatok;
- verziók közötti regresszióvizsgálat;
- emberi szakértői kontroll;
- korábbi működési állapot visszajátszhatósága.

A GEH-Core független ellenőrzési rétege közvetlenül a saját értékelésből eredő torzítás csökkentésére szolgál.

Forrásminőség: nagy, szakértői rejtett tesztkészletre épülő preprint; a vizsgált célok általánosíthatósága további ellenőrzést igényel.

### 8.4. Korrelált hibák és félrevezető modellbizonyosság

**One Human, N Agents: Audit-Budget Allocation for LLM Agent Fleets under Miscalibrated, Correlated Confidence**  
Közvetlen forrás: https://arxiv.org/abs/2607.28317

A tanulmány olyan helyzetet vizsgál, amelyben egy embernek több agent működését kell ellenőriznie korlátozott auditkapacitás mellett.

Az eredmények szerint a modellek saját bizonyossági értékei több esetben működésileg használhatatlanok voltak. A kutatás azt is kimutatta, hogy a különböző modellcsaládok hibái nem feltétlenül függetlenek: a közös feladatnehézség erősebb korrelációt okozhat, mint amit pusztán a gyártók vagy modellcsaládok különbözőségéből várnánk.

Ez azt jelenti, hogy több motor azonos válasza önmagában még nem bizonyítja a válasz helyességét.

**GEH-Core-kapcsolat:**

- nem egyszerű többségi szavazás;
- bizonyítékelsőbbség;
- eltérő motorok hibáinak korrelációvizsgálata;
- bizonyossági állítások külön ellenőrzése;
- emberi ellenőrzési kapacitás célzott felhasználása;
- egyező, de bizonyítatlan válaszok visszatartása.

A GEH-Core keresztvalidációja nem a motorok önértékelését vagy puszta számbeli többségét kezeli végső bizonyítékként.

Forrásminőség: matematikai és empirikus modellt egyesítő preprint; a valós környezetekre történő általánosítás további vizsgálatot igényel.

### 8.5. Többagentes rendszerek megfigyelhetőségének és hibakeresésének hiánya

**Observability and Fault Injection for LLM-Based Multi-Agent Systems in Software Engineering**  
Közvetlen forrás: https://arxiv.org/abs/2608.24271  
IEEE ICST 2026 publikációs adat: https://doi.org/10.1109/ICST69053.2026.00037

A kutatás kiindulópontja, hogy a nagy nyelvi modellekre épülő többagentes rendszerek működését jelenleg nehéz megfigyelni, hibakeresni és ellenőrzött meghibásodások mellett vizsgálni.

A szerzők ezért egységes OpenTelemetry-alapú nyomkövetést és célzott hibainjektálást kapcsoltak össze. A rendszer külön rögzíti az agentes lépéseket, a modellek közötti kommunikációt, az eszközhasználatot és a modellhívásokat.

A munka azt bizonyítja, hogy a reprodukálható nyomkövetés és a célzott hibavizsgálat jelenleg is aktív fejlesztési terület.

**GEH-Core-kapcsolat:**

- verziózott eseménynapló;
- motoronként elkülönített döntési nyomvonal;
- hibaterjedési pontok azonosítása;
- reprodukálható tesztek;
- célzott regresszióvizsgálat;
- döntési és végrehajtási rétegek elválasztása.

A GEH-Core eseménynaplózási és visszajátszási elve ugyanennek a problématerületnek egy szélesebb, többmotoros validációs megközelítése.

Forrásminőség: IEEE-konferencián megjelent műszaki munka; a bemutatott validáció még korlátozott számú rendszerre terjed ki.

### 8.6. Az agentes nyomvonalak nehezen auditálható szerkezete

**Automata from Agent Traces: Failure and Next-Step Prediction**  
Közvetlen forrás: https://arxiv.org/abs/2608.23670  
OpenReview-adatlap: https://openreview.net/forum?id=1cprFkvFT0

A tanulmány szerint a hosszú, strukturálatlan agentes nyomvonalak ellenállnak a hagyományos biztonsági auditnak és futásidejű megfigyelésnek.

A szerzők tizenkét nyilvános adathalmaz teljes nyomvonalaiból véges állapotú automatákat készítettek. A kinyert állapottopológia lehetővé tette a következő lépések és a várható hibák korai becslését.

A kutatás egyik lényeges eredménye, hogy a megfigyelt működési topológiát részben erősebben alakíthatja a futtatási keret, mint maga a nyelvi modell.

**GEH-Core-kapcsolat:**

- modell és futtatási környezet hatásának szétválasztása;
- állapotalapú működési napló;
- drift és router-interferencia felismerése;
- korai hibajelzés;
- determinisztikus visszajátszás;
- azonos feladat több futásának összevetése.

Ez alátámasztja, hogy egy agent működését nem lehet kizárólag az alapmodell tulajdonságaiból megítélni; a külső logikai és végrehajtási rendszer külön ellenőrzési tárgy.

Forrásminőség: tizenkét nyilvános adathalmazra épülő preprint és OpenReview-bejegyzés; független reprodukció még szükséges.

### 8.7. A jelenlegi benchmarkok nem fedik le az intézményi követelményeket

**Agent Benchmarks Fail Public Sector Requirements**  
Közvetlen forrás: https://arxiv.org/abs/2601.20617

A kutatás több mint 1300 agentes benchmarkot elemzett abból a szempontból, hogy megfelelnek-e a közszférában szükséges eljárási, jogi, szerkezeti és valósághűségi követelményeknek.

Az eredmény szerint egyetlen vizsgált benchmark sem teljesítette az összes meghatározott feltételt.

Ez azt mutatja, hogy a jelenlegi általános teljesítménymérések önmagukban nem elegendők intézményi vagy magas felelősségű alkalmazások hitelesítésére.

**GEH-Core-kapcsolat:**

- eredményalapú mérés helyett folyamatellenőrzés;
- döntési út és bizonyítékok naplózása;
- jogosultsági és felelősségi rétegek vizsgálata;
- emberi jóváhagyási pontok;
- valós munkafolyamatokon végzett validáció;
- területspecifikus ellenőrzési feltételek.

A GEH-Core megközelítése nem kizárólag azt vizsgálja, hogy a rendszer elérte-e a kívánt végkimenetelt, hanem azt is, hogy milyen ellenőrizhető folyamaton keresztül jutott oda.

Forrásminőség: több mint 1300 publikációt feldolgozó, szakértőileg ellenőrzött elemzés; konferenciamegjelenésre elfogadott preprint.

### 8.8. Összefoglaló kutatási következtetés

A felsorolt kutatások egymástól függetlenül ugyanabba az irányba mutatnak:

- a modellváltás torzíthatja a munkafolyamatot;
- az összefoglalás meggyengítheti a kötelező feltételeket;
- a motor saját értékelése nem elegendő;
- több modell hibája korrelálhat;
- a puszta többségi egyezés nem jelent bizonyítást;
- a hosszú agentes folyamatok nehezen auditálhatók;
- a futtatási környezet jelentősen alakíthatja a viselkedést;
- a jelenlegi benchmarkok nem fednek le minden intézményi követelményt;
- a többagentes rendszerek megfigyelhetősége és reprodukálható hibakeresése továbbra is nyitott fejlesztési terület.

A GEH-Core fejlesztési iránya ezekre a problémákra egységes működési keretben ad választ:

- bizonyítékelsőbbséggel;
- többmotoros keresztvalidációval;
- strukturált állapotátadással;
- kontextus- és feladatkörvédelemmel;
- ABSTAIN és fail-closed működéssel;
- emberi jóváhagyással és vétójoggal;
- verziózott eseménynaplóval;
- visszajátszható regressziós vizsgálatokkal.

A külső kutatások a problématerület tudományos jelentőségét igazolják. A GEH-Core saját működési eredményeinek igazolását a dokumentált tesztek, eseménynaplók, reprodukálható vizsgálatok és későbbi független szakmai validáció biztosíthatja.
