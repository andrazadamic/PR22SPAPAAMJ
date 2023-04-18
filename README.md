# Analiza kaznivih dejanj v Sloveniji


### Projektna naloga za predmet Podatkovno rudarjenje, Fakulteta za računalništvo in informatiko, 2022/2023

*Sašo Primožič, Ambrož Perovšek, Andraž Adamič, Matija Ječnik*

## Opis podatkov

[Vir podatkov](https://podatki.gov.si/dataset/mnzpkazniva-dejanja-od-leta-2009-dalje)

Podatki so podani v datotekah za vsako preteklo leto iz obdobja 2010-2019. V datoteki so zajeta vsa kazniva dejanja, za katera je policija vložila kazensko ovadbo ali poročilo. Združuje kazniva dejanja in osebe, udeležene v kaznivih dejanjih.

Struktura baze za kazniva dejanja (KD) je sledeča:
- številka za štetje in ločevanje posameznega kaznivega dejanja
- datum storitve kaznivega dejanja (MM.LLLL)
- ura storitve kaznivega dejanja (intervali v obliki HH:mm - HH:mm)
- dan v tednu (opisan z besedo)
- Policijska uprava storitve kaznivega dejanja
- atribut o tem, ali je osumljenec policiji znan ali ne (povratnik)
- klasifikacija kaznivega dejanja (zakon/člen/odstavek/točka/alinea - tekst člena)
- poglavje zakonika
- vrsta kriminalitete (splošna/gospodarska)
- vrsta kriminalitete (organizirana)
- vrsta kriminalitete (mladoletniška)
- dokončanost kaznivega dejanja - DA/NE
- kriminalistična označba 1
- kriminalistična označba 2
- kriminalistična označba 3
- uporabljeno sredstvo 1
- uporabljeno sredstvo 2
- uporabljeno sredstvo 3
- uporabljeno sredstvo 4
- upravna enota, kjer je bilo storjeno kaznivo dejanje
- podroben opis prizorišča kaznivega dejanja
- leto zaključnega dokumenta
- vrsta zaključnega dokumenta
- številka za štetje in ločevanje oseb, udeleženih v kaznivih dejanjih
- kot kaj nastopa oseba v kaznivem dejanju
- starostni razred, ki mu oseba pripada ob storitvi kaznivega dejanja
- spol
- državljanstvo osebe (le slovensko in tuje)
- poškodba osebe
- vpliv alkohola
- vpliv mamil
- pripadnost organizirani združbi
- materialna škoda v EUR

## Opis problema

Problem, ki ga želimo rešiti s to analizo podatkov, je razumevanje trendov in vzorcev v kriminaliteti v Sloveniji v obdobju od leta 2010 do 2019 oziroma kamor segajo najzgodnejši zapisi kaznivih dejanj. Pomembnejši cilji in vprašanja, na katera bomo skušali odgovoriti tekom analize podatkov, vključujejo naslednje:

- Trendi v kriminaliteti: Kako se je število kaznivih dejanj spreminjalo skozi leta? Ali so se določene vrste kaznivih dejanj povečevale ali zmanjševale v analiziranem obdobju?
- Geografska analiza: Kje se je največ kaznivih dejanj dogajalo v Sloveniji v različnih letih? Ali obstajajo določene policijske uprave ali regije, kjer je kriminalnost višja v primerjavi z drugimi?
- Vrste kaznivih dejanj: Katera kazniva dejanja so najpogostejša v Sloveniji? Ali so se vrste kaznivih dejanj spreminjale skozi leta?
- Osebe udeležene v kaznivih dejanjih: Kakšne so značilnosti oseb, udeleženih v kaznivih dejanjih, kot so starostni razred, spol, državljanstvo itd.?
- Vpliv alkohola in mamil: Kako pogosto so alkohol in mamila vpleteni v kazniva dejanja? Katera kazniva dejanja so najpogosteje povezana z alkoholom ali mamili?
- Dokončanost kaznivih dejanj: Kolikšen delež kaznivih dejanj je bil dokončan in koliko jih je ostalo poskusov?
- Organizirana kriminaliteta: Kako se je organizirana kriminaliteta pojavljala v Sloveniji v analiziranem obdobju? Katera vrsta kaznivih dejanj je najpogosteje povezana z organiziranimi združbami?
- Materialna škoda: Kolikšna je bila povprečna materialna škoda, povzročena s kaznivimi dejanji v analiziranem obdobju? Katera vrsta kaznivih dejanj je povzročila največjo materialno škodo?
- Čas kaznivega dejanja: Ob kateri uri je izvedenih največ kaznivih dejanj? Ali ura vpliva na količino izvedenih kaznivih dejanj v analiziranem obdobju?

Te cilje in vprašanja bomo poskušali doseči z uporabo statističnih analiz, grafičnih prikazov, primerjav med leti, geografskih analiz ter drugih metod analize podatkov, ki nam bodo omogočile boljše razumevanje kriminalitete v Sloveniji ter identifikacijo ključnih trendov in vzorcev.

## Rezultati, analize in ugotovitve

Vmesne ugotovitve so rezultat analiziranja in vizualizacije podatkov iz ciljev analize oseb in času kaznivih dejanj. 
- Osebe, udeležene v kaznivih dejanjih
    - Graf storilcev kaznivih dejanj, ločen glede na spol osumljenca

    ![SPOL](https://user-images.githubusercontent.com/96880463/232913529-a640ddf6-9cbd-40a5-9194-915878526d48.png)

    Iz grafa lahko razberemo, da je število osumljencev moškega spola približno petkrat večje kot od nasprotnega spola.
    
- Čas kaznivega dejanja
    - Graf kaznivih dejanj po urah

    ![URE](https://user-images.githubusercontent.com/96880463/232913381-f97a2ef9-98b8-4bd6-954c-800ee8ee5f2f.png)
    
    Največ kaznivih dejanj se zgodi med 00:00-00:59, sledi mu 23:00-23:59, najbolj varne pa so jutranje ure (03:00-03:59).

    - Po dnevih v tednu

    ![DNEVI](https://user-images.githubusercontent.com/96880463/232913418-6fd4f029-e07f-4a73-b817-30dcfa595342.png)

    Ponedeljek in petek imata največje število kaznivih dejanj, tesno pa jim sledijo ostali dnevi v tednu. Izjema tu sta sobota in nedelja, kjer opazimo rahlo znižanje.

    - Po letih v obdobju 2010 do 2019

    ![LETA](https://user-images.githubusercontent.com/96880463/232913540-d6c991cb-e2a0-4ecc-a416-386d5fda9459.png)
    
    Število kaznivih dejanj pada, ko se približujemo koncu obdobja, za kar pa obstajajo še neodgovorjena vprašanja.
    
#### Odprta vprašanja


Vzroki za spremembe trendov:
- Če opazimo upad kaznivih dejanj v določenem obdobju, lahko različni dejavniki, kot so spremembe v zakonodaji, izboljšane policijske metode ali družbene spremembe, prispevajo k temu trendu

Področja s pomanjkljivimi podatki in neprijavljanje: 
- Analiza podatkov o kriminaliteti temelji na prijavljenih kaznivih dejanjih, kar pa ne zajema vseh dejansko izvedenih kaznivih dejanj. Neprijavljanje ali neprepoznavanje kaznivih dejanj je lahko pogost pojav v kriminaliteti in lahko vpliva na natančnost analize podatkov.
