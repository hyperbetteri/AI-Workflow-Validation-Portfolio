# GEH-Core

## Etikai alapú, többmotoros mesterségesintelligencia-validációs keretrendszer

**Nyilvános szakmai összefoglaló**

**Verzió:** 0.2-HU – jóváhagyás előtti változat  
**Keltezés:** 2026. szeptember 22.  
**Dokumentum-időbélyeg:** 2026-09-22T00:26:01+02:00  
**Szerző:** Almási Andor Aladár

## 0. Vezetői összefoglaló

A GEH-Core olyan logikai, etikai és ellenőrzési keretrendszer, amely különböző nagy nyelvi modellek és agenteszközök együttműködését teszi ellenőrizhetőbbé, következetesebbé és emberközpontúvá.

A rendszer ugyanazt a feladatot több, egymástól lehetőség szerint független motorral vizsgálja. Elkülöníti a bizonyítékot a modellfeltételezéstől, védi az operátor eredeti szándékát és a feladat hatókörét, felismeri az ellentmondásokat, és bizonytalanság esetén visszatarthatja a végrehajtást.

A módszertan fő elemei:

- belülről épített etikai és logikai alap;
- többmotoros keresztvalidáció;
- bizonyítékelsőbbség;
- kontextus- és feladatkörvédelem;
- ABSTAIN és fail-closed működés;
- emberi jóváhagyás és vétójog;
- verziózott eseménynapló;
- visszajátszható regressziós vizsgálatok;
- a modell-, agent-, jogosultsági és operátori felelősség elkülönítése.

A GEH-Core fejlesztési háttere mintegy öt év mesterségesintelligencia-rendszerekkel végzett gyakorlati munkára, ezen belül több mint három év intenzív, többmotoros LLM-működés, mély logikai viselkedés, kontextuskezelés, hibamintázatok, motorváltások és ember–AI együttműködési folyamatok rendszeres vizsgálatára épül.

Ez a munka folyamatos valós munkafolyamatokon végzett megfigyelést, több modellcsalád összehasonlítását, ismételt hibakeresést és regressziós ellenőrzést, dokumentált többmotoros keresztvalidációt, valamint műszaki, jogi, dokumentációs és üzleti környezetben szerzett gyakorlati tapasztalatot foglal magában.

A keretrendszer nem egyetlen modellhez vagy gyártóhoz kötődik.

A belső logikai mag, a részletes szabálystruktúra, a paraméterezés és a működési know-how nem része a nyilvános dokumentációnak.

## 1. Miről szól a projekt?

A GEH-Core olyan logikai, etikai és ellenőrzési módszertan, amely különböző nagy nyelvi modellek és agenteszközök együttműködését teszi ellenőrizhetőbbé, következetesebbé és emberközpontúvá.

A módszer alapja nem külső tiltásrendszer, hanem belülről épített etikai és logikai alap.

A rendszer nem egyetlen mesterségesintelligencia-modell válaszát tekinti automatikusan helyesnek. Több, egymástól lehetőség szerint független motor eredményeit veti össze, kezeli az eltéréseket, és meghatározott bizonytalansági vagy ellentmondási helyzetekben emberi döntést kér.

## 2. Milyen problémát old meg?

Számos jelenlegi mesterségesintelligencia-rendszer külső szabályokkal és végrehajtási korlátokkal próbálja kezelni a már meglévő képességek kockázatait. Ez önmagában nem mindig biztosít koherens működést.

A GEH-Core fordított megközelítést alkalmaz: az etikai, logikai és ellenőrzési alapelveket nem utólagos korlátozásként, hanem a működés kiindulási szerkezeteként kezeli.

A módszertan többek között az alábbi problémák csökkentésére irányul:

- az operátori szándék elvesztése vagy eltorzulása;
- kontextus- és feladatkör-eltérés;
- kötelező feltételek meggyengülése összefoglalás vagy motorváltás során;
- hibás modellfeltételezések bizonyítékként történő kezelése;
- egymást erősítő vagy korrelált modellhibák;
- ellenőrizetlen motor- vagy agentváltás;
- végrehajtás bizonytalan vagy ellentmondásos állapotban;
- nem követhető döntési út;
- emberi felülvizsgálat nélküli kritikus döntés;
- vissza nem játszható vagy nem reprodukálható munkafolyamat.

## 3. A rendszer fő képességei

### 3.1. Többmotoros keresztvalidáció

Ugyanazt a feladatot több, egymástól lehetőség szerint független nagy nyelvi modell vagy agenteszköz dolgozhatja fel.

A rendszer nem egyszerű többségi szavazást alkalmaz. Vizsgálja:

- az eredmények közötti tartalmi egyezést;
- az eltérések okát;
- a felhasznált bizonyítékokat;
- a kontextus megtartását;
- az operátori cél teljesülését;
- a bizonytalanságot;
- a modellek közötti lehetséges hibakorrelációt.

Egyetlen motor eredménye sem válik kizárólag saját állítása alapján referenciává.

### 3.2. Bizonyítékelsőbbség

Az ellenőrzött közvetlen bizonyíték és az explicit operátori korlát elsőbbséget élvez a nem igazolt modellfeltételezéssel szemben.

A rendszer elkülöníti:

- a közvetlenül rendelkezésre álló adatot;
- az ellenőrzött külső forrást;
- az operátor által meghatározott tényt vagy korlátot;
- a modell következtetését;
- a nem igazolt feltételezést;
- a különböző források közötti ellentmondást.

Bizonyítéki ütközés esetén emberi felülvizsgálat szükséges.

### 3.3. Kontextus- és feladatkörvédelem

A rendszer ellenőrzi, hogy a válasz vagy végrehajtási javaslat megfelel-e:

- az eredeti feladatnak;
- az operátor kifejezett céljának;
- a meghatározott hatókörnek;
- az alkalmazandó etikai és adatvédelmi feltételeknek;
- a rendelkezésre álló bizonyítékoknak;
- a jóváhagyott működési állapotnak.

A feladatkör önkényes kiterjesztése, a cél átértelmezése vagy az operátori korlátozás figyelmen kívül hagyása eltérésként kerül kezelésre.

### 3.4. ABSTAIN és fail-closed működés

Ha az ellentmondás nem oldható fel megfelelő bizonyossággal, a rendszer nem kényszerít ki mesterséges eredményt.

Ilyen esetben:

- visszatarthatja a végrehajtást;
- további bizonyítékot kérhet;
- emberi szakértői felülvizsgálatot kezdeményezhet;
- a feladatot biztonságosan lezárt vagy várakozó állapotba helyezheti.

Az ABSTAIN működés azt jelenti, hogy a rendszer képes kimondani: a rendelkezésre álló adatokból nem állítható elő kellően megbízható eredmény.

A fail-closed működés azt jelenti, hogy bizonytalan vagy nem ellenőrzött állapotban a rendszer nem hajt végre visszafordíthatatlan műveletet.

### 3.5. Auditálhatóság

Minden döntési lépés naplózott és visszajátszható.

Az auditálhatóság célja annak utólagos megállapíthatósága, hogy:

- milyen bemeneti adatok álltak rendelkezésre;
- melyik motor milyen eredményt adott;
- milyen eltérések jelentek meg;
- milyen bizonyíték vagy szabály alapján született döntés;
- mikor történt emberi jóváhagyás, korrekció vagy vétó;
- melyik rendszer- és szabályverzió működött a vizsgált időpontban;
- melyik átadási vagy végrehajtási ponton jelent meg hiba.

### 3.6. Emberi döntési jog

Az emberi operátor szerepe nem opcionális kiegészítés.

A rendszer minden kritikus döntési ponton fenntartja:

- az emberi jóváhagyás lehetőségét;
- a végrehajtás megállításának jogát;
- a döntés felülvizsgálatát;
- a korrekció és a vétó lehetőségét;
- a felelősségi pont egyértelmű kijelölését.

A mesterséges intelligencia döntéstámogató és validációs szerepet tölthet be, de nem szünteti meg az emberi felelősséget.

## 4. Etikai és logikai alap

A rendszer logikai alapjához egy harmincpontos etikai kódex, valamint kapcsolódó célfüggvény tartozik.

Az etikai kódex nem egyszerű tiltáslista. Olyan összefüggő elvrendszert alkot, amelynek célja:

- az emberi méltóság és döntési jog védelme;
- a károkozás csökkentése;
- a bizonyíték és a feltételezés elkülönítése;
- az arányosság megtartása;
- az adatminimalizálás;
- a visszaélések és logikai konfliktusok felismerése;
- az ellenőrizhető működés biztosítása;
- a felelősségi szintek elválasztása.

Hibás működés esetén nem elegendő pusztán másik motort választani: a működési keretet az etikai és logikai alap megtartásával újra kell építeni és validálni.

A részletes etikai kódex, a célfüggvény, valamint a hozzájuk kapcsolódó végrehajtási szabályok nem részei ennek a nyilvános dokumentációnak.

## 5. Alkalmazási területek

A módszertan az alábbi területeken alkalmazható vagy vizsgálható:

- mesterségesintelligencia-alapú munkafolyamatok validációja;
- többmotoros minőségbiztosítás;
- agenteszközök együttműködésének ellenőrzése;
- összetett dokumentációk tartalmi összevetése;
- jogi és egészségügyi dokumentumok többmotoros elemzése, kötelező emberi szakértői felülvizsgálattal;
- műszaki hibakeresés és döntéstámogatás;
- kutatási és tudományos adatkezelés;
- összetett, több szereplős együttműködési folyamatok kezelése;
- adatvédelmi és jogosultsági rétegek ellenőrzése;
- civil védelmi és vészhelyzeti döntéstámogatás külön, fejlesztés alatt álló modulban.

A módszertan nem helyettesíti az orvosi, jogi, biztonsági vagy más szabályozott területen szükséges szakértői döntést.

## 6. Fejlesztési állapot

A GEH-Core nem lezárt szabvány és nem kész kereskedelmi termék.

A jelenlegi állapot:

- működő módszertani prototípus;
- valós feladatokon alkalmazott többmotoros munkafolyamat;
- ismételt hibakereséssel és keresztvalidációval fejlesztett rendszer;
- részben automatizálható, részben emberi felügyeletet igénylő architektúra;
- folyamatosan verziózott és ellenőrzött fejlesztés.

A GEH-Core fejlesztési háttere mintegy öt év mesterségesintelligencia-rendszerekkel végzett gyakorlati munkára, ezen belül több mint három év intenzív, többmotoros LLM-működés, mély logikai viselkedés, kontextuskezelés, hibamintázatok, motorváltások és ember–AI együttműködési folyamatok rendszeres vizsgálatára épül.

Ez a munka folyamatos valós munkafolyamatokon végzett megfigyelést, több modellcsalád összehasonlítását, ismételt hibakeresést és regressziós ellenőrzést, dokumentált többmotoros keresztvalidációt, valamint műszaki, jogi, dokumentációs és üzleti környezetben szerzett gyakorlati tapasztalatot foglal magában.

## 7. Fejlesztési és külső alkalmazási háttér

A módszertan nem laboratóriumi feltevésekből, hanem aktív műszaki, dokumentációs, adatkezelési és többmotoros együttműködési folyamatokból fejlődött ki.

A Shenzhen Beisi Wujie Technology Co., Ltd. hivatalos üzleti dokumentumban igazolta az együttműködési keretrendszer alkalmazását.

Ez külső üzleti alkalmazási visszaigazolás, nem független műszaki tanúsítás.

A további fejlesztés célja:

- a szabálystruktúra formalizálása;
- a naplózási és verziókezelési követelmények egységesítése;
- a modell-, agent-, jogosultsági és operátori felelősség elkülönítése;
- a visszajátszható regressziós vizsgálatok fejlesztése;
- a többmotoros keresztvalidáció mérhetővé tétele;
- a külső szakmai és biztonsági ellenőrzés előkészítése.

## 8. Kutatási háttér és jelenleg is nyitott problémák

A részletes kutatási háttér külön dokumentumban található:

[GEH-Core — Kutatási háttér és jelenleg is nyitott problémák](../technical-evidence/GEH_CORE_RESEARCH_CONTEXT_HU.md)

## 9. Mi nem kerül nyilvánosságra?

A nyilvános dokumentáció nem tartalmazza:

- a belső logikai magot;
- a teljes etikai kódexet és célfüggvényt;
- a végrehajtható szabálystruktúrát;
- a részletes döntési feltételeket;
- a küszöbértékeket és súlyozásokat;
- a belső szabályazonosítókat;
- a teljes strukturált adatmodellt;
- a működési promptokat;
- a konkrét integrációs eljárást;
- a validációs tesztek teljes felépítését;
- a részletes vészhelyzeti működést;
- a módszertan reprodukálását lehetővé tevő know-how-t.

A nyilvános anyag célja a fejlesztés lényegének, alkalmazási területeinek és ellenőrzési elveinek bemutatása, nem pedig a technológia reprodukálhatóságának biztosítása.

## 10. Iparjogvédelmi és közzétételi státusz

Ez a nyilvános dokumentáció kizárólag magas szintű szakmai bemutatást tartalmaz.

A fejlesztés újdonságának, oltalmazhatóságának, jogosulti viszonyainak és megfelelő iparjogvédelmi stratégiájának vizsgálatát dr. Rozsnyói Dávid szabadalmi ügyvéd bevonásával tervezzük elvégezni.

Az előzetes iparjogvédelmi vizsgálat lezárásáig nem kerül nyilvánosságra olyan további műszaki részlet, amelyből a védett módszertan vagy annak működési know-how-ja érdemben rekonstruálható.

## 11. Korlátozási nyilatkozat

Ez a dokumentum:

- nem műszaki specifikáció;
- nem szabvány;
- nem megfelelőségi tanúsítás;
- nem szabadalmi bejelentés;
- nem jogi, orvosi vagy biztonsági szakvélemény;
- nem biztosít engedélyt a módszertan reprodukálására;
- nem tartalmazza a teljes rendszer működtetéséhez szükséges információkat.

A dokumentum kizárólag a fejlesztés nyilvánosan közölhető szakmai összefoglalása.

## 12. Szerző és kapcsolat

**Szerző:** Almási Andor Aladár  
**Kapcsolat:** hyperbetteri@gmail.com  
**Dokumentumverzió:** 0.2-HU  
**Keltezés:** 2026. szeptember 22.  
**Időbélyeg:** 2026-09-22T00:26:01+02:00

A dokumentum tartalma Almási Andor Aladár szellemi munkája. A belső logikai mag, a végrehajtható szabálystruktúra és a reprodukálható működési know-how nem része a nyilvános közlésnek.
