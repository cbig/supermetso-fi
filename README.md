# Zonation-priorisointi metsolle sopivista soidinmaisemista

## Yleistä

Työn tavoitteena oli arvottaa suomalaista metsämaisemaa sen mukaan, mitä tiedämme metson soidinpaikkavaatimuksista. Priorisointi perustuu metsäaineistoon ja ihmisvaikutusaineistoon (tarkempi kuvaus alla). Lopputulosta on verrattu tiedettyihin soidinpaikkoihin, ja tämä vertailu osoitti, että lopputuloksena olleen rasterin (skenaario 6 [S6] , kts. alla) korkean prioriteetin paikat osuivat melko hyvin yksiin tunnettujen soidinpaikkojen sijainnin kanssa (lähes puolet soidinpaikoista osui parhaaseen 20 % prioriteettiluokkaan).

Tulosten avulla voidaan siis tunnistaa metson soidinpaikoille potentiaalisia metsäalueita. Tuloksia on jo käytetty hyväksi Uudenmaan Ely-keskuksen (Arto Pummila, nykyään Metsähallituksen luontopalvelut) suorittamissa metson soidinpaikkojen kartoituksissa, ja se on toiminut kiitettävästi. Käyttökelpoisuudessa voi kuitenkin olla eroja eri puolilla Suomea riippuen maiseman rakenteesta ja muista metson soidinpaikkoihin ja populaatiokokoon vaikuttavista tekijöistä.

**Alkuperäistutkimuksen viite:**

Sirkiä, S., Lehtomäki, J., Lindén, H., Tomppo, E., Moilanen, A., 2012. Defining spatial priorities for capercaillie Tetrao urogallus lekking landscape conservation in south-central Finland. Wildlife Biology. 18, 337–353.

[http://dx.doi.org/10.2981/11-073](http://dx.doi.org/10.2981/11-073)

## Analyysivariantit

### S1 - SM_01_loc

Lähtötasoa kuvaavassa tulosrasterissa on huomioitu pelkkä paikallisen *
elinympäristön laatu (indeksipiirteiden kuvaamana). Kaikki puulajit saavat 
saman painoarvon (1), ja soluun mahdollisesti osuva ihmisvaikutus saa yhtä 
suuren, mutta negatiivisen painoarvon (−1). Eri analyysipiirteiden (n=5) 
yhteisvaikutus ratkaisee tarkasteltavana olevan solun arvon suhteessa muihin 
soluihin, eikä ympäröivien solujen arvoilla ole minkäänlaista 
heijastevaikutusta solun arvoon. Toisin sanoen vaikka viereinenkin solu 
sisältäisi metsolle hyvää metsää, tämä ei vaikuta ko. solun arvoon, vaan arvo 
lasketaan kaikkien solujen yli vain perustuen niiden omiin arvoihin (ns. 
paikallinen arvo). Ihmisvaikutusrasterin negatiivinen painokerroin kuvastaa 
olettamusta, että metso aktiivisesti välttelee tällaisen maankäytön alueita.

### S2 - SM_02_loc_wgt

Tässä skenaariossa huomioidaan edelleen pelkkä paikallisen elinympäristön 
laatu. Eri puulajit saavat kuitenkin erilaiset painot:

| Puulajiryhmä  | Paino |
|---------------|-------|
| Mänty         |     3 |
| Kuusi         |     1 |
| Koivu         |     0 |
| Muut lehtipuut|     0 |
| Ihmisvaikutus |    -1 |

Painotusta tulee tulkita niin, että kussakin solussa mänty on kolme kertaa 
arvokkaampaa kuin esimerkiksi kuusi. Sen sijaan lehtipuilla ei ole mitään 
vaikutusta solun paikalliseen laatuun. Yksittäisen solun sisällä rastereiden 
arvo muuttuu siis annettujen painokerrointen mukaan, ja piirteiden 
yhteisvaikutus solussa ratkaisee edelleen arvon suhteessa muihin soluihin. 
Painotus perustuu tutkittuun tietoon siitä, että metson soidinpaikat 
sijaitsevat Suomessa pääosin havupuuvaltaisissa metsissä, etenkin kuivahkoilla 
mäntykankailla. 

### S3 - SM_03_loc_wgt_con_1

Kolmannessa skenaariossa solujen keskinäinen arvojärjestys perustuu sekä 
paikallisen elinympäristön laatuun (kuten edellä kuvatussa skenaariossa S2) 
että solujen väliseen kytkeytyvyyteen. Kytkeytyvyys on määritelty eri 
puulajirastereiden välille käyttäen 2 kilometrin keskimääräistä 
kytkeytyvyysmittaa. Tämä etäisyys on keskimääräinen kernel-tyyppinen etäisyys, 
mikä tarkoittaa, että kytkeytyvyysvaikutus ei rajoitu tähän etäisyyteen vaan 
vähenee periaatteessa äärettömyyteen saakka. Eri puulajien painotus on 
muutoin kuten edellä, mutta kytkeytyvyydellä muunnetut indeksipiirteet saavat 
2,5 -kertaa suuremman painoarvon kuin muut ominaisuudet. Tällä korostetaan 
metson soidinalueen merkitystä analyysissa. Kahden kilometrin keskimääräinen 
kytkeytyvyysmitta kattaa metson soidinpaikan lisäksi ympäröivät kukkojen 
päiväreviirit, joilla ne viettävät suuren osan vuodesta. Tämän kukkojen 
elinpiirin tai soidinalueen metsäisyys on siis analyysissa 2,5 -kertaa 
tärkeämpää kuin paikallisen elinympäristön laatu. Nyt yhtä solua ympäröivien 
solujen metsäisyys alkaa siis "heijastevaikuttaa" ko. solun arvon 
määräytymiseen, eli priorisoinnissa suositaan sellaisia alueita, joilta löytyy 
yksittäistä solua laajempia metsäkokonaisuuksia.

Kytkeytyvyyslaskut olettavat, että saman puulajin metsien välillä kytkeytyvyys 
on täydellistä. Kuusen ja männyn välillä kytkeytyvyys on suhteellisen korkeaa, 
samoin koivun ja muiden lehtipuiden välillä. Heikointa kytkeytyvyys on havu- 
ja lehtipuiden välillä. Nämä määritelmät perustuvat kuvitelmaan siitä, miten 
eri puulajivaltaiset elinympäristöt ovat kytkeytyneitä toisiinsa metson 
näkökulmasta. 

### S4 - SM_04_loc_wgt_con_2

Neljännessä skenaariossa on kaikki skenaarion S3 elementit, mutta lisäksi 
mukaan tulee kytkeytyvyys eri puulajirastereiden välillä 10 kilometrin 
keskimääräisellä kytkeytyvyysmitalla. Tämä mittakaava vastaa karkeasti 
poikueellisten metsonaaraiden vuodenaikaisliikehdintää sekä nuorten 
metsoyksilöiden muuttomatkaa synnyinseuduilta uusille alueille. Oletus siis 
on, että tämä mittakaava kattaa suurimman osan niistä tilaan liittyvistä 
ilmiöistä, jotka vaikuttavat metson paikallisen soidinpopulaation kokoon. Tämä 
kytkeytyvyystaso huomioidaan analyysissa paikallisen elinympäristön laatua 
vastaavilla painoarvoilla (taulukko 1).

### S5 - SM_05_loc_wgt_con_3

Skenaario on muutoin samanlainen kuin S4, mutta mukaan tulee sekametsää 
suosiva, metsikkötason kytkeytyvyys eri indeksipiirteiden välillä 200 metrin 
keskimääräisellä kytkeytyvyysmitalla. Sekametsässä on todennäköisemmin 
metsolle sopivaa monipuolista metsikkörakennetta, joka tarjoaa lajille sekä 
ruokaa että suojaa. Vaikka solun paikallista arvoa laskettaessa lehtipuiden 
kerroin on nolla, niin tässä kohden lehtipuilla on suuri merkitys 
sekapuustoisuuden luomisessa. Toisin sanoen ne runsaasti havupuita sisältävät 
solut, joiden lähistöllä on runsashavupuustoisia soluja joissa on seassa 
lehtipuustoa, saavat analyysissa korkeamman prioriteetin. Tämän 
kytkeytyvyystason painoarvo on sama kuin paikallisen elinympäristön laadun ja 
10 kilometrin kytkeytyvyystason (taulukko 1). 

### S6 - SM_06_loc_wgt_con_4

Lopullisessa priorisointirasterissa S6 oleva solujen arvojärjestys perustuu 
sekä paikallisen elinympäristön laatuun että solujen väliseen 
kytkeytyneisyyteen neljällä eri kytkeytyvyystasolla. Edellisten lisäksi mukana 
on nyt negatiivinen kytkeytyvyys puulajirastereiden ja ihmisvaikutusrasterin 
välillä 500 metrin keskimääräisellä kytkeytyvyysmitalla. Negatiivinen vaikutus 
on lähtöisin ihmisvaikutusrasterista, ja se kohdistuu kaikkiin muihin 
analyysipiirteisiin. Solun arvo on siis alhaisempi, jos sen lähistöllä on 
ihmisvaikutusta sisältäviä soluja. Toisin sanoen voidaan ajatella, että solun 
paikallinen ihmisvaikutusarvo ”säteilee” negatiivista vaikutusta ympäröiviin 
soluihin, vaikka nämä olisivatkin metsäisiä ja vielä ympäröity muilla 
metsäisillä soluilla. Asiantuntijatiedon mukaan soidinpaikalla olevat metsot 
alkavat häiriintyä lähestyvistä ihmisistä kun he ovat suunnilleen 500 metrin 
päässä. Myös maatalousalueiden aiheuttaman metsien pirstoutumisen 
negatiivisten vaikutusten on arvioitu ulottuvan suunnilleen tämän etäisyyden 
verran metson käyttämien metsäalueiden sisälle (nk. reunavaikutus, mm. 
lisääntynyt pienpetojen saalistus).