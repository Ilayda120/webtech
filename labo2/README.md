# Labo 2 - reflecties

Naam: Ilayda Yigit

## 2. Selectors lezen

Welke elementen raakt elke selector? Eén zin per selector.

- a. `header nav ul li a`: elke a
- b. `article > p`: //elke <p> die een direct kind is van een <article>.
- c. `.uren li:nth-child(3)`: elke <li> die het derde kind is van een element met de class uren
- d. `h2 ~ p`: elke <p> na een <h2>, binnen dezelfde ouder.
- e. `.rassen li:first-child`: de eerste <li> binnen een element met de class rassen.

## 3. Voorspel, dan kijk

Vul de eerste twee kolommen in vóór je de pagina opent. Trede: herkomst, specificiteit, volgorde of overerving (of iets anders, benoem het).

| vraag | mijn voorspelling (kleur) | beslissende trede | uitkomst in de browser | juist? |
|---|---|---|---|---|
| 1 |               groen               Herkomst            groen                     v
| 2 |               blauw               spicificatie        blauw                     v
| 3 |                rood               spicificatie        rood                      v
| 4 |               groen               volgorde            rood                      
| 5 |               blauw               spicificatie        blauw                     v
| 6 |                rood               spicificatie        blauw                     
| 7 |                rood               overerving          rood                      v
| 8 |                rood               spicificatie        blauw                     
| 9 |               blauw               herkomst            rood                      
| 10 |              groen               spicificatie        groen                     v

Bij welke vraag zat je fout, en wat was de reden? (Alles juist? Welke vraag duurde het langst, en waarom?)

## 4. De nabouw

- Welke selector koos je voor de links in de navigatie, en waarom geen class?
als selector heb ik nav gebruikt. Ik heb geen class gebruikt omdat dat meer werk zou creeren (een class voor elke link terwijl je nav maar één keer hoeft te gebruiken)

- Welke regel kostte je het meeste tijd, en wat was uiteindelijk de oorzaak?
De link-knop nam me veel tijd: was constant onderlijnd al was text decoration niet aan, blijkt dat ik een fout had bij de hover code. Nu weet ik dat er geen spatie mag rond de dubbelpunt!

## 6. Je site

- Welke drie waarden staan in je tokenblok, en waarom die?
    - kleuren
    - border radius
    - box-shadow
- Wat verandert er in je site als je één token wijzigt?
kleuren wijzigen, borders kunnen ronder of scherper worden, schaduws wijzigen

## Thuis: R2.3 (met AI)

Prompt en onbewerkte output staan in `review/`. Minstens vijf bevindingen, elk met een verwijzing naar de sectie of het foutnummer:

1. Geen pixel-soep. Lettergroottes zijn uitgedrukt in rem of clamp() met vw; px komt alleen terug in borders en focusomlijningen. maar het gebruikt wel soms em.

2. Selectors zijn niet overspecifiek. Er staan geen zware ketens zoals div.container ul.menu li a.link. De selectors blijven kort en leesbaar.

3. De stylesheet gebruikt geen !important

4. Kleuren gebruiken bestaande tokens; er zijn geen losse kleurnamen verspreid door de stylesheet.

5. Geen geneste spelling. Alle regels zijn vlak geschreven tenzij @media als geneste spelling telt?

extra :D
6. Focus-offset wordt overschreven; article a:hover, article a:focus-visible zet outline-offset: 2px; 
    de latere a:focus-visible geeft 3px. 