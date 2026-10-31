# Eesti uudiste algallikad ja RSS-kanalid

Valik 42 Eesti asutuse, spordiliidu, omavalitsuse ja kultuuriorganisatsiooni enda avalikke uudistekanaleid: **40 RSS-kanalit ja kaks uudiste veebilehte**. Sobib oma RSS-lugeja täiendamiseks ning organisatsiooni algse teate leidmiseks. Loend ei ole täielik ülevaade Eesti uudisallikatest.

Koostanud [Uudised.ai](https://uudised.ai/). [Otsitav veebiloend ja allikate kontrolliküsimused](https://uudised.ai/allikad) · [Avalik OPML eksport](https://uudised.ai/allikad.opml). Uudised.ai on automaatselt AI abil avaldav uudisväljaanne, kus puudub inimtoimetaja. Siinsed 42 allikakirjet kirjeldavad lingitud organisatsioonide enda kanaleid; Uudised.ai on kogumiku koostaja.

## Failid

| Fail | Sisu |
| --- | --- |
| [feeds.opml](feeds.opml) | 40 RSS-kanalit, rühmitatud seitsme teema kaupa; imporditav uudislugejasse. |
| [sources.json](sources.json) | Kõik 42 allikat: nimi, avalik tunnus, teema, keel, veebiaadress, võimalik RSS-aadress, viidete ülevaatamise kuupäev, lühiselgitus ja kontrolliküsimus. |
| [validation.json](validation.json) | Vormingu, avaliku lehega kattuvuse ja kuupäevastatud tehnilise kontrolli tulemused. |

## Kuidas kanalid oma uudislugejasse lisada?

1. Ava [feeds.opml](feeds.opml) ja laadi faili **Raw**-versioon alla. Salvesta XML-fail, mitte GitHubi veebileht.
2. Vali oma RSS-lugejas kanalite või OPML-faili importimine ning ava allalaaditud fail.
3. Jäta alles endale vajalikud teemad ja allikad. OPML sisaldab kanalite aadresse, mitte artiklite koopiaid.
4. Kui soovid lisada ainult ühe kanali, kopeeri selle RSS-aadress allolevast tabelist või JSON-faili väljast `feedURL`.

Politsei- ja Piirivalveameti ning Päästeameti kirjed viitavad uudiste veebilehele. Nende jaoks pole selles loendis RSS-aadressi märgitud ning need ei kuulu OPML-faili. See ei kinnita, et avaldajal ei võiks olla mõni muu RSS-kanal.

## Mida ja millal kontrolliti?

Kõik 42 kirjet ja 40 RSS-aadressi vastasid ekspordi ajal avalikule [allikaloendile](https://uudised.ai/allikad) ning [OPML-failile](https://uudised.ai/allikad.opml). Failide sisu koostati 1. novembril 2026 Eesti aja järgi.

40 RSS-kanalit läbisid tehnilise vormingu- ja loetavuskontrolli **31. oktoobril 2026**. Selle ekspordi jaoks ei küsitud kõiki kanaleid uuesti. Kontrolli aja, kirjekoguse ja uusima leitud avaldamiskuupäeva leiab failist `validation.json`. JSON-kirje `reviewedAt` tähistab viidete ülevaatamise kuupäeva.

Kuupäevastatud kontroll ei taga kanali praegust kättesaadavust, uut postitust iga päev ega iga teate õigsust. Uuenduste kiirus sõltub avaldajast ja sinu uudislugejast. Kanalit kasutades järgi avaldaja tingimusi ning HTTP vahemälu- ja veateateid; väldi põhjendamatult sagedasi korduspäringuid.

## Kuidas algallikat lugeda?

- Erista organisatsiooni enda teadet sõltumatust hinnangust. Amet, spordiklubi, erialaliit või artisti esindaja võib kirjeldada sündmust enda vaatenurgast.
- Vaata sündmuse aega, piirkonda ja inimesi, keda teade puudutab. Lehe muutmise kuupäev ei pruugi olla sündmuse kuupäev.
- Erista ettepanekut otsusest, nominatsiooni võidust, mängu vahetulemust lõppskoorist ja kavandatud sündmust toimunust.
- Võimaluse korral ava teates viidatud otsus, uuring, tulemustabel või muu algdokument. Iga allika juures on üks konkreetne kontrolliküsimus.

## Allikad teemade kaupa

### Riik ja turvalisus

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Riigikontroll](https://www.riigikontroll.ee/) | [RSS](https://www.riigikontroll.ee/rss-feeds/rss.xml) | Vaata auditi uurimisperioodi ning erista kontrollitud leid, soovitus ja asutuse vastus. |
| [Vabariigi President](https://president.ee/) | [RSS](https://president.ee/rss-feeds/rss.xml) | Erista kõneleja seisukohta, kohtumise toimumist ja tegelikult sõlmitud kokkulepet. |
| [Kriis.ee](https://www.kriis.ee/) | [RSS](https://www.kriis.ee/rss-feeds/rss.xml) | Kontrolli juhise kehtivat piirkonda ja ajavahemikku ning seda, kas ilmunud on uuem teade. |
| [Politsei- ja Piirivalveamet](https://www.politsei.ee/et/uudised) | Veebileht | Tee vahet kahtlustusel, menetlusel ja jõustunud kohtuotsusel; esialgne info võib täpsustuda. |
| [Päästeamet](https://www.rescue.ee/et/uudised) | Veebileht | Vaata sündmuse asukohta, tegelikku toimumisaega ja viimast täpsustust, mitte ainult lehe uuendamisaega. |

### Raha ja töö

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Finantsinspektsioon](https://www.fi.ee/et) | [RSS](https://www.fi.ee/et/uudised/rss) | Võrdle täpset ettevõttenime ja tegevusloa ulatust; hoiatus ei kirjelda kõiki samanimelisi teenuseid. |
| [Riigi Tugiteenuste Keskus](https://www.rtk.ee/) | [RSS](https://www.rtk.ee/rss-feeds/rss.xml) | Erista vooru avanemist taotluse rahuldamisest ning kontrolli toetuse saaja tingimusi ja tähtaega. |
| [Tööinspektsioon](https://www.ti.ee/) | [RSS](https://www.ti.ee/rss-feeds/rss.xml) | Kontrolli, kas kirjeldatakse kehtivat nõuet, tulevast muudatust või soovituslikku juhist. |
| [Eesti Toiduainetööstuse Liit](https://toiduliit.ee/) | [RSS](https://toiduliit.ee/feed/) | Liit esindab oma liikmeid: otsi turgu või hindu puudutava väite juurest andmeallikat ja ajavahemikku. |

### Tervis ja haridus

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Tervisekassa](https://tervisekassa.ee/uudised) | [RSS](https://tervisekassa.ee/rss.xml) | Kontrolli, kellele muudatus laieneb ja mis kuupäevast see kehtib; üldteade ei kirjelda iga inimese juhtumit. |
| [Sotsiaalkindlustusamet](https://www.sotsiaalkindlustusamet.ee/) | [RSS](https://www.sotsiaalkindlustusamet.ee/rss-feeds/rss.xml) | Vaata toetuse tingimusi, taotlemise vajadust ja jõustumisaega; väljakuulutatud muudatus ei pruugi veel kehtida. |
| [Põhja-Eesti Regionaalhaigla](https://www.regionaalhaigla.ee/) | [RSS](https://www.regionaalhaigla.ee/rss-feeds/rss.xml) | Erista ühe haigla teenusemuudatust üleriigilisest korraldusest; uuringu tulemusel otsi uuringu enda viidet. |
| [Valga Haigla](https://valgahaigla.ee/) | [RSS](https://valgahaigla.ee/feed/) | Kontrolli teenuse täpset asukohta, vastuvõtu kuupäeva ja seda, kas teade puudutab ajutist või püsivat muutust. |
| [Tartu Tervishoiu Kõrgkool](https://www.tartuh.ee/) | [RSS](https://www.tartuh.ee/feed/) | Õppevõimaluse juures vaata õppekava, vastuvõtutingimusi ja tähtaega; projektiteade ei ole veel uuringutulemus. |

### Keskkond

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Maa- ja Ruumiamet](https://maaruum.ee/) | [RSS](https://maaruum.ee/rss-feeds/rss.xml) | Vaata kaardi või andmestiku seisukuupäeva ja piirkonda; andmete avaldamispäev ei pruugi olla mõõtmispäev. |
| [Eesti Roheline Liikumine](https://roheline.ee/) | [RSS](https://roheline.ee/feed/) | Erista ühenduse ettepanekut vastu võetud otsusest ning kontrolli arvnäitajate algset uuringut või andmestikku. |

### Linnad ja vallad

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Pärnu linn](https://parnu.ee/) | [RSS](https://parnu.ee/rss-feeds/rss.xml) | Vaata, kas teade puudutab Pärnu linna, mõnd osavalda või kogu maakonda ning millal muudatus rakendub. |
| [Rakvere linn](https://www.rakvere.ee/) | [RSS](https://www.rakvere.ee/rss-feeds/rss.xml) | Ära aja Rakvere linna segi Rakvere vallaga; vaata otsuse tegijat ja täpset tegevuspiirkonda. |
| [Haapsalu linn](https://haapsalu.ee/) | [RSS](https://haapsalu.ee/feed/) | Erista avalikku arutelu või eelnõu lõplikust otsusest ning kontrolli otsuse rakendumiskuupäeva. |
| [Valga vald](https://valga.ee/) | [RSS](https://valga.ee/feed/) | Kontrolli, millist valla asulat ja teenust teade puudutab; Valga vald ja Läti Valka on eri omavalitsused. |
| [Võru linn](https://www.voru.ee/) | [RSS](https://www.voru.ee/rss-feeds/rss.xml) | Erista Võru linna, Võru valda ja maakonda ning kontrolli näiteks toetuse puhul elukoha tingimust. |
| [Paide linn](https://paide.ee/) | [RSS](https://paide.ee/feed/) | Vaata, kas tegemist on otsuse, ettepaneku või taotluskutsega; tähtaja juures kontrolli ka aastat. |
| [Rae vald](https://www.rae.ee/) | [RSS](https://www.rae.ee/rss-feeds/rss.xml) | Kontrolli asulat ja aadressi; planeeringu algatamine ei tähenda ehituse alustamist või valmimist. |
| [Viimsi vald](https://viimsi.ee/) | [RSS](https://viimsi.ee/rss-feeds/rss.xml) | Vaata, millal ja kellele teenusemuudatus kehtib; ajutine liiklus- või teenusepiirang vajab täpset lõppaega. |
| [Räpina vald](https://www.rapina.ee/) | [RSS](https://www.rapina.ee/feed/) | Erista valminud tööd kavandatavast teenusest ning otsi toetuse tingimuste juurest valla enda otsust. |
| [Saue vald](https://www.sauevald.ee/) | [RSS](https://www.sauevald.ee/rss-feeds/rss.xml) | Kontrolli, kas teade käib Saue linna või mõne teise valla asula kohta ning kes saab teenust kasutada. |

### Sport

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Eesti Sõudeliit](https://www.soudeliit.ee/) | [RSS](https://www.soudeliit.ee/feed/) | Vaata paadiklassi ja võistlusvooru; eelsõidu koht ei ole võistluse lõppkoht. |
| [Eesti Triatloni Liit](https://www.triatlon.ee/) | [RSS](https://www.triatlon.ee/feed/) | Kontrolli distantsi ja vanuseklassi; vanuseklassi võit ei tähenda alati üldarvestuse võitu. |
| [Eesti Judoliit](https://judo.ee/) | [RSS](https://judo.ee/feed/) | Vaata kaalukategooriat ja turniiri taset ning erista üksikmatši tulemust lõplikust medalist. |
| [Eesti Purjetamise Liit](https://puri.ee/) | [RSS](https://puri.ee/feed/) | Erista üksiku võistlussõidu tulemust regati koondtulemusest ning kontrolli paadiklassi. |
| [Tartu Ülikooli korvpallimeeskond](https://basket.ut.ee/) | [RSS](https://basket.ut.ee/feed/) | Kontrolli vastast, sarja ja lõppskoori; poolajaseis või tulevase mängu tutvustus ei ole lõpptulemus. |
| [Korvpalliklubi Kalev](https://bckalev.ee/) | [RSS](https://bckalev.ee/feed/) | Vaata täpset meeskonda ja võistlussarja; klubi enda hinnang mängule ei ole sõltumatu analüüs. |
| [Eesti Uisuliit](https://www.uisuliit.ee/uudised) | [RSS](https://www.uisuliit.ee/uudised.rss) | Erista lühi- ja vabakava ning võistluse lõpptulemust; võistlusele sõitmise teade ei kinnita veel tulemust. |

### Kultuur ja muusika

| Allikas | RSS | Mida kontrollida? |
| --- | --- | --- |
| [Eesti Noorsooteater](https://www.eestinoorsooteater.ee/) | [RSS](https://www.eestinoorsooteater.ee/feed/) | Kontrolli esietenduse tegelikku kuupäeva ja lavastuse autorite rolle; piletimüügi algus pole esietendus. |
| [Eesti Joonisfilm](https://joonisfilm.ee/) | [RSS](https://joonisfilm.ee/feed/) | Erista festivalile valimist, nominatsiooni ja võitu; vaata filmi täpset auhinnakategooriat. |
| [Eesti Pärimusmuusika Keskus](https://folk.ee/uudised) | [RSS](https://folk.ee/uudised.rss) | Vaata auhinna aastat ja kategooriat ning seda, kas valiku tegi publik või žürii. |
| [Eesti Jazzliit](https://jazz.ee/) | [RSS](https://jazz.ee/feed/) | Eelvalik, lõppvalik ja auhinna võit on eri sündmused; kontrolli täpset valikuastet ja korraldajat. |
| [Eesti Disainerite Liit](https://www.edl.ee/uudised) | [RSS](https://www.edl.ee/uudised.rss) | Võrdle teate avaldamispäeva gala või näituse kuupäevaga ning kontrolli auhinna täpset nimetust. |
| [Tallinn Fashion Week](https://tfw.ee/) | [RSS](https://tfw.ee/feed/) | Vaata, kas jutt käib väljakuulutatud programmist või toimunud sündmusest; korraldaja pildid pole automaatselt vabakasutuses. |
| [Eesti Muusikaauhinnad](https://www.muusikaauhinnad.eu/) | [RSS](https://www.muusikaauhinnad.eu/feed/) | Kontrolli auhinna aastat ning erista kandideerimist, nominatsiooni ja lõplikku võitjat. |
| [Moonwalk](https://www.moonwalk.ee/blog) | [RSS](https://www.moonwalk.ee/blog?format=rss) | Erista tulevase loo väljakuulutamist ilmumisest; agentuur esindab artiste ja selle hinnangud ei ole sõltumatu arvustus. |
| [Legendaarne Records](https://legendaarne.ee/) | [RSS](https://legendaarne.ee/feed/) | Kontrolli ilmumiskuupäeva ja väljaande täpset nime; eeltellimus või kaubapakkumine ei tõenda uut ilmunud albumit. |

## Paranduse pakkumine

Katkise või muutunud aadressi puhul kontrolli esmalt organisatsiooni enda veebilehel avaldatud RSS-viidet. Parandusettepanekus lisa allika nimi, vana ja uus avalik aadress ning kontrollimise kuupäev. Kirjelda, kas kontrollisid ainult faili vormingut või ka kanali sisu ja seost avaldajaga.

Kui muudad allikat, hoia `sources.json` ja `feeds.opml` omavahel kooskõlas. Ära lisa loendisse paroole, API-võtmeid, kontopõhiseid linke ega privaatseid kontaktandmeid.

## Sisu kasutamine

See kogumik sisaldab viiteid ja lühikesi allikakirjeldusi. Lingitud uudiste tekst, fotod ja muu materjal kuuluvad nende õiguste omajatele. RSS-kanali avalikkus ei anna automaatselt luba sisu või pilte uuesti avaldada; vaata avaldaja kasutustingimusi. Organisatsiooni loendis olemine ei tähenda tema heakskiitu Uudised.ai-le ega kogumiku koostaja kinnitust iga tema väite kohta.

## English

A curated list of **42 Estonian first-party organizational news sources**, including **40 RSS feeds** and two website-only entries. Import `feeds.opml` into an RSS reader, or use `sources.json` for public metadata and source-specific reading questions. The list covers government, work and money, health and education, environment, local government, sport and culture. It is a selection, not a complete national directory.

Curated by [Uudised.ai](https://uudised.ai/); a searchable version is available at [uudised.ai/allikad](https://uudised.ai/allikad). Uudised.ai is an automated AI news publication without a human editor and is identified here as the curator, not as one of the organizational primary sources.

The 40 feeds passed a dated technical readability/format check on 31 October 2026. Validation does not guarantee continuing availability, publication frequency, factual accuracy or republication rights. Article text, images and other linked material remain subject to their publishers and rights holders.
