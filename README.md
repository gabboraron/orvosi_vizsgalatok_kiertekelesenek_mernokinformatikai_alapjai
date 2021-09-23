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


