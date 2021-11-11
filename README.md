# orvosi vizsgálatok kiértékelésének mérnökinformatikai alapjai


> **Követelmények:**
> 
> - beadandó: 2000 szavas összefoglaló egy dokumentumfilmről
> - prezentáció: orvosi cikk prezentálása 10 percben + 5 perc kérdések
> - zh
> 
> ezek alapján megajánlott jegy, ha ezek nincsenek meg, akkor vizsga

> - nov. 4 konzultáció
> - nov. 11 zh
> - nov. 18 rektori szünet
> - nov. 25 előadások part I - clinical trial, observational study
> - dec. 2 előadások part II
> - dec. 3 videó összefoglaló beadandó határidő
> - dec. 9 pót zh

## EA2
### Bizonyítékokon alapuló orvoslás

**Részei:**
- expozíció (adott)
- oksági kapcsolat (keressük)
- végpont (választott)

**Nehézségek:**
- sztohasztikus értékek: statisztika, stb
- a következményei nem azonnaliak
- ismeretlen mechanikus komponensek: nehezen mérhető, nehezen tanulmányozható területeken, pl. biokémia
- erős hitvilág
- következmények: biztonság, monitorozás

*pl: - A vérnyomás csökkentő csökkenti-e a vérnyomást?
        - Császármetszés növeli-e az I. típusú diabétesz kialakulását?*

**Confounding**

<img src="https://www.healthknowledge.org.uk/sites/default/files/documents/elearning/epidemiologyp/rcbces/Exposure%20Outcome.jpg" width=50% height=50%>
- Cofounder: expozíciót és kimenetet is befolyásoló tényező
- Predictor: csak a kimenetre hat (a csoportok randomizációja miatt)
- Cofounding-probléma: Ha azt szertnénk nézni, hogy a császármetszés milyen kapcsolatban áll a születendő gyermek I. típusú diabéteszével? Ha cserélgetjük ezeket akkor is megfeleltethetőek egymásnak.

**Randomizáció**
- A célunk, hogy a két elkülönített csoport csak a vizsgált célban különbözzön, ne legyen nemi/kor/stb alapú egyéb különbség, akkor sem, ha pl öszesen 30 nő és 2 férfit osztunk szét.
- A kísérleteket vakosítjuk, ha tudjuk, hogy a betegek ne tudják melik csoportba kerültek.
- Ha teljesen random allokállom a csoportokat, akkor előfordulhat, hogy mind egy csoportba kerül!

<img src="https://emj.bmj.com/content/emermed/20/2/164/F1.large.jpg" width=50% height=50%>

**Oksági kapcsolat*** Az expozíciónál kitett, vagy nem kitett a két tényező.

blokkosítás:
//Statában

## EA3

| Tables        | Aetiological factors           | Intervention effects  |
| ------------- |:-------------:| -----:|
| observational - descriptive      | Case studies | Case studies |
|observational - compertive | CAse-control cohort | histroically controlled rials |
| experimental intervention | rare,esceptas prevention trials |    controlled trials |

**Eset sorozatok leírásai:**
- megfigyeléses vizsgálat
  - **cohort vizsgálatok:**
    - csoportokat képzünk egy közös faktorból (valami alapján csoportosítható, pl vlamainek ki van téve vagy valaminek nincs)
    - múltbeli faktor lapján kezdjük a vizsgálatot
    - nagyszámú beteget vizsgál
    - retrospektívnél hosszútávú megfigyelést is végre tud hajtani, viszonylag olcsón
    - náluk próbálok egy közös jellemzőt találni, hogy a betegségben szenvedőknél is így alakul-e?
    - oksági kapcsolatokat alakítunk ki
- leíró
- hipotéziseket generál
- ritka, hosszú távú hatásokat is megfigylehet

> **[Nun study](https://en.wikipedia.org/wiki/Nun_Study)**
> - Majdnem 700 amerikában élő katolikus apáca felajánlotta, hogy az agyukat szövetttani vizsgálatoknak ki lehet tenni, ezáltal egy homogén csoportot képezve. A vizsgálat elindult, és összehasonlították a tüneteket neuropatológiai szövetekkel.
> - Ez egy esetkontroll vizsgálat, retrospektív, cohorttal.
>
> Boncolás után találtak olyan eseteket ahol erős Alzheimer társult ép agyi szövetekkel, illetve erősen roncsolt szövetek előzetes tünetek nélkül.
>
> Korrleációt találtak szókincskészlettel: ezek alapján akinek gazdagabb szókincse volt később jelentkeztek nála tünetek.

**Torzítások:**
- az időbeli egymásutániságot az ember ok-okozati összefüggésnek hajlamos értelmezni
- az emlékezet torzíthatja a tényeket
- számít-e hogy hol laknak a figyelt alanyok (nem, ha pl földrészekről van szó)
- ugyanazon helyről származnak a mért adatok
- mi az alany elő- és utóélete
- milyen nagy a populáció

**Cross sectional:** a teljes populációban, nem is feltétlen a mintában hány beteg van(*prevalencia*), és hány új beteg jelenik meg (*incidencia*)?

**Ökonómiai tanulmányok:** Két azonos területen mért adat összehasonlítása, *pl: GDP - egészségügy / országokra lebontva*

<ims src="https://s2.studylib.net/store/data/005488388_1-d55c7bb53c27169c2e8c7771914750a2.png" width=50% height=50%>

### Gyógyszerfejlesztés fázisai
<img src="https://www.phrma.org/-/media/Project/PhRMA/PhRMA-Org/PhRMA-Org/Teaser-Image/Clinical-Trial-Chart.jpg?w=768&hash=847BFF91FAFFF09919D099FC8295AE18" width=50% height=50%>

Pre-clinical research and development
  - **1. fázis**
    - biztonságos-e a készítmény
    - kontrollált
    - gyakori mellékhatás
    - a 3 beteg egy csoportban jelemző a területre
    - dózis vizsgálat
  - **2. fázis**
    - a maximum dózis meghatározás
    - a betegek nem egyszerre kapják a gyógszert
    - nincs kontroll (nem érdekel, hogy hánynak-e)
  - **3. fázis**
    - van kontrollcsoport
    - törzskönyvezés
    - engedélyezés folyamata
  - **4. fázis**
    - már kint van a piacon
    - hosszútávú mellékhatások mérése
    - engedélyezett

- Clinical research and development
  - ...


- Átszivárgás kontroll csoportból kezelt csoportba
  - **per protocol:** van egy mintám amit randomizálok `A` és `B` csoportba, A protokollal azt mondjuk, hogy az adott csoportban a kezelést úgy hasonlítjuk össze, hogy ahol tényleg megtörtént és úgy történ meg ahoy le van írva, és az alapján úgyabb két-két csoportot alkotunk.
  - **intention to treat:** nem vesszük figyelembe azt, hogy mi történt a két csoportban, csak az egyiket választjuk fő elemzésnek és összehasonlítjuk a másikkal.

<img src="https://pbs.twimg.com/media/D1BTV9CWsAAiJKp.jpg" width=50% height=50%>

## EA4

### Kaplan-Meier plot, censoring
<img src="https://miro.medium.com/max/1400/1*ATbW_NU5GMtTaCCPpfkzEA.png" width=50% height=50%>

### Cox regresszió
> kihat a túlélésre: *nem*, *kor*, *stb*
>
> A végső arány amit kapunk, az a hazard ratio.

<img src="https://www.researchgate.net/publication/341746353/figure/download/fig4/AS:897727533678599@1591046331701/Univariate-Cox-regression-analysis-of-differentially-expressed-autophagy-related-genes.png" width=50% height=50%>

### Lead time bias
<img src="https://i2.wp.com/first10em.com/wp-content/uploads/2018/06/777px-Lead_time_bias.png?fit=777%2C224&ssl=1" width=50% height=50%>
> mennyien halnak meg amúgy is miután hatott a kezelés
>
> Jól látszik, hogy attól, hogy hamarabb detektálom, nem növeli meg az életminőséget.

### Immortal time bias
> egy kezelés amire várni kell valamennyit
<img src="https://www.bmj.com/content/bmj/340/bmj.b5087/F2.large.jpg" width=50% height=50%>

## EA5
> Ha van egy informácink a fluktuációról akkor tudunk egy mintaelem számot számolni, és tudjuk számolni mennyi az esély arra, hogy random-e a fluktuáció.

A szignifikáns különbségek mögött fontos kérdés, hogy hány emberen végzett vizsgálat alapján számoltunk.

- p érték, elütés, adatkezelés nagyobb valószínűséggel add false pozitiveot mint a mintavételi hibák

> binomiális adatgörbénél a nagyság melett a bekövetkezési esély is számít. Ha ritka eseméynt nézek akkor nem nagy a különbség kettő között törvény szerűen.

- **klinikai szignifikancia:** tartalmi eltérés
- **p:** mértékegység nélküli különbség

- 3mmHG-al csökkentett magas vérnyomás már populáció szinten, eloszlása jelentős 
- populáció szinten az ami egyéni szinten mérési hibaként is elkönyvelhető, jelentős lehet

**konfidencia intervallum**: pontbecsléshez hozzárendelt intervallum, pl:*95%os konfidencia intervallumon az érték 95%al beleesik a keresett csoportba*

> *filmmel kapcsolatos kérdések:*
> - *milyen új dolgot hallottál*
> - *hogyan és mi alapján történik döntéshozatal 1-1 kezelés kapcsán*
> - *hogyan zajlik döntéshozatal MAgarországon*
> - *mi az leőnye/hátránya*
> - *milyne kezelés lehet kiugróan költségkímélő*
> - *hogy döntöttél volna szavazáskor*
> - *mi nem hangzot el a filmben?*

## EA6
### Regression to the mean

- a biológiai folyamatok fluktuiálnak
- ezkenek lehet trendje
- ha vágok egyet akkor az, ha egy extrém pontnál vágom el akkor azok a megigyelések amik alatta vannak közelebb lesznek az átlaghoz.

<img src="https://ars.els-cdn.com/content/image/1-s2.0-S0735109716351099-gr6.jpg" width=50% height=50%>

Ha egy beteg állapotot nézünk akkor az minidg egy kicsit extrém, tehát ha beteg akkor az ő bináris állapotát valamilyen folytonos mennyiségből származtatt bináris álllapotokra vonatkoztatjuk.

*Pl:*
- *vérnyomás*
- *depresszió*
- *fájdalom*

A variabilitással mérhetjük az időbeli változását

### Placebo hatás
> no intervention = regression to the mean
>
> ha lemérek egy csoportot és nincs utána különbség akkor jelenik meg a *regression to the mean*
>
> ha placebo kontroll csoportot adok meg akkor a *placebo hatás*hoz hozzáadódik a *regression to the mean*
>
> ha van egy kezelt kontroll csoport akor azoknál a *kezelés hatása* is megjelenik

### fontos-e a reprezentativitás?
- nem kell reprezentatív legyen a minta ahhoz, hogy egy kísérleti eredmény számszerűleg valid legyen**!**
- ha egy statisztikai kérdést nézünk populációra vonatkozóan akkor annak egyeznie kell az általunk elvárt populációhoz

**DE**

> #### Mitől reprezentatív a statisztikai felmérés:
> - ha a populációt nem akarjuk másiokhoz hasonlítani

> #### Kevésbé reprezentatív:
> - irreleváns a hajszíne, stb
> - releváns: a kora, elhízás, neme, stb => ez a kockázata
>
> a kockázata másmilyen, mint a mi áltlaunk mért populáció akkor ***nem reprezetnatív a mintánk egészségügyi szempontból***  

***Minden statisztikai vizsgálat a vizsgált szempont alapján kell reprezentatív legyen.***

Risk ratio: mekkora esélyem van a másik csoportban meggyógyulni, azaz a `treated/control`:  `megtörtént/1`
Odds ratio: mekkora esélyem arra, hogy odds skálán meggyógyuljak `p/(1-p)`, azaz kiszámolom ezt a törtet mindkét csoportra majd a kettőt elosztjuk `megtörtént/(1-megtörtént)`

<img src="https://assets.cureus.com/uploads/figure/file/138481/lightbox_65ee62a0db3611eaafa31b2789baa093-fig-1-odds-vs-prob.png" width=50% height=50%>

ARR = absolute risk reduction =  a két risket kivonom egymásból
RD = risk differnece

Egy jó leírás: (When to use the odds ratio or the relative risk?)[https://www.semanticscholar.org/paper/When-to-use-the-odds-ratio-or-the-relative-risk-Schmidt-Kohlmann/69a8767574819102bf47572df70c0561ddc8633b/figure/1]        
        
A kezelés odds ratioja átvihető egyik populációról másikra!

Ha kontextusa más a mérésnek és a viszonyított populációnak, így más lesz a végeredmény.

Ha a populációban jelentős a különbésg valamilyen téren akkor jó eyélel nem lesz megfelelő egy másik populációra, *pl: ezért más a koncnetráció megy más génállományú betegekbe*

A nem reprezentativitás a csak a háttérkokckázat szempontjából számít.

> *zh kérdés: Mi a három hatás ami megjelenhet a csoportoknál? Regression to the mean, placebo hatás, kezelés hatása.*
> *kivétel: interakció, más a populáció, más a kezelés*

## EA7
https://vimeo.com/4796083

## EA8
### Klinikai kíséreletek és vizsgálatok protokolljai
A protokoll a kísérlet írásos terve ami mindenre megszületik a kísérlettel kapcsolatban. Ezzel lehet pályázni kísérletekhez támogatásért. 

A tervel illik transzparensnek lenni, ez íratlan szabály.

- Ez a legfrisseb verzió?
- Milyen változtatás született a verziók között (change log)
- Good clinical prctice filozófia követése
  - ***good clinical prctice:*** *Egy egészségügyi leírás csomag, amiben protokollok vannak csomagokba gyűjtve. *
- A bevezető fontos, főleg olyanoknak akiknek nincs az adott szakmában közvetlen háttértudásuk.
- Mekkora a társadalmi fontossága? Mennyi embert érint, érinteni fog, stb?
- Szükséges erőforrás becslés (hány nap kórházi ellátás, mennyi embert érint, munkaórák, stb.)
- Mit érhetünk el?
- Hol és mekkora kontrollcsoportunk van?
- Risk assesment az etikai bizottság felé, amennyiben érintett a kérdés, pl. halálozás esetén.
- Trial design: minnél szélesebb legyen, hogy a végeredmény jól kezelhető legyen.
  - A beteg legyen tényleg beteg.
  - Kizáró kritériumok: kor, terhesség, alkoholizmus, stb.
  - Stopping rules: DMEC - TSC dönt, hogy helyes-e a kísérlet
    - recruitment nem jön össze
    - biztonsági okok
  - Kezelések: bemutatja mondjuk egy gyógyszer hatásait, lefolyását, stb.
    - mi számít tényleg kezelésnek és miképp lesz mérve?
  - Végpontok: megfogalmazza a várt kimeneteket
  - Mellékhatás: 
    - kedvezőtlen esemény (AE), nem kell közvetlen kapcsolatban legyen a kezeléssel. Hogy ok-okozati összefüggés van-e, azt később döntik el. Valami betegésgre jellemző eseményt lehet, hogy nem kell feltüntetni, ezt is itt határozzák meg.
    - fontos kedvezőtlen eseményt (SAE) azonnal jelenteni kell a hatóságoknak, akár halállal is járó mellékhatás lehet
  - Protokoll: vannak-e farmatokinetikai mérések
    - ha csak nem kifejezetten ezzel foglalkozunk akkor a statisztikai szempontból nem lényeges
- Vizit leírása
- Statisztikai összefoglaló: milyen módszert alkalmaztak és hogy mérték, mi van a hiáynzó adatokkal 
- Betegek informálása, stb.

### Különböző szórások összehasonlítása:
<img src="https://www.nlm.nih.gov/nichsr/stats_tutorial/images/Section2Module7HighLowStandardDeviation.jpg" width=50% height=50%>

### Vakosítás
> Első szintű vakosítás: a beteg ne tudjon arról, hogy mit kap.
> 
> Kettős vak a vizsgálat: a gyógyszertátban aki átadja a gógyszert ne tudja mit ad át, az orvos, és a kezelő személyzet se tudja, hogy a beteg mit kap.
> 
> Hármas vakosítás: a statisztikus se tudja ki milyen csoporthoz tartozik.

- 1995 számít a vakosítás
- 200 nem számít
- 2001 számít

