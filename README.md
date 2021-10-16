# orvosi vizsgálatok kiértékelésének mérnökinformatikai alapjai


> **Követelmények:**
> 
> - beadandó: orvosi cikk összefoglalaása és prezentálása is
> - zh
> 
> ezek alapján megajánlott jegy ha ezek nincsennek meg akkor vizsga


# EA2
## Bizonyítékokon alapuló orvoslás
**Nehézségek:**
- sztohasztikus értékek: statisztika, stb
- a következményei nem azonnaliak
- ismeretlen mchanikus komponensek: nehezen mérhető, nehezentanulmányozható területeken, pl biokémia
- erős hitvilág
- következmények: biztonság, monitorozás

**Vizsgálatok szentháromsága:**
- expozíció
- kimenet
- ezek között milyen ok-okotati kapcsolat van?

*pl: - A vérnyomás csökkentő csökkenti-e a vérnyomást?
        - Császármetszésnöveli-e az I. típusú diabétesz kialakulását?*

**Confounding**
![császármetszés és más hatások kapcsolata az egyes típusú diabéteszre](https://www.researchgate.net/publication/348707397/figure/fig1/AS:990049109815296@1613057510555/Directed-Acyclic-Graph-theoretical-model-of-causal-association-between-childbirth-type_Q320.jpg)
Ha azt szertnénk nézni, hogy a császármetszés milyen kapcsoaltban áll a születendő gyermek 1. típusú diabéteszével? Ha cserélgetjük ezeket akkor is megfeleltethetőek egymásnak, ezért confounding van.

**randomizáció**
- a célunk, hogy a két elkülönített csoport csak a vizsgált célban különbözzön, ne legyen nemi/kor/stb alapú egyéb különbség, akkor sem, ha pl öszesen 30 nő és 2 férfit osztunk szét.
- a kísérleteket vakosítjuk, ha tudjuk, hogy a betegek ne tudják melik csoportba kerültek.
- ha teljesen random allokállom a cspoprtokat,akkor előfordulhat, hogy mind egy csoportba kerül!

![randomizáció](https://emj.bmj.com/content/emermed/20/2/164/F1.large.jpg)

**oksági kapcsolat:*** Az expozíciónál kitett vagy nem kitett a két tényező

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
> - majdnem 700 amerikában élő katolikus apáca felajánlotta, hogy az agyukat szövetttani vizsgálatoknak ki lehet tenni. Ezáltla egy homogén csport, a vizsgálat elindult és összehasonlították neuropatológiai szüvetben
> - Ez egy esetkontroll vizsgálat, retrospektív, cohorttal.
>
> Találtak olyan eseteket akinkek erős alzheimerük volt de a szövetük majdnem ép volt, de volt akinek nem volt ép és nem voltak tünetei.
>
> Korrleációt találtak szókincskészlettel és ezek alapján akinek gazdagabb szókincse volt később jelentkeztek nálaa tünetek.

**Torzítások:**
- az időbeli egymásutániságot az ember ok okozati dolognak hajlamos megélni
- az emlékezet másíhatja a tényeket
- számít-e hogy hol laknak a figyelt alanyok (nem, ha pl földrészekről van szó)
- ugyanazon helyről származnak a mért adatok
- mi az alany elő és utóélete
- milyen nagy a populáció

**Cross sectional:** a teljes populációban, nem is feltétlen a mintában hány beteg van(*prevalencia*), és hány új beteg jelenik meg (*incidencia*)?

**Ökonómiai tanulmányok:** Két azonos területen mért adat összehasonlítása, *pl: GDP - egészségügy / országokra lebontva*

![hierarcy of studies](https://s2.studylib.net/store/data/005488388_1-d55c7bb53c27169c2e8c7771914750a2.png)

### Gyógyszerfejlesztés fázisai
- pre-clinical research and development
  - ![phase of drug  development](https://www.phrma.org/-/media/Project/PhRMA/PhRMA-Org/PhRMA-Org/Teaser-Image/Clinical-Trial-Chart.jpg?w=768&hash=847BFF91FAFFF09919D099FC8295AE18)
- **1-4 fázis van**
  - **1.**
    - biztonságos-e a készítmény
    - kontrollált
    - gyakori mellékhatás
    - a 3 beteg egy csoportban jelemző a területre
    - dózis vizsgálat
  - **2.**
    - a maximum dózis meghatározása
    - a betegek nem egyszerre kapják a gyógszert
    - nincs kontroll (nem érdekel, hogy hánynak-e)
  - **3.**
    - van kontrollcsoport
    - törzskönvezés
    - engedélyezés folyamata
  - **4.**
    - már kinn van a piacon
    - hosszútávú mellékhaatások mérése
    - engedélyezett  
- clinical research and development
- Átszivárgás kontroll csoportból kezelt csoportba
  - **per protocol:** van egy mintám amit randomizálok `A` és `B` csoportba, A protokollal azt mondjuk, hogy az adott csoportban a kezelést úgy hasonlítjuk össze, hogy ahol tényleg megtörtént és úgy történ meg ahoy le van írva, és az alapján úgyabb két-kt csoportot alkotunk 
  - **intention to treat:** nem vesszük figyelembe a, hogy mi trörtént a két csoportban, csak az egyiket választjuk fő elemzésnek és összehasonlítjuk a másikkal

![itti vs pp](https://pbs.twimg.com/media/D1BTV9CWsAAiJKp.jpg)

## EA4

![kaplan meier plot censoring](https://miro.medium.com/max/1400/1*ATbW_NU5GMtTaCCPpfkzEA.png)![kaplan meier plot censoring](https://www.researchgate.net/profile/Avijit-Hazra-2/publication/326232846/figure/fig2/AS:666983502737413@1536032667905/A-basic-Kaplan-Meier-survival-plot-That-censoring-is-indicated-in-this-plot-by-small.png)


![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Km_plot.jpg/250px-Km_plot.jpg)

### Cox regresszió
> kihat a túlélésre: *nem*, *kor*, *stb*
>
> A végső arány amit kapunk  a hazard ratio
>
> ![hazard ratio on cox chart](https://lh3.googleusercontent.com/proxy/sj9b9pCSazyq0kXtnm7jXvOioPY-kCRjDgEcbkfhox2pE-6SNZVjL0PfH9Y4fkNcesBT7x6Q__4HjBlQesxpoMCHvLvhWQ)

### Lead time bias
> ![Lead time chart](https://i2.wp.com/first10em.com/wp-content/uploads/2018/06/777px-Lead_time_bias.png?fit=777%2C224&ssl=1)
>
> mennyien halnak meg amúgy is miután hatott a kezelés
>
> Jól látszik, ohgy attól, hogy hamarabb detektálom nem növeli meg az életminőséget.

### Immortal time bias
> egy kezelés amire várni kell valamennyit
>
> ![immortal time ](https://www.bmj.com/content/bmj/340/bmj.b5087/F2.large.jpg)

## EA5
> Ha van egy informácink a fluktuációról akkor tudunk egy mintaelem számot szmolni, és tudjuk számolni mennyi az esély arra, hogy random-e a fluktuáció?

aszignifikáns különbségek mögött fontos kérdés,hogy hány emberen végzett vizsgálat alapján.

- p érték, elütés, adatkezelés nagyobb valószínűséggel add false pozitiveot mint a mintavételi hibák

> binomiális adatgörbénél a nagyság melett a bekövetkezési esély is számít. Ha ritka eseméynt nézek akkor nem nagy a különbség kettő között törvény szerűen.

- **klinikai signifikancia:** tartalmi eltérés
- **p:** mértékegység nélküli különbség

- 3mmHG-al csökkentett magyasvérnyomás már populáció szinten eloszlása jelentős 
- pupuláció szinten az ami egyéni szinten mérési hibaként is elkönyvelhető jelentős lehet

**konfidencia intervallum**: pontebcsléshez hozzárendeltintervallum, pl:*95%os konfidencia intervallumon az érték 95%al beleesik a keresett csoportba*

> *filmmel kapcsolatos kérdések:*
> - *milyen új dolgot hallottál*
> - *hogyan és mi alapján történik döntéshozatal 1-1 kezelés kapcsán*
> - *hogyan zajlik döntéshozatal MAgarországon*
> - *mi az leőnye/hátránya*
> - *milyne kezelés lehet kiugróan költségkímélő*
> - *hogy döntöttél volna szavazáskor*
> - *mi nem hangzot el a filmben?*

## EA6 ~ regression to the mean
- a biológiai folyamatok fluktuiálnak
- ezkenek lehet trendje
- ha vágok egyet akkor az, ha egy extrém pontnál vágom el akkor azok a megigyelések amik alatta vannak közelebb lesznek az átlaghoz.

![](https://ars.els-cdn.com/content/image/1-s2.0-S0735109716351099-gr6.jpg)

Ha egy beteg állapotot nézünk akkor az minidg egy kicsit extrém, tehát ha beteg akkor az ő bináris állapotát valamilyen folytonos mennyiségből származtatt bináris álllapotokra vonatkoztatjuk.

*Pl:*
- *vérnyomás*
- *depresszió*
- *fájdalom*

A variabilitással mérhetjük az időbeli változását

## placebo hatás
> no intervention = regression to the mean"
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
> a kockázata másmilyen, mint a mi áltlaunk mért populáció akkor ***nem reprezetnatív a mintánk egészségügyi szmepontból***  

***Minden statisztikai vizsgálat a vizsgált szmepont alapjn kell reprezentatív legyen.***

Risk ratio: mekkora esélyem van a másik csoportban meggyógyulni, azaz a `treated/control`:  `megtörtént/1`
odds ration: mekkora esélyem arra, hogy odds skálán meggyógyuljak `p/(1-p)`, azaz kiszámolom ezt a törtet mindkét csoportra majd a kettőt elosztjuk `megtörtént/(1-megtörtént)`

![odds vs risk](https://assets.cureus.com/uploads/figure/file/138481/lightbox_65ee62a0db3611eaafa31b2789baa093-fig-1-odds-vs-prob.png)

ARR = absolute risk reduction =  a két risket kivonom egymásból
RD = risk differnece

A kezelés odds ratioja átvihető egyik populációról másikra!

Ha kontextusa más a mérésnek és a viszonyított populációnak, így más lesz a végeredmény.

Ha a populációban jelentős a különbésg valamilyen téren akkor jó eyélel nem lesz megfelelő egy másik populációra, *pl: ezért más a koncnetráció megy más génállományú betegekbe*

A nem reprezentativitás a cska a háttérkokckázat szempontjából számít.

> *zh kérdés Mi a három hatás ami megjelenhet a csoportoknál: regression to the mean, placebo hatás, kezelés hatása*
> *kivétel: interakció, más a populáció, más a kezelés*
