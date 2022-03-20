Gondolatok a járvány elleni védekezés értékeléséről, és a járvány
hatásának vizsgálatáról
================
Ferenci Tamás

-   [Egy gondolkodási keret, és a confounding mindent átható
    problémája](#egy-gondolkodási-keret-és-a-confounding-mindent-átható-problémája)
-   [Egy előkészítő pont: kimenet
    megválasztása](#egy-előkészítő-pont-kimenet-megválasztása)
-   [Az elméleti megalapozás: kauzális diagram egy járvány
    hatására](#az-elméleti-megalapozás-kauzális-diagram-egy-járvány-hatására)
-   [Technikai részletek](#technikai-részletek)
-   [Az empirikus vizsgálat lehetőségei és
    nehézségei](#az-empirikus-vizsgálat-lehetőségei-és-nehézségei)
    -   [A confounding problémája](#a-confounding-problémája)
    -   [Kihagyott változós torzítás](#kihagyott-változós-torzítás)
    -   [A regresszió eszköze](#a-regresszió-eszköze)
    -   [Több változó modellezése](#több-változó-modellezése)
    -   [A változószelekció kérdésköre](#a-változószelekció-kérdésköre)
    -   [A kényelmetlen tudomány](#a-kényelmetlen-tudomány)
-   [Záró gondolatok](#záró-gondolatok)

*“Ne fogjon senki könnyelműen*  
*A húrok pengetésihez!*  
*Nagy munkát vállal az magára,*  
*Ki most kezébe lantot vesz.*

*(Petőfi Sándor: A XIX. század költői)*

------------------------------------------------------------------------

E pillanatban Európa a koronavírus-járványt lényegileg lezártnak
tekinti. Noha a dolog véglegességében azért van még kérdőjel, az alkalom
tökéletesen megfelelő arra, hogy feltegyünk két olyan kérdést, melyek
legjobban visszatekintve válaszolhatóak meg, egy járvány végén
relevánsak – de akkor viszont nagyon is. (Ebben a dolgozatban az ,,a
járvány’’ kitétel alatt a COVID-19 járványt értem, de az elmondottak
lényegében teljesen általánosak, és más esetre is alkalmazhatóak.)
Jelesül:

-   Hogyan értékeljük egy ország járványügyi intézkedéseit? Megfelelő
    lépéseket hoztak és a kellő időben? Jó volt a járványügyi rendszer,
    a tesztelés, a korlátozó intézkedések, a tájékoztatás vagy lehetett
    volna jobban is eljárni?
-   Mi hat arra, hogy a járvány egy adott országban mekkora pusztítást
    végez? Miért van az, hogy valahol ez nagyobb, máshol viszont kisebb,
    adott esetben akár jóval kisebb? Mik a közreható tényezők, és
    melyiknek mekkora a szerepe?

Mostani írásom egyik első állítása az lesz, hogy a két kérdés(csoport)
valójában szorosan összefügg, sőt, lényegében ugyanarról a
problémakörről szólnak.

A kérdéskör rendkívüli fontosságát az adja, hogy nem csak „tudományos
szempontból“ releváns, hanem a hétköznapi beszédben, politikai vitákban,
közéleti diskurzusban is lépten-nyomon, és nagy súllyal kerül elő:
Magyarországon sikeres volt a járvány elleni védekezés! Magyarországon
sikertelen volt a járvány elleni védekezés! A kormány megfelelő
intézkedéseket hozott! A kormány megkésetten és nem elégséges
intézkedéseket hozott! Magyarországon sokan haltak meg a járvány miatt!
Magyarországon nem haltak meg sokan a járvány miatt! Magyarországon
sokan haltak meg a járvány miatt, de ez nem a kormány hibája, hanem a
lakosság egészségi állapotán múlt!

E kérdések megválaszolását számos irányból kísérelhetjük meg:
használhatunk járványügyi megfontolásokat, biológiai modelleket,
epidemiológiai elméleteket és így tovább, én azonban most egyetlen
módszerrel fogok foglalkozni: az *empirikus* vizsgálattal, vagyis amikor
a begyűjtött tényadatok alapján próbáljuk megválaszolni ezeket a
kérdéseket. Gyakori vita tárgya ennek pontos szerepe, ám e kérdésben –
mind tudományosan, mind a közvélemény előtt – a legmegbízhatóbb
módszerként tűnik fel az empirikus kutatás.

Előre megmondom, hogy az írásomnak nem az a célja, hogy „végeredményt
hirdessen“. Sokkal inkább a módszerekre akarok fókuszálni, helyesekre és
hibásakra egyaránt, bemutatva a megfelelő eljásárokat, és – különös
hangsúllyal – a tipikus csapdákat és buktatókat is. Remélem, hogy ezzel
hozzá tudok járulni a már most is zajló, és – az előbb említett
megbízhatóság miatt – várhatóan a jövőben sem elhalkuló viták
színvonalának emeléséhez. Aggodalomra ugyanis lehet okunk e téren: a
téma jellegéből adódóan lényegében óhatatlan a politikai szempontok
szerinti értelmezése az adatoknak (ami soha nem tesz jót), de hiszek
benne, hogy a tudományos szempontok hozzáférhető összefoglalása segít a
diskurzus javításában.

A keretes szerkezet kedvéért elmondom az egyik utolsó állításomat is: a
kérdést rendkívül nehéz megválaszolni empirikusan, tehát a különböző
országok tényadatai alapján következtetve. Bár megpróbálok helyes
vizsgálati módszereket bemutatni, és lehetőségeket a nehézségek
enyhítésére, a kérdésre nem lehet egyszerű és perdöntő választ adni.
Mégis, azt gondolom, hogy ennek ellenére nem haszontalan végiggondolni a
problémát, sőt – részint mert segít elkerülni a tipikus csapdákat,
buktatókat, téves következtetéseket, részint pedig a probléma jó
megértése, átlátása néha még értékesebb is, mint egy egyszerű
eredményközlés.

## Egy gondolkodási keret, és a confounding mindent átható problémája

Az első állításom tehát az, hogy a két kérdéscsoport lényegében
ugyanazon probléma megoldását teszi szükségessé. Ennek megértéséhez
kezdjük az első kérdéssel. A probléma ennek kapcsán nyilvánvaló: annak
eldöntéséhez, hogy „jó“ volt-e a járvány kezelése, muszáj valahogy
definiálni, hogy mit értünk „jó“ alatt. Ezt legtermészetesebben úgy
lehet megtenni, amit angolul counterfactual, magyarul a – kissé furcsán
ható – tényellenes szóval szoktak jellemezni: megnézzük, hogy a járvány
ideális kezelése esetében mi lett volna a kimenet, és ehhez hasonlítjuk
a tényleges kimenetet. (Ez is mutatja, hogy a kérdés nem triviális:
lehet olyan helyzet, hogy 10 halott nagyon rossz kezelést jelent és az
1000 jót – ha az ideális esetben az első helyzetben 1 lett volna, a
másodikban pedig 999.) Igen ám, de mi az, hogy „ideális kezelés“?
Amennyiben van időgépünk, akkor ez semmiféle problémát nem jelent:
visszamegyünk időben, próbálkozunk más döntésekkel, és megkeressük, hogy
melyik a legjobb. Időgép híján azonban gondban vagyunk. Mihez
viszonyítsunk? Az egyetlen épkézláb, empirikusan vizsgálható
viszonyítási pontot az jelenti, hogy *más országokban* mi a helyzet
(feltéve, hogy nem mindenki pontosan ugyanúgy kezelte a járványt),
csakhogy ez elég problémás viszonyítási pont: más országok ezernyi,
milliónyi egyéb tényezőben is eltér(het)nek tőlünk azon túl, hogy
máshogy kezelték a járványt, mint mi – ha találunk is különbséget a
végeredményben, a járvány okozta pusztítás méretében, honnan tudjuk,
hogy ez mennyiben tudható be az eltérő kezelésnek, és mennyiben az egyéb
különbségeknek? Ha valahol kevesebb halott van, az azt jelenti, hogy ott
jobban kezelték a járványt? (És így nézzük azt, hogy mit csináltak
másképp?) Mi van, ha ugyanolyan jól kezelték a járványt, csak fiatalabb
a korfájuk, és ezért lett kevesebb halálozásuk? Mondok még jobbat: mi
van, ha rosszabbul kezelték a járványt, csak annyival fiatalabb az
ottani lakosság, hogy ez többet javított, mint amennyit a rosszabb
kezelésük rontott…?

Itt térhetünk át a második kérdésre, illetve arra, hogy miért ugyanaz
lényegében a kettő. A fenti okfejtés ugyanis egy speciális esete egy
általános kérdésnek: annak, hogy milyen tényezők befolyásolták, és
milyen mértékben a járvány hatását egy adott országban. Azért speciális
eset, mert leszűkítettük a kérdést egy tényezőre, a járvány kezelésének
jóságára. De nem muszáj ezt a leszűkítést megtennünk, nyugodtan
vizsgálhatjuk általában (sőt, mint majd látni fogjuk, vizsgálnunk is
*kell*, a speciális kérdés jó megválaszolásához *is*), hogy milyen
tényezők alakították ki, hogy hány halálozás volt, és melyik tényezőnek
mekkora a szerepe. És ebből, mintegy mellesleg, majd azt is
kiolvashatjuk, hogy mi a helyzet a járvány kezelésének a jósága kapcsán.
Ezért mondtam, hogy elég erről a kérdésről beszélni, és ez mindkettőt
megválaszolja.

A probléma, hogy itt *pontosan ugyanabba* a problémába futunk bele, mint
az előbb. Amennyiben tudnánk egyetlen és csakis egyetlen tényezőt
változtatni, majd megnézni úgy a járvány áldozatainak a számát, akkor
meg tudnánk mondani, hogy az a tényező hat-e rá, és ha igen, milyen
mértékben. De a probléma ugyanaz: ezt csak időgéppel lehet megtenni, ha
vissza tudnánk menni az időben, és pontosan egy dolgot megváltoztatni.
(Azért mondok időgépet, hogy látszódjon: az egyetlen dolgon kívül
*minden más* változatlanul marad.) Jelen tudásunk szerint e megoldás
kivitelezése technikai nehézségekbe ütközik, így visszajutunk ugyanahhoz
a gondolathoz: nézzünk e helyett különböző országokat, amik a vizsgált
tényezőben eltérnek. Mondjuk, ha az érdekel minket, hogy a 100 ezer
lakosra jutó nővérek száma hogyan hat a halálozásra, akkor vegyünk
országokat, ahol ez a szám – az egyszerűség kedvéért kereken mondva –
2000, és vegyünk olyanokat, ahol csak 1000, majd hasonlítsuk össze a
járvány-halálozást. De a probléma ugyanaz: mi van, ha a 2000-es, tehát
jobb nővér-ellátottságú országokban egyúttal mondjuk az elhízottak
aránya is alacsonyabb? Azért hoztam épp ezt a példát, mert ez is a
kisebb halálozás irányába hat. Innen kezdve, ha azt is találjuk, hogy a
2000-es országokban kisebb a halálozás, honnan tudhatjuk, hogy az
tényleg a több nővér miatt van? Mi van, ha valójában a nővéreknek a
világon semmi szerepe, csak ezekben az országokban kevesebb az elhízott,
és *ez* a valódi oka annak, hogy ott kisebb a halálozás?

Ezt a problémát szokták úgy hívni angol szóval, hogy confounding.
(Angolul nagyon találó kifejezés: szó szerint „egybemosódást“ jelent, és
valóban arról van szó, hogy a különböző tényezők hatása egybemosódik, a
több nővér egybemosódik a kevesebb elhízottal. Magyarra leginkább
„zavaró vátozós hatásként“ szoktak fordítani, csak sajnos ez jóval
nyakatekertebb, mint az angol kifejezés.) Ez egy általános probléma, ami
akkor jelentkezik, ha adott tényező szerint eltérő csoportokat
hasonlítunk össze, de azok a csoportok más tényezőkben is el fognak
térni – innen kezdve, ha találunk is különbséget a kimenetben, nem lehet
tudni, hogy az mi miatt van: az általunk vizsgált eltérés miatt, a vele
együtt járó egyéb eltérés(ek) miatt, vagy ezek valamilyen keveréke
miatt. A fenti példából is látható módon leginkább úgy ragadható meg a
probléma, hogy van egy – vagy több – háttérben lévő változó, a példában
mondjuk a gazdasági fejlettség, ami *egyszerre* függ össze a vizsgált
tényezővel (fejlettebb országokban több a nővér) *és* hat a kimenetre
(fejletebb országokban kevesebb az elhízott, ami szintén csökkenti a
halálozást).

A probléma általánosságából adódóan számos más területen fellép,
orvostudománytól a közgazdaságig
([videó-előadás](https://www.youtube.com/watch?v=dYt6vqqdtYQ), [írott
jegyzet](https://tamas-ferenci.github.io/FerenciTamas_AzOrvosiMegismeresModszertanaEsAzOrvosiKutatasokKritikusErtekelese/az-empirikus-megismer%C3%A9s-alapgondolata-%C3%A9s-a-confounding.html)).

Érdemes megjegyezni, hogy *elvileg* van mód a probléma megoldására
időgép nélkül is: az, ha tudunk
[randomizálni](https://tamas-ferenci.github.io/FerenciTamas_AzOrvosiMegismeresModszertanaEsAzOrvosiKutatasokKritikusErtekelese/a-confounding-megold%C3%A1sai-megfigyel%C3%A9s-%C3%A9s-k%C3%ADs%C3%A9rlet.html).
Ez azt jelenti, hogy fogjuk a vizsgálat tárgyát képező alanyokat, és
pénzfeldobással két csoportba sorsoljuk őket, az egyik a vizsgált
tényező egyik értékét kapja, a másik a másikat, majd ezeket hasonlítjuk
egymáshoz. Ez könnyen elképzelhető – és meg is valósítható – egy
gyógyszer kipróbálásánál: az „egyik érték“, hogy kap gyógyszert, a
másik, hogy nem. Ezt valóban kioszthatjuk pénzfeldobással. És ez
csakugyan fontos is: ha nem ezt tennénk, hanem mondjuk az orvosokra
bízzuk, hogy belátásuk szerint adjanak bizonyos betegeknek gyógyszert,
másoknak pedig nem, akkor azonnal jönne ugyanaz a probléma – mi van, ha
inkább a súlyosabb állapotúaknak adják a készítményt, vagy pont, hogy az
enyhébb eseteknek? A randomizálás megoldja ezt a problémát: ha
pénzfeldobással soroltuk őket csoportokba, akkor *biztosan* nem lehet
*semmilyen* tulajdonságukban szisztematikus különbség. (Különösen
fontos, hogy ez azt is jelenti, hogy azokban a tulajdonságokban sem,
amikről nincs információnk, sőt, azokban sem, amikről eszünkbe sem
jutott, hogy confounding-ot okozhatnak!) Ehhez azonban arra van szükség,
hogy mi tudjuk irányítani, meghatározni, hogy ki milyen tényezőnek van
kitéve; az ilyen vizsgálatokat szokás kísérletes kutatásnak nevezni.

A mostani esetünkben ez nyilván szóba sem jön: nem lehet pénzfeldobással
kisorsolni, hogy melyik országban legyen 1000 nővér és melyikben 2000.
Marad az, hogy nézzük a tényadatokat – csak épp ott, szemben a kísérlet
példájával, a nővérek száma már összefügghet más jellemzőkkel is. Az
ilyen vizsgálatokat szokás [megfigyeléses
vizsgálatnak](https://tamas-ferenci.github.io/FerenciTamas_AzOrvosiMegismeresModszertanaEsAzOrvosiKutatasokKritikusErtekelese/a-confounding-megold%C3%A1sai-megfigyel%C3%A9s-%C3%A9s-k%C3%ADs%C3%A9rlet.html)
nevezni. Az ilyen típusú vizsgálatoknál, általában is, nem csak ennél a
példánál, a confounding egy mindent átható probléma, olyan értelemben,
hogy folyamatosan, minden elemzési lépésnél gondolnunk kell rá, mert
Damoklész kardjaként lebeg mindig a fejünk felett.

## Egy előkészítő pont: kimenet megválasztása

A fenti leírásban implicite feltételeztem, hogy a járvány hatását a
halálozásban mérjük. A mostani dolgozat fő kérdése nem ez lesz, de azért
pár gondolat erejéig érdemes erről a választásról is beszélni.

Először is, az önmagában választás kérdése, hogy egyáltalán a halálozást
használjuk mérőszámként, kimenetként. Ez nem egyértelmű: a „járvány
terhe“, a „járvány okozta pusztítás“ egy sokdimenziós fogalom, azaz sok
szempont szerint mérhető. Terhe a járványnak természetesen és mindenek
előtt, hogy emberek halnak meg miatta, de az is teher, hogy szenvednek
tőle (még ha túl is élik), teljesen más szempontból de az is teher, hogy
kiesnek a munkából, az is teher, hogy ha maradványtünetekkel gyógyulnak,
az is teher, hogy az egészségügyi ellátórendszer kapacitásait igénybe
veszik stb. stb. Ezek ráadásul nem is feltétlenül egy irányba mutatnak,
elképzelhető, hogy egyik ország egyik dimenzió szerint jobb, de a
másikban rosszabb, egy másik ország még épp fordítva.

Mégis, a halálozási szám használata a járvány terhének mérésére elég
univerzális, és sok szempontból indokolható. Egyrészt a legnagyobb súlyú
és legdrámaibb vetület, másrészt általában azért jól korrelált a többi
szempont is vele (még ha nem is tökéletesen, ahogy az előbbi megjegyzés
is mondta), harmadrészt az egyik legbiztosabban mérhető mutató
(gondoljuk meg mennyivel nehezebb lenne azt megmondani, hogy hány
munkaóra esett ki a járvány miatt, de igazából még azt is, hogy hány
fertőzött volt – ne feledjük, hogy azok száma rettenetesen függ a
tesztelési intenzitástól). Valójában persze a halálozási mutató is
elrejt szempontokat, például azt, hogy milyen életkorban történik a
halálozás, vagy milyen egészségi állapotú alanyban, egyszóval az
elvesztett életévek számának
[problémáját](https://link.springer.com/article/10.1007/s10654-021-00774-0),
de most ezt is utaljuk egy másik vizsgálódás témakörébe.

A második kérdéskör, hogy a halálozást hogyan mérjük. Nagyon
kézenfekvőnek látszik a jelentett halálozás használata (hát az épp az,
hogy hány halálozás volt, nem?), de sajnos ez sem ilyen egyszerű: a
jelentett halálozási számokat is befolyásolja a tesztelési aktivitás
(még ha kevésbé is, mint a jelentett fertőzött-számot) és a haláloki
besorolásra alkalmazott definíciók. Ezek megnehezíthetik az országok
összehasonlítását, de adott esetben akár egy országon belül is
változhatnak időben. E kérdések önmagukban is nagyon érdekesek, itt most
csak utaltam a problémára, de egy [másik
írásom](https://github.com/tamas-ferenci/ExcessMortEUR#a-t%C3%B6bblethal%C3%A1loz%C3%A1si-mutat%C3%B3r%C3%B3l-%C3%A1ltal%C3%A1ban)
részletesen bemutatja a problémát.

Ez a gond vezet el egy másik mutatóhoz: az úgynevezett
többlethalálozáshoz. Itt a járvány előtti adatokat használva
statisztikai úton készítünk egy előrejelzést a halálozások számára, ezt
tekintjük úgy – mivel a járvány hatása nélküli adatokból készült – mint
az a halálozás ami akkor lett volna, ha nincs járvány. Kivonva ezt az
értéket a tényleges halálozási adatból, kapjuk a többlethalálozást. E
mutató hatalmas előnye, hogy biztosan semennyire nem függ a tesztelési
aktivitástól és biztosan semennyire nem függ a haláloki besorolástól.
Hátránya azonban – azon túl, hogy a leglassabban ismertté váló mutató –
egyrészt, hogy függ az előrejelzés jóságától, de még inkább az, hogy egy
bruttó jellegű mutató: egybeméri a járvány direkt hatásaival (belehalnak
emberek) annak indirekt hatásait is, amik ráadásul egyaránt lehetnek
pozitívak és negatívak. Pozitív indirekt hatás, hogy az intézkedések
mondjuk az influenza ellen is jót tesznek, de kicsit elengedve a
fantáziánkat, az is pozitív indirekt hatás lehet, hogy kevesebb
autóbaleset történik. Negatív indirekt hatás, hogy más betegség ellátása
nehezedik meg vagy lehetetlenül el, de itt is lehet távlatibb kérdésekre
gondolni, például mi van, ha megnő az öngyilkosságok száma a szociális
elszigetelődés miatt. A többlethalálozás nem teszi lehetővé ezek biztos
elkülönítését. Itt is igaz, hogy e problémakör önmagában több oldalnyi
tárgyalást igényelne, ami az [említett
írásomban](https://github.com/tamas-ferenci/ExcessMortEUR#a-t%C3%B6bblethal%C3%A1loz%C3%A1si-mutat%C3%B3r%C3%B3l-%C3%A1ltal%C3%A1ban)
megtalálható, itt megint csak a címszavakban összefoglalásra
szorítkoztam. Egyetlen
[megállapítást](https://github.com/tamas-ferenci/ExcessMortEUR#%C3%B6sszevet%C3%A9s-a-jelentett-hal%C3%A1loz%C3%A1ssal)
emelnék ki: Európán belül öt országtól (Bulgária, Románia, Litvánia,
Lengyelország és félig-meddig Szlovákia) eltekintve a két mutató értékei
nagyon hasonlóak egymáshoz.

Ez azért is fontos, mert azt mondja, hogy – szerencsére – a két mutató
közti választás nem várható, hogy nagy hatást gyakoroljon a
végeredményre. Így különösebben sokat nem kell gondolkozni azon, hogy
melyiket választjuk, én most a többlethalálozást fogom használni a teher
végső mutatójaként, azért, mert az empirikus elemzés különböző országok
adatait fogja egybevetni, így fontos, hogy országok között robusztusan
összehasonlítható mutatót használjunk.

Ennek az értékei így néznek ki a 2021. 52. heti állapot szerint (ezt az
indikátort nagy késleltetéssel közlik, így sokat visszamegyünk, hogy a
lehető legtöbb országra legyen adatunk):

``` r
RawData <- fread("https://github.com/tamas-ferenci/ExcessMortEUR/raw/main/ExcessMortEUR_data.csv",
                 dec = ",")[time=="2021W52"&nuts_level==0]
RawData$cumexcessperpop <- RawData$cumexcess/RawData$meanpopulation*1e6
ggplot(RawData[order(cumexcessperpop)],
       aes(x = factor(geo, levels = geo), y = cumexcessperpop, fill = geo=="HU")) +
  geom_col() + guides(fill = "none") + labs(x = "", y = "Összesített többlethalálozás [fő/1M fő]")
```

![](README_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

Az rögtön látszik, hogy Magyaroszág az utolsó harmad elején található;
arról persze ez még nem nyilatkozik, hogy ennek mi az oka – pontosan ezt
próbáljuk most felderíteni.

## Az elméleti megalapozás: kauzális diagram egy járvány hatására

Az ember ezen a ponton késztetést érezhet arra, hogy rögtön el is kezdje
nézni az empirikus adatokat: melyik országban mekkora volt a teher (azaz
a többlethalálozás)? Összefügg ez a nővérek számával? A gazdasági
fejlettséggel? Az intézkedések szigorúságával? Az elhízottak arányával?
A korfával?

Mielőtt azonban ebbe belevágunk, némi óvatosságot javasolok. Az ilyen
„mindent mindennel“ típusú, elméleti megalapozás nélküli „összevissza“
nézegetéseken alapuló adatbázis-masszírozások általában nem sok jóra
vezetnek. Ennek a későbbiekben egy sor konkrét okát bemutatom, de most
fontosabb egy általános, mondhatni filozofikus gondolat: az ilyen típusú
empirikus vizsgálatoknak mindig a háttérben lévő elméleti *jó*
megértésén kell alapulnia. Nem egyszerűen azért, mert azt alaposan
végiggondolva kap jó rálátást az ember a problémára, hanem azért is,
mert – pont emiatt – ez teszi lehetővé jobb empirikus modellek
készítését is.

Egyelőre tehát – és én azt gondolom, hogy általában is ez a jó
hozzáállás – ne nyúljunk hozzá semmilyen adathoz. Ehelyett próbáljuk meg
először a fejünkben összeszedni, végiggondolni, és strukturálni a
kérdést: milyen tényezők alakítják, hogy hányan halnak meg egy országban
a járvány alatt?

Legfelső szinten függ attól, hogy (A) hányan fertőződnek meg és (B) a
megfertőződöttek milyen arányban halnak meg. Világos, hogy annál több
halálozás lesz, minél több a fertőzött, illetve ha a fertőzöttek minél
nagyobb arányban halnak meg. (Vagy, természetesen, mindkettő egyszerre.)
Legfelső szinten így dekomponálhatjuk a problémát.

Menjünk tovább. Eggyel lejjebb haladva az ‘A’ megint két tényezőtől
függ: hogy milyen a kontaktusszám az országban és milyenek az ezt
csökkentő intézkedések. Ezek aztán megint tovább bonthatóak. Az előbbi
függ a népsűrűségtől, a lakásviszonyok zsúfoltságától, az érintkezésre
vonatkozó szociális szokásoktól és hagyományoktól, a különböző
generációk együttélési mintázataitól, a szabadidős tevékenységek
jellegétől, a városi lakosság arányától, a munkavégzés
jellegzetességeitől stb. stb. Számíthat még az ország bekötöttsége a
nemzetközi turizmusba, kereskedelembe, a népmozgás intenzitása. Az
utóbbi függ az intézkedések szigorúságától, időbeniségétől, betartásuk
fegyelmétől, a tesztelési, kontaktuskutatási, karanténozási
stratégiától, a járványügy szervezettségétől, hitelességétől stb. stb.

A ‘B’ tényező megint csak két részre bontható: függ az alanyok olyan
jellemzőitől, amik befolyásolják a prognózist egyrészt, másrészt az
ellátásuk hatékonyságától. Az előbbi megint rengeteg tényezőre bontható
tovább: mindenekelőtt számít az életkori összetétel, tehát a korfa, de
ott van az elhízás, a dohányzás prevalenciája, az alkoholfogyasztás
mennyisége, a releváns társbetegségek – ez önmagában több tucat –
prevalenciája, ami szintén eltérhet országok között. A medikális
beavatkozás megint kettéválik: egyik oldalról számít az oltási program
(az oltóanyag portfólió összetétele és az átoltottság), másik oldalról a
kezelési oldal. A gyógyszerek elérhetősége, felhasználása, orvosok,
nővérek, szakdolgozók tudása, de – mindenekelőtt – a túlterhelődésük.
Az, hogy az ellátás mennyire zajlik egységes irányelvek mentén, milyen a
minőségbiztosítás és a teljesítménymérés (régi vesszőparipám). Stb. stb.
stb. És akkor még nem említettem, hogy számíthat az összes felsorolt
tényező országon belüli egyenlőtlensége, ami szintén nem biztos, hogy
ugyanaz minden országban.

Láthatjuk, hogy a cél az ilyen végiggondolásnál nem is feltétlenül az,
hogy minden egyes tényezőt számbavagyünk az utolsó szálig, hanem sokkal
inkább, hogy a probléma *struktúráját* megértsük.

Amit a fentiekben verbálisan igyekeztem körülírni, az lényegében egy
egyszerűsített változata annak, amit kauzális diagramnak szoktak
nevezni:

![](README_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

A valóságban a [kauzális diagramok](http://bayes.cs.ucla.edu/BOOK-2K/)
ennél jóval összetettebbek, itt ez némileg idézőjelben értendő, és
inkább csak egyfajta grafikus megjelenítése a fenti leírásnak. Ha csak
annyit teszünk, hogy egy ilyet felvázolunk, sokszor már az is segíti a
strukturálást és így a jobb megértést.

## Technikai részletek

A következő pontban az empirikus számításoknál az azokat megvalósító
konkrét kódokat is közölni fogom. Ennek célja az, hogy az ez után
érdeklődők azt is lássák, hogy mi történik a háttérben, milyen kódokkal
lehet kivitelezni ténylegesen ezeket a vizsgálatokat. Az ebből való
tanuláson túl az ilyen kódok közlését elvileg is fontosnak tartom, a
reprodukálhatóság és a nyílt tudomány jegyében, hogy az esetleges hibáim
könnyebben kiderüljenek, és elősegítsem továbbfejlesztési lehetőségek
megfogalmazását. Ha valakit ez a része nem érdekel a kérdésnek, bátran
ugorja át a szürke hátterű kódokat és e fejezet hátralevő részét.

A számítások `R` statisztikai programnyelven készültek, 4.1.2-es verziót
használva. Felhasználtam a `data.table` (1.14.2-es verzió) és `ggplot2`
(3.3.5-es verzió) csomagokat.

A kimeneti adat, azaz a többlethalálozási számok forrása a
‘Többlethalálozási adatok európai összevetésben’ című
[anyagom](https://github.com/tamas-ferenci/ExcessMortEUR). Ebben minden
további technikai kérdés részletesen le van írva, de egy mondatban
összefoglalva: Acosta és Irizarry
[módszerét](https://www.medrxiv.org/content/10.1101/2020.06.06.20120857v3)
használtam a többlethalálozás becsléséhez.

A potenciális magyarázó adatok forrása az egységesség és az egyszerűség
kedvéért mindenhol az [Eurostat](https://ec.europa.eu/eurostat) volt. A
következő adatokat gyűjtöttem le (nem feltétlenül fogom kivétel nélkül
mindegyiket használni a későbbiekben, de az adatbázisban rendelkezésre
áll, ha valaki szeretne tovább kísérletezni a témában):

| Változó                            | Eurostat azonosító | Év   | Mértékegység    |
|------------------------------------|--------------------|------|-----------------|
| Népsűrűség                         | tps00003           | 2019 | fő/km2          |
| Túlzsúfolt lakások aránya          | tessi170           | 2019 | %               |
| Városi lakosság aránya             | ilc_lvho01         | 2019 | %               |
| Egy főre jutó bruttó hazai termék  | nama_10_pc         | 2019 | Folyó áron, PPS |
| 65 év felettiek aránya             | demo_pjan          | 2019 | %               |
| Elhízás prevalenciája              | sdg_02_10          | 2019 | %               |
| Dohányzás prevalenciája            | hlth_ehis_sk1i     | 2019 | %               |
| Naponta alkoholt fogyasztók aránya | hlth_ehis_al1i     | 2019 | %               |
| Cukorbetegség prevalenciája        | hlth_ehis_cd1e     | 2019 | %               |
| Magas vérnyomás prevalenciája      | hlth_ehis_cd1e     | 2019 | %               |
| Asztma prevalenciája               | hlth_ehis_cd1e     | 2019 | %               |
| Koszorúér-betegség prevalenciája   | hlth_ehis_cd1e     | 2019 | %               |
| Egy főre jutó egészségügyi kiadás  | hlth_sha11_hf      | 2019 | euró/fő         |
| Ezer főre jutó nővérek száma       | hlth_rs_prsns      | 2017 | fő/ezer fő      |

Elsőként letöltjük ezeket az adatforrást, majd egy táblában egyesítjük
az összeset a későbbi felhasználás céljából. A táblát könnyen kezelhető
`csv` formátumban is mentsük ki, hogy megkönnyítsük az adatainkat
esetlegesen felhasználók dolgát:

``` r
RawData <- Reduce(function(...) merge(..., by = "geo"), list(
  RawData,
  as.data.table(eurostat::get_eurostat("tps00003"))[
    unit=="PER_KM2"&time=="2019-01-01",.(geo, popdensity = values)],
  as.data.table(eurostat::get_eurostat("tessi170"))[
    sex=="T"&time=="2019-01-01",.(geo, overcrowding = values)],
  as.data.table(eurostat::get_eurostat("ilc_lvho01"))[
    incgrp=="TOTAL"&building=="TOTAL"&deg_urb=="DEG1"&time=="2019-01-01",
    .(geo, urbanization = values)],
  as.data.table(eurostat::get_eurostat("nama_10_pc"))[
    unit=="CP_PPS_HAB"&na_item=="B1GQ"&time=="2019-01-01",.(geo, gdp = values)],
  as.data.table(eurostat::get_eurostat("demo_pjan"))[
    sex=="T"&time=="2019-01-01",.(popold = sum(values[age%in%c(paste0("Y", 65:99),
                                                               "Y_OPEN")])/values[age=="TOTAL"]*100),
    .(geo)],
  as.data.table(eurostat::get_eurostat("sdg_02_10"))[
    bmi=="BMI_GE30"&time=="2019-01-01", .(geo, obese = values)],
  as.data.table(eurostat::get_eurostat("hlth_ehis_sk1i"))[
    smoking=="NSM"&quant_inc=="TOTAL"&sex=="T"&age=="TOTAL"&time=="2019-01-01", .(geo, smoke = 100-values)],
  as.data.table(eurostat::get_eurostat("hlth_ehis_al1i"))[
    frequenc=="DAY"&quant_inc=="TOTAL"&sex=="T"&age=="TOTAL"&time=="2019-01-01", .(geo, alcohol = values)],
  dcast(as.data.table(eurostat::get_eurostat("hlth_ehis_cd1e"))[
    unit=="PC"&isced11=="TOTAL"&time=="2014-01-01"&sex=="T"&age=="TOTAL"&
      hlth_pb%in%c("ASTHMA", "HBLPR", "DIAB", "CHRT_ANGPEC"), .(geo, hlth_pb, values)],
    geo ~ hlth_pb, value.var = "values"),
  as.data.table(eurostat::get_eurostat("hlth_sha11_hf"))[
    unit=="EUR_HAB"&icha11_hf=="TOT_HF"&time=="2019-01-01", .(geo, healthexpenditure = values)],
  as.data.table(eurostat::get_eurostat("hlth_rs_prsns"))[
  unit=="P_HTHAB"&wstatus=="PRACT"&time=="2017-01-01"&isco08=="OC2221_3221",
  .(geo, nurses = values)]))
names(RawData) <- tolower(names(RawData))

write.csv2(RawData, "RawData.csv", row.names = FALSE)
```

A változók sora – mint a fenti leírás is mutatta – végeláthatatlanul
bővíthető, ez pusztán egy illusztrációs kiindulópont.

A vizsgált országok körét meghatározza az a tény, hogy mely országokra
van információnk; végeredményben 22 ország lesz az adatbázisunkban;
angol nevükkel ezek a következőek: Austria, Belgium, Bulgaria, Cyprus,
Czechia, Germany, Denmark, Estonia, Greece, Spain, Croatia, Hungary,
Italy, Lithuania, Luxembourg, Latvia, Netherlands, Norway, Poland,
Romania, Sweden, Slovenia.

A begyűjtött adataink:

``` r
knitr::kable(RawData[, c(1, 20, 21:35)], digits = 1)
```

| geo | geoname     | cumexcessperpop | popdensity | overcrowding | urbanization |   gdp | popold | obese | smoke | alcohol | asthma | chrt_angpec | diab | hblpr | healthexpenditure | nurses |
|:----|:------------|----------------:|-----------:|-------------:|-------------:|------:|-------:|------:|------:|--------:|-------:|------------:|-----:|------:|------------------:|-------:|
| AT  | Austria     |          1802.4 |      107.6 |         15.1 |         31.0 | 40350 |   18.8 |  17.1 |  26.2 |     5.7 |    4.4 |         2.2 |  4.9 |  21.1 |            4671.6 |  685.0 |
| BE  | Belgium     |          2009.9 |      377.3 |          5.7 |         29.5 | 37690 |   18.9 |  16.3 |  19.4 |     9.7 |    4.3 |         1.5 |  5.3 |  16.5 |            4418.1 | 1122.4 |
| BG  | Bulgaria    |          8374.1 |       63.4 |         41.1 |         44.8 | 17010 |   21.3 |  13.6 |  36.2 |    10.2 |    2.7 |         9.1 |  6.4 |  29.6 |             625.6 |  437.5 |
| CY  | Cyprus      |           855.1 |       95.7 |          2.2 |         51.8 | 29400 |   16.1 |  15.2 |  25.5 |     4.0 |    4.3 |         1.6 |  6.1 |  17.3 |            1771.2 |  538.1 |
| CZ  | Czechia     |          3851.9 |      138.2 |         15.4 |         30.0 | 29760 |   19.6 |  19.8 |  26.4 |     7.8 |    4.5 |         4.3 |  7.7 |  23.7 |            1644.1 |  850.1 |
| DE  | Germany     |           932.0 |      235.2 |          7.8 |         36.3 | 38650 |   21.5 |  19.0 |  28.3 |     7.5 |    6.1 |         3.9 |  7.2 |  28.5 |            4855.3 | 1312.7 |
| DK  | Denmark     |           322.1 |      138.5 |         10.0 |         37.6 | 40750 |   19.6 |  16.5 |  20.0 |     9.6 |    6.5 |         1.9 |  4.6 |  17.7 |            5355.1 | 1003.0 |
| EE  | Estonia     |          2219.3 |       30.5 |         13.9 |         61.0 | 26330 |   19.8 |  21.8 |  24.8 |     1.3 |    3.1 |         5.6 |  5.5 |  22.9 |            1426.0 |  619.2 |
| EL  | Greece      |          2309.8 |       82.4 |         28.7 |         36.9 | 21080 |   22.0 |  16.7 |  28.6 |     5.9 |    4.4 |         3.4 |  9.2 |  20.9 |            1340.8 |  330.9 |
| ES  | Spain       |          1799.7 |       93.8 |          5.9 |         49.6 | 28980 |   19.4 |  16.0 |  22.1 |    13.0 |    4.5 |         0.8 |  6.8 |  18.7 |            2411.7 |  573.6 |
| HR  | Croatia     |          3808.6 |       72.8 |         38.5 |         29.6 | 21200 |   20.6 |  23.0 |  25.7 |    10.2 |    3.0 |         5.1 |  7.1 |  24.6 |             930.6 |  656.0 |
| HU  | Hungary     |          3534.0 |      107.1 |         20.3 |         32.8 | 23280 |   19.3 |  24.5 |  27.2 |     6.3 |    4.9 |         4.9 |  8.1 |  31.9 |             949.4 |  651.2 |
| IT  | Italy       |          2735.8 |      201.5 |         28.3 |         35.3 | 30820 |   22.9 |  11.7 |  22.4 |    12.1 |    4.8 |         2.5 |  6.7 |  20.6 |            2599.2 |  579.8 |
| LT  | Lithuania   |          4772.7 |       44.6 |         22.9 |         43.2 | 26770 |   19.8 |  18.9 |  23.7 |     0.8 |    2.7 |         7.5 |  4.4 |  28.1 |            1223.8 |  770.8 |
| LU  | Luxembourg  |           458.4 |      239.8 |          7.1 |         19.6 | 81300 |   14.4 |  16.5 |  18.2 |     8.9 |    6.8 |         2.5 |  5.6 |  16.5 |            5502.1 | 1172.5 |
| LV  | Latvia      |          3108.7 |       30.2 |         42.2 |         43.8 | 22150 |   20.3 |  23.0 |  26.8 |     1.2 |    3.5 |         6.6 |  4.7 |  29.4 |            1045.6 |  456.8 |
| NL  | Netherlands |          1595.6 |      507.3 |          4.8 |         56.2 | 40980 |   19.2 |  14.7 |  21.1 |     8.3 |    5.5 |         1.9 |  5.4 |  16.8 |            4748.7 | 1093.6 |
| NO  | Norway      |           514.0 |       17.3 |          6.1 |         28.9 | 46390 |   17.2 |  14.1 |  18.1 |     1.4 |    6.7 |         1.7 |  4.2 |  12.7 |            7126.7 | 1766.2 |
| PL  | Poland      |          4352.6 |      123.6 |         37.6 |         35.0 | 23220 |   17.7 |  19.0 |  22.6 |     1.6 |    4.1 |         9.0 |  6.6 |  23.1 |             906.1 |  510.1 |
| RO  | Romania     |          5967.9 |       82.7 |         45.8 |         28.8 | 22130 |   18.5 |  10.9 |  27.3 |     2.9 |    2.0 |         3.4 |  4.8 |  17.1 |             661.3 |  696.7 |
| SE  | Sweden      |          1457.1 |       25.2 |         15.6 |         40.3 | 37920 |   19.9 |  15.3 |  12.6 |     1.8 |    7.6 |         1.5 |  4.8 |  16.2 |            5041.8 | 1089.4 |
| SI  | Slovenia    |          2218.2 |      103.7 |         11.6 |         19.5 | 28240 |   19.8 |  19.9 |  23.2 |     6.6 |    5.0 |         3.2 |  6.9 |  24.8 |            1975.2 |  992.3 |

Érzékelhetőek a hatalmas különbségek: a többlethalálozás az egymillió
lakosonként 500 alattitől (Dánia) a 8000 felettiig (Bulgária) terjednek,
és több magyarázó jellegű változóban is vannak drámai eltérések,
nagyságrendi különbségek vannak a népsűrűségben, az
alkoholfogyasztásban, de még az egészségügyre fordított kiadásokban is.

## Az empirikus vizsgálat lehetőségei és nehézségei

Miután nagyon alaposan végiggondoltuk a háttérben lévő elméleti modellt,
elkezdhetünk foglalkozni azzal a kérdésből, hogy ebből mit és hogyan
tudunk empirikus adatok alapján megbecsülni (illetve mit nem).

### A confounding problémája

Először, hogy benyomást kapjunk az elemzési lehetőségekről, és azok
problémáiról, kezdjünk néhány egyszerű vizsgálattal.

Sokan mondják, hogy a kimenet összefügg a nővérek számával: ahol több
van, ott kedvezőbben alakult a járvány-halálozás. Nézzük is meg a
kérdést empirikusan! Ezt látjuk az európai országok körében:

``` r
ggplot(RawData, aes(x = nurses, y = cumexcessperpop)) + geom_point() +
  geom_smooth(method = "lm", formula = y ~ x, se = FALSE) +
  labs(x = "Ezer főre jutó nővérek száma [fő/ezer fő]",
       y = "Összesített többlethalálozás [fő/1M fő]")
```

![](README_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->

Első ránézésre teljes mértékben megerősíthetjük a felvetést: a több
ápoló valóban alacsonyabb halálozás jár együtt. A behúzott vonal a
pontokra legjobban illeszkedő egyenes; később ennek majd nagyobb
jelentősége lesz, egyelőre fogjuk fel úgy, hogy azért van ott, hogy
vezesse a szemet.

Ha figyelmen kívül hagyjuk a felvezetésben mondottakat, azaz
megfeledkezünk a confounding lehetőségéről, akkor akár le is vonhatnánk
a következtetést, hogy a nővérek száma *csökkenti* a halálozást.
(Figyeljünk a szóhasználatra! A „csökkenti“ már egy *kauzális* szó, azt
mondja, hogy okozati összefüggés van, szemben a „jár együtt“
megfogalmazással.) Csakhogy eszünkbe jut a confounding problémája: mi
van, ha a nővérek száma összefügg valamilyen más változóval, ami a
*valódi* oka a kedvezőbb adatoknak…?

Például eszünkbe jut, hogy a jobb gazdasági állapotú országokban több az
ezer főre jutó nővér. (Megengedhetik maguknak? Más az ottani felfogás a
nővérek szerepére vonatkozóan? – ez most, ilyen szempontból, mindegy
is.) Ellenőrizzük is ezt gyorsan le, a gazdasági fejlettség mérésére a
GDP-t használva:

``` r
ggplot(RawData, aes(x = nurses, y = gdp)) + geom_point() +
  geom_smooth(method = "lm", formula = y ~ x, se = FALSE) +
  labs(x = "Ezer főre jutó nővérek száma [fő/ezer fő]",
       y = "Egy főre jutó bruttó hazai termék [PPS, folyó áron]")
```

![](README_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->

Ez bejött! De akkor viszont… lehet, hogy baj van? Lehet, hogy az ápolók
száma nem is fontos, csak a fejlettségé…? Nézzük meg:

``` r
ggplot(RawData, aes(x = gdp, y = cumexcessperpop)) + geom_point() +
  geom_smooth(method = "lm", formula = y ~ x, se = FALSE) +
  labs(x = "Egy főre jutó bruttó hazai termék [PPS, folyó áron]",
       y = "Összesített többlethalálozás [fő/1M fő]")
```

![](README_files/figure-gfm/unnamed-chunk-7-1.png)<!-- -->

És akkor most tényleg bajban vagyunk.

Persze vigyázat: nem arról van szó, hogy bebizonyítottuk, hogy a nővérek
számának nincs hatása – ettől még éppenséggel lehet! Csak azt
bizonyítottuk be, hogy erre vonatkozólag az első ábra, bármennyire is
szuggerálná ezt a konklúziót, valójában nem bizonyítő erejű.

Hogy lehet ennek a kérdésnek utánajárni? Próbálkozzunk egy trükkös
ábrázolással. Ismét a nővérek száma és a kimenet közti kapcsolatot
ábrázoljuk, ugyanúgy mint a legeslő ábrán, *de* úgy, hogy megbontjuk a
GDP értékei szerint:

``` r
ggplot(RawData, aes(x = nurses, y = cumexcessperpop)) + geom_point() +
  geom_smooth(method = "lm", formula = y ~ x, se = FALSE) +
  facet_wrap(~Hmisc::cut2(gdp, g = 4)) +
  labs(x = "Ezer főre jutó nővérek száma [fő/ezer fő]",
       y = "Összesített többlethalálozás [fő/1M fő]")
```

![](README_files/figure-gfm/unnamed-chunk-8-1.png)<!-- -->

Bár az eleve sem túl nagy mintanagyság további szétosztódása miatt ez
kicsit nehezebben értelmezhető, az azért így is látszik, hogy valami
nagyon érdekes történt: míg *összességében* nézve egyértelmű és negatív
kapcsolat volt (több nővér – kevesebb halálozás), addig most ez a
kapcsolat teljesen megszűnt! Néhol egy kicsit negatív kapcsolat van,
néhol egy kicsit pozitív, ilyen mintaméretek mellett egyiknek sincs
jelentősége, nem látunk érdemi kapcsolatot sehol sem.

Ahhoz, hogy megértsük, hogy itt mi történik, gondoljuk végig, hogy az
első ábra esetében mit jelent a confounding problémája. Mi ott a
probléma? Az, hogy ha megyünk jobbra (több ápoló), akkor *egyúttal* a
gazdasági fejlettség is javul, nem csak az ápolók száma nő. Azaz, amit
látunk (csökkenő halálozás), valójában nem pusztán a több ápoló, hanem a
több ápoló *és* magasabb GDP *együttes* hatása (és nem tudjuk, hogy
milyen arányban). A probléma tehát, hogy egy változót akartunk vizsgálni
(ápolók száma), de ahogy az változik az ábrán, vele együtt valami más is
odébbmászik.

…ez a mostani ábrázolás azonban pont ezt oldja meg! Hiszen az egyes kis
részábrákban a GDP adott értékű (közelítőleg), azaz, amikor a kis
részábrákat nézzük, akkor a fenti hatást kikapcsoltuk! Ilyen értelemben
ez az ábrázolás az ápolók számának valódi hatását igyekszik megragadni,
[tisztítva](https://tamas-ferenci.github.io/FerenciTamas_AzOrvosiMegismeresModszertanaEsAzOrvosiKutatasokKritikusErtekelese/megfigyel%C3%A9ses-vizsg%C3%A1latok-a-gyakorlatban.html)
a fejlettség miatti confounding-tól. (Ezt a módszert szokás egyébként
rétegzésnek nevezni.)

Ez itt egy nagyon fontos általános gondolat: hogy egy változó hatását
úgy kapjuk meg, ha *csak* a kérdéses tényezőt változtatjuk. És most
értünk körbe, hiszen honnan indultunk? Abból, hogy az a probléma, hogy
nem tudunk „egyetlen és csakis egyetlen tényezőt“ változtatni – ezt
látjuk a fenti ábrákban megjelenni. Csakhogy most már, ezzel az utolsó
ábrával, az e probléma elleni küzdelem eszköze is kezd a kezünkbe
kerülni.

Egy pillanatra még érdemes elidőzni az ábrázolásoknál. Ez keményebb dió
lesz az eddigieknél, de kiegészítő pontként nem felesleges: egy utolsó
vizualizációt mutatok, ami az előbbieknél jobb térlátást igényel, de
megéri, ha az ember becsukja a szemét, és igyekszik meglátni maga előtt
a helyzetet, mert segíti, hogy mélyebben megértse a confounding
mibenlétét. Készítsünk egy három dimenziós ábrát! Itt természetesen nem
egyenest, hanem egy síkot illesztünk a pontjainkra (a függőleges piros
vonalak csak a síktól vett eltérést mutatják):

``` r
fit <- lm(cumexcessperpop ~ gdp + nurses, data = RawData)

gdpgrid <- seq(min(RawData$gdp), max(RawData$gdp), length = 10)
nursegrid <- seq(min(RawData$nurses), max(RawData$nurses), length = 10)
predgrid <- predict(fit, expand.grid(gdp = gdpgrid, nurses = nursegrid))

rgl::plot3d(RawData$gdp, RawData$nurses, RawData$cumexcessperpop,
            xlab = "GDP", ylab = "Nővérek száma", zlab = "Halálozás")
            # xlab = "Egy főre jutó bruttó hazai termék [PPS, folyó áron]",
            # ylab = "Ezer főre jutó nővérek száma [fő/ezer fő]",
            # zlab = "Összesített többlethalálozás [fő/1M fő]")
rgl::view3d(userMatrix = matrix(c(0.74, -0.18, 0.44, 0, 0.67, 0.23, -0.70, 0, -0.02, 0.95, 0.30,
                                  0, 0, 0, 0, 1), nc = 4))
rgl::segments3d(rbind(RawData$gdp, RawData$gdp),
                rbind(RawData$nurses, RawData$nurses),
                rbind(RawData$cumexcessperpop, predict(fit)),
                alpha = 0.4, col = "red")
rgl::surface3d(gdpgrid, nursegrid, predgrid, alpha = 0.4, front = "lines")
rgl::lines3d(c(gdpgrid[1], gdpgrid[10]), rep(nursegrid[1], 2), c(predgrid[1], predgrid[10]),
             col = "blue")
rgl::lines3d(rep(gdpgrid[10], 2), c(nursegrid[1], nursegrid[10]), c(predgrid[10], predgrid[100]),
             col = "green")
```

![](README_files/figure-gfm/unnamed-chunk-9-1.png)<!-- -->

Amit látunk, hogy a GDP–halálozás vetületben ferde a sík (nézzük a kék
élet) – ez fejezi ki azt, hogy a GDP növekedtével csökken a halálozás.
Viszont a nővér–halálozás vetületben (zöld él) szinte vízszintes – a
GDP-t is figyelembe véve már nincs hatása a nővérek számának! Ez egy
fontos megállapítás, vagy jobban mondva újabb elmondása a korábbi
megállapításnak: *ha* lerögzítjük a GDP-t, akkor a nővérek változtatása
már nem számít. Ha rögzítjük a GDP értékét, azaz kiválasztunk egy pontot
a kék él mentén, majd *adott, rögzített GDP mellett* elkezdjük
változtatni a nővérek számát, azaz a kiválasztott ponttól elindulunk a
sík mentén a nővér él növekvő irányába, akkor szinte vízszintesen
haladunk – nem változik a halálozás.

Ez egyúttal azt is jelenti, hogy a sík valami nagyon fontos dolgot tud:
annak ellenére, hogy a valódi adatokban (lévén, hogy nem kísérletről van
szó) együtt változik a két tényező, mi *mégis*, pusztán *matematikai
úton* megmondjuk, hogy mi lenne, ha csak az egyik változna. Úgy tudunk
erre válaszolni, hogy pusztán megfigyeléses adataink vannak! Erre a
gondolatra mindjárt visszatérek.

Az ábra azt is szemlélteti, hogy miért lép fel a confounding. Hiszen,
kérdezhetné a fentiek alapján valaki, akkor miért láttuk a legelső
ábránkon azt, hogy az ápolók száma és a halálozás között van
összefüggés? Egy egyértelműen negatív meredekségű egyenest tudtunk
behúzni. Most meg azt mondjuk, hogy „vízszintes“ abban az irányban a
sík, és „nem számít“ az ápolók száma…?! Akkor most vízszintes, vagy
negatív meredekségű? Számít a nővérek száma vagy sem? Az ellentmondás
csak látszólagos. Nézzük meg jobban az ábrát! A pontok nem akárhogy
helyezkednek el a síkon: alapvetően a jobb alsó sarok – bal felső sarok
átló mentén szóródnak. (Ez fejezi ki azt, hogy a GDP és a nővérek száma
*egymással is összefügg*!) Azaz amikor mi csak a nővéreket vizsgáltuk,
akkor nem *pusztán* balról jobbra haladtunk a nővér tengely mentén,
hanem *egyúttal* jöttünk fentről is le! És itt van a magyarázat: ezért
láttuk úgy, hogy van összefüggés, és negatív a kapcsolat, hiszen ez
utóbbi, a fentről lefelé jövés okozta a csökkenő halálozást.

Tudom, hogy mindez elég agyzsibbasztó, és valószínűleg kell rá aludni
egyet (többet), ha valaki először látja, de e kép megértése sokat segít
a confounding átlátásában és a megoldás megtalálásában is.

### Kihagyott változós torzítás

Valamit nagyon fontos megérteni részleteiben is a confounding problémája
kapcsán: ha kihagyunk egy lényeges változót, tehát olyat, aminek
*valójában* van hatása a kimenetre, akkor annak a hatását a bentmaradt
változók veszik át. (Attól a gyakorlatban nem túl izgalmas esettől
eltekintve, ha egyik vizsgált változóval sem függ össze a kihagyott.)
Ezt szokták kihagyott változó okozta torzításnak nevezni.

Ha meggondoljuk, akkor ez a fenti, két magyarázó változót tartalmazó
példán is tökéletesen elmondható: ha kihagyjuk a GDP-t, akkor a nővér
változó valójában már nem *csak* a nővérek hatását fogja mutatni, hanem
a nővérek *és* a GDP együttes hatását. A nővér változó, legalábbis
részben, *átvette* a GDP szerepét is! Általánosan megfogalmazva: a
vizsgált változóinkra kimutatott hatások – sajnos – a nem vizsgált
változók hatásait (is) tartalmazzák, ha nem vizsgáltunk olyat, ami
valójában lényeges.

Bár tényleg csak átfogalmazásról van szó, azért fontos külön is
említeni, mert egy gyakori tévedés, ha egy nem vizsgált változóról
automatikusan kijelentjük, hogy nincs hatása. Ez nem csak hogy nem igaz,
de a helyzet rosszabb: ezt a hatást, ha van neki, sajnos a vizsgált
változókra szétosztva fogjuk kimutatni…! Ha a társadalmi
távolságtartásra vonatkozó szokásokra nincs adatunk (hogy mondjak egy
csakugyan nehezen mérhető változót), akkor nem mondhatjuk, hogy annak
nincs hatása, de ez még hagyján, az igazi baj, hogy a hatását, ha van
neki, a többi változóban fogjuk elszámolni, mert azok *átveszik* a
kimaradt változó hatását. Ha például a déli országokban szorosabbak a
szociális kontaktusok mint az északiakban, *és* a déliek és az északiak
között GDP-ben is van eltérés, akkor a szociális távolság hatását
vidáman ki fogjuk mutatni GDP címszó alatt!

A kihagyott változó okozta problémák legegyszerűbb kezelési megoldása
elég kézenfekvő: ne hagyjunk ki lényeges változót… A dolog azonban nem
ilyen egyszerű, két okból sem. Az egyik, kézenfekvő probléma, hogy mi
van, ha nincs információnk a lényeges változóról? Akár azért, mert nem
tudtuk begyűjteni az információt, akár azért, mert nem is gondoltunk rá,
hogy be kellene gyűjteni! (Ugye ez a kísérletes vizsgálatok nagy
előnye.) Megjegyzem, jelen esetben az információ begyűjtése sem
feltétlenül nyilvánvaló; lehetnek változók amiről nincs megfelelő
nemzetközi adatgyűjtés, vagy – mint az előző bekezdés példája is mutatja
– az is előfordulhat, hogy nem is könnyű mérni, számszerűsíteni a
tulajdonságot. Ilyenkor szoktak néha úgynevezett proxy változót
használni, azaz olyat, ami – remélhetőleg szoros – kapcsolatban van a
vizsgálni kívánt változóval, de szemben azzal, mérhető. Egyébként a GDP
nagyon sok változónak lehet a proxy-ja (a probléma inkább pont az, hogy
sok minden keveredik benne). A másik probléma, hogy még ha ismerjük is a
lényeges változókat, baj származhat abból, ha nagyon sok van belőlük (a
minta nagyságához képest). Ezt a kérdéskört fogjuk hamarosan körbejárni.

### A regresszió eszköze

A háromdimenziós ábrával már nagyon közel kerültünk a confounding
problémájának egy lehetséges kezeléséhez. (A „megoldásához“ szó
használata talán túlzás lenne, hiszen megfigyeléses adatból igazán
bombabiztosan soha nem tudunk okozati hatásra következtetni. De az ezzel
kapcsolatos problémákat enyhíthetjük.) Ez lesz az egyenes – és később a
sík – behúzásának igazi értelme: nem a görbeillesztés a lényeg, hanem,
hogy feltételezünk egy modellt, és annak paramétereit becsüljük meg a
begyűjtött tényadatok alapján. Az egyenes és a sík épp egy ilyen modell
megjelenése; ezt a modellt hívjuk lineáris regressziónak. Ebben a
modellben annak a hatása, ha az ezer lakosra jutó nővérek száma eggyel
nagyobb miközben a GDP értéke rögzített, nem függ sem attól, hogy milyen
értéken rögzített a GDP, sem attól, hogy honnan indulva növeljük meg
eggyel a nővérek számát.

Az egész kulcsa a „miközben a GDP értéke rögzített“ kitétel: a
confounding problémája *épp* az volt, hogy a nővérek számának
növelésével a GDP is változik közben, de most mit látunk? Hogy a modell
ezen paramétere azt jelenti, hogy mennyi a hatás *akkor* ha a GDP nem
változik! Ilyen értelemben meg tudtuk azt tenni, hogy bár az adataink
megfigyelésesek voltak, confounding-gal terhelve, mi mégis, *pusztán
matematikai úton* kiszedtük belőle a confounding-tól tisztított értéket!
Úgy szokták szép szóval mondani: kimutattuk a nővérek hatását úgy, hogy
*kontrolláltunk* a GDP-re.

Mindezek eredményét mutatja a következő táblázat, a ‘Becsült hatás’
oszlop adja meg a fenti értelemben vett hatást:

``` r
sjPlot::tab_model(fit, string.pred = "Változó", string.est = "Becsült hatás",
                  string.intercept = "Tengelymetszet", string.ci = "95% CI", digits = 3)
```

<table style="border-collapse:collapse; border:none;">
<tr>
<th style="border-top: double; text-align:center; font-style:normal; font-weight:bold; padding:0.2cm;  text-align:left; ">
 
</th>
<th colspan="3" style="border-top: double; text-align:center; font-style:normal; font-weight:bold; padding:0.2cm; ">
cumexcessperpop
</th>
</tr>
<tr>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  text-align:left; ">
Változó
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
Becsült hatás
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
95% CI
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
p
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
Tengelymetszet
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
5969.405
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
3983.953 – 7954.857
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
<strong>\<0.001</strong>
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
gdp
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.072
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.142 – -0.003
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
<strong>0.042</strong>
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
nurses
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-1.148
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-3.889 – 1.593
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.392
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; padding-top:0.1cm; padding-bottom:0.1cm; border-top:1px solid;">
Observations
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; padding-top:0.1cm; padding-bottom:0.1cm; text-align:left; border-top:1px solid;" colspan="3">
22
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; padding-top:0.1cm; padding-bottom:0.1cm;">
R<sup>2</sup> / R<sup>2</sup> adjusted
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; padding-top:0.1cm; padding-bottom:0.1cm; text-align:left;" colspan="3">
0.426 / 0.366
</td>
</tr>
</table>

Észrevehető, hogy ez a módszer lényegében a rétegzés továbbfejlesztése:
ott is arra törekedtünk, hogy a nővérek számának hatását úgy mutassuk
ki, hogy a GDP nem változik vele együtt, azt állandóan tartjuk, de most
ezt ügyesebben tesszük meg (pl. nem kell kategóriákra osztani a GDP-t,
amik ha túl szélesek, akkor nagyon különböző dolgokat mosnak egybe, ha
túl szűkek, akkor kevés pont jut egy kategóriába, közvetlenül számszerű
válsazt kapunk stb.).

Természetesen annak, hogy a modell által becsült paraméterek tényleg jó
választ adjanak, bizonyos feltételeknek meg kell felelniük. Hát persze:
nem fordulhat elő például, hogy van egy *harmadik* változó, amiről még
mindig megfeledkeztünk! Hiszen honnan tudjuk, hogy csak a nővérek és a
GDP számít? Mi van, ha valamit így is kihagytunk? Ami, ha hat a
halálozásra, megint pont a confounding problémáját hozza be! Itt jutunk
vissza ahhoz a tételmondathoz, amit már az elején is láttunk:
megfigyeléses adatoknál mindig a fejünk felett lebeg, hogy mi van, ha
egy confounding-ot okozó változóról megfeledkezünk. Pontosan ez
tükröződik itt is vissza: ha egy lényeges változót kihagyunk, akkor baj
lesz.

Valójában nem ez az egyetlen feltétel. Mi van, ha a hatás nem lineáris,
például eleinte nagyon számítanak a plusz nővérek, de később már egyre
kevésbé? Mi van, ha a nővérek hatása függ a másik magyarázó változótól,
a gazdasági fejlettségtől, például alacsony fejlettségnél jobban számít
plusz egy nővér, mint magasnál? (Ez utóbbi esetben automatikusan igaz
lesz az is, hogy a gazdasági fejlettség halálozásra gyakorolt hatása is
függ a nővérek számától; ilyenkor szokták azt mondani, hogy
interakcióban van a két változó.) Ezek a kérdések mindazonáltal jól
vizsgálhatóak a regressziós keretrendszerben.

Az ilyen modellek becslésére rendelkezésre állnak jól bevált módszerek.
Ezek milliónyi kérdése közül csak egyet emelnék ki: az így kapott számok
bizonytalanságának ügyét. A probléma az, hogy ezek becsült értékek,
melyekben van attól függő ingadozás, hogy épp milyen adatbázisból
(mintából) becsüljük. Nagyon fontos, hogy most nem arról beszélek, hogy
a mintát bármilyen értelemben is „hibásan“ vettük: a legtökéletesebben
véletlen mintavétel esetén is lesz a becsült értékben ingadozás, pont
úgy, ahogy a kihúzott lottószámok átlaga sem pont 45,5 minden héten.
Pedig az összes számnak (1-től 90-ig) ennyi az átlaga, a mintavétel –
remélhetőleg – itt aztán tökéletesen véletlen, és mégis, a mintának,
tehát a kihúzott 5 számnak az átlaga néha kicsit kisebb mint 45,5, néha
kicsit nagyobb. A dolog kétféleképp is megfogalmazható: ha tudom, hogy a
valódi érték mondjuk 10, akkor a mintából becsült lehet 9 vagy épp 11
is, avagy fordítva: ha a mintában 20-at kaptam, attól még a valódi lehet
19 vagy 21 – hiszen az előbbi azt mondja, hogy a 19 vagy a 21 is
beingadozhat a 20-ba, pusztán a véletlen szeszélye folytán.

Ezt a bizonytalanságot ragadja meg a harmadik oszlopban feltüntetett
úgynevezett konfidenciaintervallum (CI). Ez tartalmazza azokat az
értékeket, amikre igaz, hogy ha az lenne a valódi, akkor könnyen
beingadozhatnának abba, amit ténylegesen kaptunk is: a -0,142 és a
-0,003 közti valódi értékekből könnyen kaphatnánk, pusztán a véletlen
ingadozás miatt, -0,072-t. (A fejlécben feltüntett 95% szabályozza azt,
hogy mit értünk „könnyen“ alatt.) Úgy is szokták mondani, hogy ilyen
valódi értékek esetén a tényleges érték attól való eltérése betudható a
véletlen ingadozásnak, szép szóval: nem *szignifikáns* az eltérés. Ha a
konfidenciaintervallum tartalmazza a nullát (ami ugye azt jelenti, hogy
a kérdéses változónak valójában nincs hatása az eredményre!), az
magyarra lefordítva azt jelenti, hogy nincs okunk feltételezni, hogy a
változónak van hatása: ha nem lenne, akkor is kényelmesen kijöhetett
volna az, ami ki is jött. Ilyenkor mondjuk azt, hogy a változó hatása
nem szignifikáns. A táblázatban vastag betűtípus jelöli a szignifikáns
változókat.

A regresszió kérdésköre ezen túlmenően is egy hatalmas, de érdekes, és
nagyon sok területen – így a biostatisztikában kiemelten – fontos téma.
Most szinte csak utalásszerűen tudtam megemlíteni pár fontos kérdését,
de a részletek
[előadásaimban](https://www.youtube.com/c/FerenciTam%C3%A1s) és
[jegyzeteim között](https://tamas-ferenci.github.io/) elérhetőek (néhány
adott témába vágót a szövegben is belinkelek a megfelelő helyen).

### Több változó modellezése

Látszólag tehát meg is vagyunk: kimutattuk mind a nővérek számának, mind
a GDP-nek a hatását, immár korrekt módon – legalábbis, ha az említett
feltételek teljesülnek, például más változó nem játszik szerepet, ezek
hatása tényleg lineáris. Kezdjük az első megjegyzéssel: ennél a kettőnél
ugyanis jóval több – potenciálisan – a kimenetet befolyásoló változónk
van, és ezt már szépen ábrázolni nem fogjuk tudni. De sebaj, ha
elszakadunk az ábrázolástól, és áttérünk arra az értelmezésre, hogy egy
lineáris kapcsolatot feltételezzük, és annak a paramétereit (amik „adott
paraméter egységnyi növelésének a hatása a többit változatlanul tartva“
értelmük van) szeretnénk megbecsülni, akkor ez nem probléma. Márpedig ez
az eljárás könnyedén kiterjeszthető tetszőleges számú változóra.

Úgyhogy ezt használva bepakoljuk az összes változót egy nagy modellbe,
és abból kiolvassuk az eredményt, azt is, hogy mi az ami befolyásolta a
halálozást (és mennyire), és azt is, hogy mi az, ami nem:

``` r
fit2 <- lm(cumexcessperpop ~ popdensity + overcrowding + urbanization + gdp + popold + obese +
             smoke + alcohol + asthma + chrt_angpec + diab + hblpr + healthexpenditure + nurses,
           data = RawData)

sjPlot::tab_model(fit2)
```

<table style="border-collapse:collapse; border:none;">
<tr>
<th style="border-top: double; text-align:center; font-style:normal; font-weight:bold; padding:0.2cm;  text-align:left; ">
 
</th>
<th colspan="3" style="border-top: double; text-align:center; font-style:normal; font-weight:bold; padding:0.2cm; ">
cumexcessperpop
</th>
</tr>
<tr>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  text-align:left; ">
Predictors
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
Estimates
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
CI
</td>
<td style=" text-align:center; border-bottom:1px solid; font-style:italic; font-weight:normal;  ">
p
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
(Intercept)
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
8593.20
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-5967.44 – 23153.83
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.206
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
popdensity
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.35
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-6.64 – 5.94
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.899
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
overcrowding
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
36.77
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-64.16 – 137.70
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.418
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
urbanization
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-4.91
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-95.22 – 85.40
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.901
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
gdp
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.04
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.14 – 0.07
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.439
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
popold
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-187.95
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-880.95 – 505.04
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.542
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
obese
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-245.32
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-548.34 – 57.69
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.097
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
smoke
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-37.66
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-379.32 – 303.99
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.802
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
alcohol
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
109.46
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-105.57 – 324.48
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.268
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
asthma
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-310.45
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-1666.98 – 1046.09
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.605
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
chrt angpec
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
292.37
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-247.49 – 832.23
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.241
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
diab
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-18.78
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-1179.77 – 1142.21
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.971
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
hblpr
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
123.88
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-284.40 – 532.16
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.496
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
healthexpenditure
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-0.25
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-1.66 – 1.15
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.686
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; ">
nurses
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
1.61
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
-2.03 – 5.26
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:center;  ">
0.330
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; padding-top:0.1cm; padding-bottom:0.1cm; border-top:1px solid;">
Observations
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; padding-top:0.1cm; padding-bottom:0.1cm; text-align:left; border-top:1px solid;" colspan="3">
22
</td>
</tr>
<tr>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; text-align:left; padding-top:0.1cm; padding-bottom:0.1cm;">
R<sup>2</sup> / R<sup>2</sup> adjusted
</td>
<td style=" padding:0.2cm; text-align:left; vertical-align:top; padding-top:0.1cm; padding-bottom:0.1cm; text-align:left;" colspan="3">
0.909 / 0.727
</td>
</tr>
</table>

Akkor most végeztünk? Sajnos a helyzet nem ilyen egyszerű.

#### A multikollinearitás problémája

Az első probléma abból fakad, hogy ezek a magyarázó változók – ahogy azt
a GDP és a nővér-szám példáján láttuk is – egymással is összefüggenek.
Ez probléma? Ha empirikusan szeretnénk meghatározni az egyes változók
szerepét, akkor igen: ahogy arról volt szó, a regresszió azt próbálja
megbecsülni, hogy mi a helyzet akkor, ha az egyik változó értéke
rögzített, és csak a másik változik. Igen ám, de ha a magyarázó változók
összefüggenek egymással, az épp azt jelenti, hogy ha az egyiket
lerögzítjük, az elég jól meghatározza a másikat is, azaz kicsi lesz
abban a szóródás. Márpedig kicsi szóródásból nehéz lesz megbecsülni a
hatást: mikor mondanánk meg szívesebben empirikus alapon, hogy +1 fok
hőmérséklet hogyan hat a gázfogyasztásra, ha ezer darab -10 és +30 fok
közötti napról van információnk, vagy ha ezer darab 20 és 21 fok közötti
napról? Ezt hívjuk a
[multikollinearitás](https://www.youtube.com/playlist?list=PLqdN24UCw5hk7KefBBleJkE6QpPSBgszh)
problémájának. Mint ebből is látható, ez a jelenség egyetlen változóra
vonatkoztatva is ugyanúgy értelmezhető: amiben kicsi a szóródás, annak
nehezebb megbecsülni a hatását. Extrém esetben, ha egy változónak
ugyanaz az értéke az egész mintában, akkor annak a hatását nem tudjuk
megbecsülni – hiszen egyáltalán nem lesz benne szóródás. (Például ezen
adatbázis alapján mondjuk meg, hogy az északi féltekén történő
elhelyezkedés hogyan hat a járvány terhére – érthető, hogy ezt nem
fogjuk tudni megmondani!) De nem kell ilyen erőltetett példát hozni: ha
mindenki pontosan ugyanúgy hozott egy intézkedést, akkor ennek hatása
empirikusan nem vizsgálható. A regresszió tehát mindig csak valamilyen
szóródásból tud becsülni, ezt sokszor fontos végiggondolni, hogy milyen
szóródás áll rendelkezésre egy adott paraméter becsléséhez.

Térjünk vissza a két, összefüggő változó kérdésére. Hangsúlyozom, hogy
ilyen esetben a két változó hatása *együtt* továbbra is jól
megbecsülhető, csak *külön-külön* nem, magyarán: nehéz *elkülöníteni* a
hatásukat. De ez talán intuitíve is érezhető: nehéz megmondani, hogy
*külön* mi a hatása a demenciának *és* a 60 év feletti életkornak,
hiszen kevés alanyunk lesz akinek 60 év alatt demenciája van, így amikor
a nem demens helyett demens alanyokat nézünk, akkor *szinte*
automatikusan 60 év felettiek is lesznek.

Ez nem egy „kijavítható“ probléma abban az értelemben, hogy nem az
általunk megalkotott modell, hanem a felhasznált adatok jellemzője – az
meg olyan, amilyen, az nem egy általunk befolyásolható kérdés, hogy a
GDP és a nővérek száma összefügg.

Minél több egymással összefüggő változót rakunk bele a modellbe, annál
jobban fogja az egyes változókat a többi magyarázni, így annál rosszabb
lesz ilyen szempontból a helyzet. Ami biztosan segít, az a nagyobb
mintanagyság: ettől ugyan továbbra is nehezebben lesznek
szétválaszthatóak a hatások, azaz bizonytalanabbak lesznek a becslések
ahhoz képest, mintha a változók nem függenének össze, de a nagyobb
mintanagyság ezt ellensúlyozza, azáltal, hogy *általában* csökkenti a
becslések bizonytalanságát.

Így máris jobban érthető, hogy miért lett inszignifikáns az összes
változónk!

Valójában azonban ennél rosszabb a helyzet. Ha valami véletlen folytán
lett volna szignifikáns változó, akkor sem biztos, hogy túlságosan
hihető lenne az eredmény a jelen esetben. Ennek okát fogjuk megnézni a
következő pontban.

#### A túlilleszkedés problémája

A másik gond, ami akkor jelentkezik, ha a mintamérethez képest túl sok a
változónk, a túlilleszkedés. Amikor mi egy regressziós modellt
megbecslünk, azt mindig egy minta alapján végezzük, és az a célunk, hogy
a mintát a lehető legpontosabban leírjuk. (Ha megnéztük volna a becslés
konkrét módszerét, akkor [láttuk
volna](https://www.youtube.com/playlist?list=PLqdN24UCw5hmIG2eOsaH9tpleuppR_ssG),
hogy ez szó szerint is igaz: a legnépszerűbb becslési eljárás *épp* azt
adja vissza becsült értékként, ami mellett a modellünk a legjobban
leírja a mintát). Igen ám, de közben persze valójában nem magát a mintát
akarjuk jól leírni (ha ennyi lenne a célunk, akkor nincs is szükség
regresszióra, ott a minta, az teljesen pontosan leírja a mintát, és
kész), hanem következtetni a minta alapján a háttérben lévő valóságra
(statisztikus nyelven úgy szokták mondani: a sokaságra). Ehhez
természetesen fel kell használnunk a mintabeli információt, és ha olyan
modellt alkalmazunk, ami nem tud elég információt felhasználni –
nevezzük ezt alulilleszkedésnek – akkor természetesen nem várható, hogy
a sokaságról helyesen tudunk nyilatkozni. Ez eddig elég logikus, de itt
jön a csavar, mert az előbbiből úgy tűnhet, hogy minél több információt
felhasználni képes, azaz minél komplexebb modellt vetünk be, annál jobb
lesz a helyzet. Csakhogy meglepő módon ennek egy ponton túl épp az
ellenkezője lesz az igaz: egyre komplexebb modelleket használva nem
egyszerűen nem javul a sokaság leírása, hanem elkezd kifejezett romlani!
Ezt hívjuk túlilleszkedésnek.

A probléma úgy fogalmazható meg, hogy a túl komplex modell egy ponton
túl már az adatbázisban lévő véletlen zajokat is képes lesz leírni,
márpedig ha képes lesz rá, akkor meg is fogja tenni, hiszen a becslési
módszernek ugyebár épp az a célja, hogy a mintát minél jobban leírja –
azt pedig a véletlen zajok leírása is javítja. Csakhogy a sokaság
leírását ez nem hogy nem javítja, de kimondottan lerontja, hiszen abban
nem lesznek benne ezek a véletlen zajok.

Ezt szemléletesen mutatja az alábbi animáció, ahol egy magyarázó
változónk van, a piros görbe mutatja a valódi összefüggését az
eredményváltozóval, ebből generáltuk véletlenszerűen a fekete pontokat,
majd azokra egyre komplexebb és komplexebb regressziós modelleket
illesztünk; ezeket a kék görbék mutatják:

``` r
set.seed(1)
SimData <- data.frame(x = runif(20))
SimData$y <- 2*SimData$x^3 + rnorm(20, 0, 0.2)
for(p in 0:18)
  print(ggplot(SimData, aes(x = x, y = y)) + geom_point() +
          geom_function(fun = ~ 2*(.x)^3, color = "red") + 
          geom_smooth(method = "lm", formula = if(p==0) y ~ 1 else y ~ poly(x, p), se = FALSE, n = 500) +
          labs(title = if(p<=1) paste0("Alulilleszkedés (p = ", p, ")") else
            if(p<=6) paste0("Nagyjából jó illeszkedés (p = ", p, ")") else
              paste0("Túlilleszkedés (p = ", p, ")")) + coord_cartesian(ylim = c(-0.5, 1.5)))
```

![](README_files/figure-gfm/unnamed-chunk-12-.gif)<!-- -->

(Érdemes megnézni, hogy több modellre is a „nagyjából jó“ kifejezést
használtam: bár a sokaság ismeretében meg lehetne mondani, hogy közülük
konkrétan melyik a jó, de az ilyen kis mintanagyság nem teszi lehetővé,
hogy ezeket a minta alapján elkülönítsük.)

Azt hiszem a fenti illusztráció nem sok kommentárt igényel a
tekintetben, hogy mit jelent a túlilleszkedés, az, hogy a túl komplex
modell már a zajokat is megragadja, így bár a mintát egyre jobban
leírja, a sokaságot meg egyre kevésbé.

Bár a fenti animáció nem a magyarázó változók számának változtatásával
oldotta meg a modell komplexitásának változtatását (hiszen az fixen 1
volt), de a helyzet az, hogy a több magyarázó változó is pontosan
ugyanezt jelenti! A több magyarázó változó ugyanis több megbecsülendő
paramétert jelent (ahogy a fenti táblázat is mutatja, mindegyiknek van
egy saját hatása), a több szabad paraméter pedig komplexebb modellt
jelent. Ha túl sok magyarázó változót pakolunk bele egy regressziós
modellbe, akkor azt fogjuk *hinni*, hogy gyönyörű szép az illeszkedése
(és ezt fogják a különböző számszerű jellemzők is, látszólag teljesen
objektíven, mutatni), de valójában az történik, amit a fenti animáción
látunk.

A történet tanulsága tehát, hogy az értelmesen megbecsülhető paraméterek
száma limitált attól függően, hogy mennyi adatunk van: van egy –
mintanagyságtól függő – felső korlátja a modell komplexitásának, aminél
még remélhetőleg nem lesz túlilleszkedett az eredmény. Ez azt is
jelenti, hogy a modellezhető változók száma is limitált, függően a
mintanagyságtól!

### A változószelekció kérdésköre

Egészében véve mindkét fenti problémakör végén hasonló konklúzióra
jutottunk: jó lenne vagy a mintanagyságot növelni, vagy a változók
számát csökkenteni. Fókuszáljunk most ez utóbbira! A túlilleszkedéssel
kapcsolatos irodalom a mintanagyság és a modellezhető változók számának
összefüggéséről [nagyon sok
eredményre](https://onlinelibrary.wiley.com/doi/10.1002/sim.7993)
jutott, egészen számszerű formában; egy gyakori mondás például, hogy
olyan regresszióknál, mint amit most mi is használunk, legyen a
felhasznált változók száma legfeljebb a mintaméret osztva 15-tel. Avagy,
fordítva megfogalmazva, legyen legalább 15-ször annyi megfigyelésünk a
mintában, mint ahány változót a modellbe akarunk rakni! A pontos szám
sok mindentől függ, a multikollinearitás fokától, attól, hogy a
valóságban mennyire szoros a kapcsolat a kimenet és a magyarázó változók
között, a magyarázó változók eloszlásától, így a helyzet akár ennél
rosszabb is lehet, de nagyjábóli irányszámnak most tökéletesen megteszi
ez a 15.

A fenti szabály azért fontos, mert azonnal ordítóvá teszi, hogy milyen
drámai helyzetben vagyunk. Nekünk a legjobb esetben is 25-30 európai
országunk van, és mivel ezzel nem tudunk mit kezdeni, így ez lényegében
azt jelenti, hogy 2 változót tudunk mindössze vizsgálni!

Ez egy egészen drasztikus probléma – emlékezzünk vissza a felrajzolt
diagramra a megvizsgálandó tényezőkről! (És persze még az sem volt
teljes, milliónyi további ötletünk lehet!) Hogy fogunk így egyáltalán
*bármit* mondani?! Azonnal elkezd járni az ember agya azon, hogy mit
tehetünk a megoldás érdekében. Az első ötlet nagyon kézenfekvő: valahogy
válogassuk ki a változók egy részét, és csak azokat rakjuk be a
modellbe. Ez nagyon csábító lehetőség, hiszen így csökkentjük a köztük
lévő, lehetséges összefüggéseket, így javítjuk a multikollinearitást, és
egyidejűleg a túlilleszkedés ellen is védekezünk. Ez nem egyszerűen
„csábító“, de egy ilyen helyzetben szinte megkerülhetetlennek is tűnik:
valahogy be kell a mintanagyság osztva 15-tel küszöb alá pofozni a
magyarázó változók számát.

A gond az, hogy ez az egész terület egy hatalmas aknamező, ahol nagyon
könnyű hibás megoldást választani (és sok közülük sajnos még a
szakirodalomban is újra meg újra felbukkan).

A tételmondat nagyon egyszerű: csak olyan módszert használhatunk a
változók kiválogatására, ami nem használja fel a kimenet értékeit.

Tehát néhány jó módszer:

-   Pusztán a magyarázó változók struktúráját, azaz egymás közti
    kapcsolataikat vizsgálva elhagyni olyanokat, amik redundánsak (azaz
    a bennük lévő információk más magyarázó változókban is jórészt
    megvannak).
-   Pusztán a magyarázó változók struktúráját, azaz egymás közti
    kapcsolataikat vizsgálva új magyarázó változókat képezni
    összevonással (erre vannak statisztikai módszerek).
-   Nem statisztikai, hanem szakmai alapon képezve összevonásokat. Egy
    tipikus példa, hogy az „alany cukorbeteg“, az „alanynak magas
    vérnyomása van“, az „alanynak perifériás érbetegsége van“ változók
    helyett berakunk egy darab az „alanynak krónikus betegsége van“
    változót. Igen, jobb lenne megmondani, hogy *külön-külön* mi a
    hatása a cukorbetegségnek, a magas vérnyomásnak és a perifériás
    érbetegségnek, de ha egyszerűen nincs elég nagy mintánk, akkor el
    kell fogadni, hogy erre nem leszünk képesek.

A végére hagytam a legjobb jó módszert: szakmai alapon, tárgyterületi
ismereteket használva megpróbálni szűrni a felhasznált változók körét.
Igen, ez nem empirikus (miközben pont ez lenne a célunk), de néha nem
tudunk jobbat tenni. (A „néha nem tudunk jobbat tenni“ gondolatra még
visszatérünk.)

Nézzünk most néhány rossz módszert:

-   Megnézni, hogy melyik függ össze önmagában az eredményváltozóval, és
    csak azokat belerakni a többváltozós modellbe. Ez a módszer
    [teljesen
    hibás](https://www.jclinepi.com/article/0895-4356(96)00025-X/pdf).
    Az még csak hagyján, hogy az előzetes szűrés is egy statisztikai
    teszttel történik, ami nem tökéletes (a valóságban az
    eredményváltozóval nem összefüggőre is mondhatja, hogy összefüggő,
    vagy, ami a mi mostani szempontunkból még nagyobb probléma, pont
    fordítva), de az igazi gond, hogy nem veszi figyelembe a
    többváltozós struktúrát: mi van, ha egy változó csak az *után* válik
    lényegessé, ha más változók már bent vannak a modellben?!
-   Megcsinálni a többváltozós modellt, majd elhagyni az inszignifikáns
    változókat. Ez a módszer [szintén
    hibás](https://www.tandfonline.com/doi/abs/10.1080/00031305.1983.10482729).
    A helyzet ugyanaz pepitában: egyrészt az, hogy „inszignifikáns“, nem
    ugyanaz, mint hogy biztosan 0 a hatása: az inszignifikanciát is egy
    statisztikai teszttel ítéljük meg. Ha ez téved, márpedig ez
    előfordulhat, és lényeges változót hagyunk el, akkor épp a kihagyott
    változó okozta torzítást fogjuk előhozni! Épp emiatt a dolog
    ráadásul filozófiailag is érthetetlen, hiszen attól még, mert egy
    változó inszignifikáns, nagyon is segíthet a többi paraméterét
    helyes értékre beállítani.
-   Pláne
    [horrorisztikusak](https://journalofbigdata.springeropen.com/articles/10.1186/s40537-018-0143-6)
    azok a módszerek, amelyek oda-vissza veszik be és dobálják ki a
    változókat, keresve a valamilyen mutató szerinti legjobbat
    („stepwise regresszió“). Ez lényegében felturbózza az előbbi
    módszerek hibáit: szinte garantáltan túlilleszkedett modellre vezet,
    aminek praktikusan minden létező paramétere [torzított/hibás
    lesz](https://stats.stackexchange.com/a/20856).
-   Amire kevesebben gondolnak, pedig ugyanaz a helyzet, amikor a kutató
    az előbbit „kézzel“ hozza létre: össze-vissza keresgél, kidobva és
    bevonva változókat, próbálkozva különböző modellekkel, hogy mi a
    legjobb.

Ha valaki nem hiszi el a fentieket nekem (nagyon jól teszi!), akkor
statisztikai programnyelven maga is leszimulálhatja, és saját kezűleg
kipróbálhatja; ilyen módon, tehát szimulációval a többség könnyen
leellenőrizhető.

Érdemes kiemelni és mélyebben végiggondolni azt a megjegyzést, hogy az
utóbbi módszerek túlilleszkedéshez vezetnek. Ez egyfelől végülis nem
olyan meglepő: e módszerek mind a konkrét adatbázishoz „csiszolják“ az
eredményt, innen nézve érthető, hogy ahhoz vezethetnek, hogy a modell
túl jól fog illeszkedni ahhoz. De másrészt mégis csak valami nagyon
paradox helyzetre jutottunk, hiszen miért is kezdtünk egyáltalán bele
ebben az egész változó válogatás dologba? Azért, mert hallottunk róla,
hogy a túl sok változó túlilleszkedéshez vezethet, és tenni akartunk ez
ellen valamit. Magyarán: nekiálltunk lépni a túlilleszkedés ellen, majd
kiderül, hogy amit teszünk, az pont a túlilleszkedést rontja!

Ez egy nagyon nagy csapdája és nehézsége ennek az egész témakörnek: azt
szoktuk mondani, hogy a regressziós modellépítés egy „iteratív folyamat“
(azaz a modellt ellenőrizni kell, ha nem jó, akkor visszamenni,
módosítani, újra ellenőrizni, és így tovább), ami persze igaz is, csak
közben a *túl sok* iteráció ugyanúgy hiba forrása lehet! Ebben igazi
feladat megtalálni az egyensúlyt.

Még egy kommentárt fűznék a fentiekhez. Gyakran hallani hivatkozást
arra, hogy a modelleknek „egyszerűeknek“, „takarékosnak“ kell lenniük
(néha erre mondják azt, hogy a parszimónia elve). Ami persze igaz is, ha
a túlilleszkedés szempontjára gondolunk. De he ezzel indokolják az
inszignifikáns változók elhagyását, vagy a stepwise módszerek
alkalmazását, az a parszimónia elvének totális félreértéséről
tanúskodik: a parszimónia nem egyszerűen az, hogy hány darab változó van
benne a végső modellben! A takarékosság fogalmába ugyanúgy beletartozik
az is, hogy hogyan jutottunk el ahhoz a modellhez. Ha a végső modellben
csak három magyarázó változó van, de háromszáz lépésen keresztül
barkácsoltuk, mire kijött, az a legkevésbé sem „takarékos“ – csak ez nem
látszik a végeredményből! A probléma *pont* az, hogy a közbenső
barkácsoló lépések mind-mind a modell (valódi) komplexitását növelik,
csak épp ezzel sehol nem számolunk el, ha a végső modellt úgy
prezentáljuk, mintha élből azt becsültük volna meg. Azaz a parszimónia
elve rendben van, csak épp annak az állításnak, hogy e módszerek ezt
segítik elő, épp az ellenkezője az igaz: ezek megsértik ezt az elvet,
csak ezt *eldugják* az útban, amíg eljutunk a végső modellig, ami persze
még annál is rosszabb, mintha legalább látnánk, hogy mi a valódi
helyzet.

A fentiek abba az irányba mutatnak, hogy lehetőleg egyetlen modellt
találjunk ki, előre, azt becsüljük meg az adatokon, és bármi is jön ki,
ne módosítsuk. (Különben túl fogunk illeszkedni.) Ahogy az iterációra
vonatkozó megjegyzésemben is utaltam rá, ez azért túl radikális
álláspont: ugyanúgy ahogy egy *kicsit* a modell komplexitását is
növelhetjük túlilleszkedés nélkül, mondjuk néhány változó hozzáadásával,
*kicsit* azért pofozgathatjuk is. (Amint láttuk, ez a kettő igazából
ugyanaz: mindkettő a modell valódi komplexitását növeli.) Pár
próbálkozást tehát tehetünk változó kihagyására vagy hozzávételére,
összehasonlíthatjuk az eredeti modellünkkel ezeket, és kiválaszthatjuk,
hogy melyik a legjobb. Ami fontos, hogy *néhány* próbálkozást tegyünk,
ne rengeteget, és hogy ezek *prespecifikáltak* legyenek! (Tehát még az
adatokkal való bármilyen munka előtt, előre döntsük el, szakmai
megfontolások, tárgyterületi ismeretek alapján hogy melyik lesz az a
néhány modellünk, amik közül adat-alapon majd választunk.) A
túlilleszkedés szempontjából ugyanis az a legrosszabb, ha adatok által
sugallt felvetéseket vizsgálunk meg.

### A kényelmetlen tudomány

A fenti okfejtés összességében véve egy nagyon nyugtalanító képet
sugall: úgy tűnik, hogy ha kevés adatunk van, akkor egyszerűen nem
tudunk mit tenni. Nem akarok zsákbamacskát árulni, ez valamilyen
értelemben tényleg így van. Olyannyira, hogy a helyzetet a neves
statisztikus John Wilder Tukey találóan úgy hívta: ez az „uncomfortable
science“, a kényelmetlen tudomány.

A talán leghíresebb példa erre a Titius–Bode-szabály. Ez azt állítja,
hogy a Naprendszerben a sorrendben *n*-edik bolygó távolsága a naptól
0,4 + 0,3 · 2<sup>*n*</sup> (egy csillagászati egységnek nevezett
mértékegységben mérve). Ezt a 18. században vetették fel, és az akkor
ismert bolygókra prímán működött. De itt vajon tényleg valamilyen
matematikai összefüggés van, azaz valamilyen csillagászati okot kell
keresni amögött, hogy ez így alakult? Vagy egyszerűen csak véletlen
egybeesésről van szó? (Lehet szó túlilleszkedésről? Hogyne, simán,
elvégre ki tudja, hogy Titius és Bode vajon hány formulát próbált ki,
mire ez működött…!) De akkor mit tegyünk, hogyan ellenőrizzük le? És itt
jön a kényelmetlen tudomány: aligha tudunk venni még egy bolygót
mintának, hogy kipróbáljuk azon is működik-e a szabály…!

De mennyire „kényelmetlen tudomány“ helyzet a mi mostani kérdésünk?

Egyrészt megpróbálhatjuk növelni a mintanagyságot. Lejjebb tudunk menni
megyei szintre? Esetleg járásira? Ez csábító lehetőség, de két nehézség
lesz. Az egyik az adatokhoz kapcsolódik: van adatunk arra, hogy *megyei*
szinten hány nővér jut egy betegre? Egyáltalán, értelmezhető ez a mutató
megyei szinten? (Pláne járásin!) A másik gond, hogy sok változó van,
amiben az országon *belüli* adatokban nem lesz nagy szóródás (például a
bevezetett intézkedések akár teljesen egységesek is lehetnek), ami
nehezíti a becslésüket, ahogy a multikollinearitásnál láttuk is.

Kísérletezhetünk azzal is, hogy idődimenziót is adunk a vizsgálatnak,
tehát nem egyben vizsgáljuk az egész járványt, hanem időszakonként. Ez
egyébként önmagában, a mostani problémától teljesen függetlenül is egy
fontos felvetés. Hiszen egészen idáig „összeöntöttük“ a járvány adatait,
és bár valóban van sok minden, ami teljesen állandó, vagy lényegében
állandó (mondjuk az ország korfája), sok minden nem: oltást bevezettek,
időben felfutott az oltottak aránya, intézkedéseket meghoztak, vagy épp
kivezettek stb. Szép szóval élve a *dinamika* is fontos lehet, így egy
finomabb vizsgálat – sajnos azonban, legyünk őszinték, komoly
módszertani kihívások és adatszerzésre vonatkozó nehézségek árán –
megpróbálkozhat ezt is figyelembe venni.

Tehetünk okosan a változók számának csökkentése érdekében is. Már az
ottani pont végén is említettem ennek egy lehetőségét, a néhány,
prespecifikált modell összehasonlítását. A korszerű statisztika további
eszközökkel is szolgál: vannak módszerek a túlilleszkedés fokának
megbecslésére, hogy lássuk, bajban vagyunk-e (validáció, például
bootstrap), vannak módszerek amelyek úgy becsülnek regressziót, hogy
igyekeznek tenni a túlilleszkedés ellen (regularizáció, vagy más szóval
penalizáció), vannak más még jobban eltérő elven felépülő becslések (pl.
a LASSO), sőt, elárulom, hogy ha ésszel csináljuk, akkor akár még a
stepwise szelekciós módszereknek is lehet szerepük (nagy mintán,
megfelelő paraméterekkel, elszámolva az előzetes szelekció tényével).

## Záró gondolatok

Talán ezek az utolsó gondolatok érzékeltették legjobban, hogy írásom
célja nem egy „lezárt válasz“ közvetítése volt. Sőt, egyáltalán
semmilyen választ nem adtam a kérdésre, és szándékosan: én most a
módszertanra szerettem volna fókuszálni, ezen belül is különösen arra,
hogy felhívjam a figyelmet a veszélyes (mert csábító) csapdákra.

A területtel foglalkozó kutatók nem lesznek egyszerű helyzetben
hazánkban. Ezt sajnos nem csak statisztikai okokból mondom: a kérdéskör
átpolitizáltsága véleményem szerint rendkívül romboló a valódi
tudományos kutatásokra nézve. Félreértés ne essék, a „politika“ szót nem
egy szükségképp negatív töltetű értelemben használom, sőt, ez pont egy
olyan téma, ahol fontos és hasznos is a politikával való kölcsönhatás,
hiszen az ilyen vizsgálatokból levonhatóak olyan következtetések,
amelyek az (egészség)politikát is vezethetik a magyar ellátórendszer, a
prevenciós rendszer, a népegészségügyi programok javításának irányában.
A gond ott kezdődik, amikor megjelenik a prekoncepciózus szemlélet,
amikor minden intézkedésnek vagy teljesen, alapjában és menthetetlenül
rossznak, vagy teljesen, tökéletesen és aggálytalanul jónak *kell*
lennie. (Pláne, ha vannak olyan szereplők, akik rá is tudják ezt
kényszeríteni másokra, például mert elhallgattathatnak nekik nem tetsző
véleményeket…) A probléma az, hogy az ilyen kutatások sajnos ennek
nagyon kitettek, hiszen nehéz elkerülni, hogy a magyarázó változókat az
ember összekösse a kormány tevékenységével: mi az, amire nincs érdemi
ráhatása a releváns időhorizonton (pl. a korfa), mi az, amire van, de
azért nem túl direkt és azonnali módon (pl. elhízottak aránya), és mi
az, amire direkt és azonnali módon van (pl. tesztelési stratégia).
Minden oldali szereplőnek meg kellene értenie, hogy az ország érdekét
csak az szolgálja, ha e kérdéseket olyan légkörben lehet megbeszélni,
ami nem a pillanatnyi politikai haszon kinyerésének lehetőségét nézi az
eredményekből.

A fentiekből minden bizonnyal kiderült, hogy miért gondolom, hogy nehéz
ezt a lantot kézbe venni. Ezzel azonban senkit nem elriasztani
szeretnék, épp ellenkezőleg, remélem azt is meg tudtam mutatni, hogy a
nehézségei egyúttal a terület szépségét is jelentik, valamint, hogy ha
valaki kellő óvatossággal, alapossággal és persze elszántsággal vág
bele, akkor az egész ország számára értékes eredményekre lehet jutni
ebben a témában. Remélem írásom, ha csak gondolatébresztés erejéig is,
de segítséget jelent ebben.

------------------------------------------------------------------------

(Az írás a 2022. március 20-án érvényes magyar állapotokat tükrözi.)

A [szerző](http://www.medstat.hu/) klinikai biostatisztikus,
orvosbiológiai mérnök. A fent leírtak teljes egészében a magánvéleményét
képviselik.
