# Labo 4 - reflecties

Naam: Ilayda yigit

## 1. Drie kolommen

- Op welk element staat `display: flex`, en op welke elementen staat `flex`?
display:flex heb ik bij main gezet 
en flex heb ik bij div:nth-child gezet

- Waarom staan die twee niet op hetzelfde element?
Ze staan op verschillende elementen omdat ze verschillende taken hebben: 
display: flex maakt van main een container en de 3 divs zijn directe kinderen als flex-items indeelt. 

## 2. Navigatiebalk

- Welke property verdeelt de ruimte langs de hoofdas, en welke lijnt uit op de kruisas?
Dat doet justify-content: space-bewteen. Die verdeelt de ruimte tussen de onderdelen van de header, van links naar rechts. 
En align-items lijnt ze van boven naar beneden uit.

- Wat gebeurt er met de links als je `gap` vervangt door `margin-right` op elke `li`?
Bij mijn site stond er geen verschil qua iuterlijk als ik text-align of gap gebruikte.


## 3. Mondriaan

- Welke twee vlakken moest je expliciet plaatsen, en waarom volstond de impliciete vulling voor de andere vier?
De lila en olijfkleurige vlakken zijn expliciet, omdat ze elk twee kolommen breed zijn. De andere vier zijn elk maar één vak groot, dus die kunnen automatisch in de open plekken terechtkomen.

- Waarom is `gap` hier beter dan een border op elk vlak?
omg ik had hierbij eerst border gekozen maar die botste met andere rasters waardoor de borders binnen het schilderij dikker werden. 
Het nam me een tijdje om te beseffen dat het gap moest zijn en dat de 'randen' in de schilderij daadwerkelijk het achtergrond is van het schilderij

met andere woorden: opgaves niet skimmen

## 4. Trap

- Wat zie je als je de `grid-row`-declaraties weghaalt, en waarom?
Alle tredes komen helemaal vanboven staan (rij 1). Zonder grid-row worden ze automatisch op het eerste rij gezet.

- Wat betekent `grid-column: 4 / -1` voor de laatste trede, en waarom werkt het hier ook?
-1 betekent dat het inhoud naar de laatste lijn wordt verplaast. Hier werkt het omdat de vierde trede als laatste staat bij kolom 4 en rij 4, en -1 verwijst ook naar het laatste.

## 5. Dierenasiel Zonnehoek

- Hoeveel layoutcontainers telt deze pagina, en welk gereedschap koos je voor elk?

De pagina telt zes soorten layoutcontainers:
1. `body`, gereedschap: grid (`auto 1fr auto`), voor header, main en footer onder elkaar met de footer onderaan.
2. `header`, gereedschap: flexbox, logo en nav uit elkaar met `space-between`.
3. `nav ul`, gereedschap: flexbox, de links in een rij met `gap`.
4. `footer`, gereedschap: flexbox, om de tekst te centreren.
5. `.kaarten, gereedschap: grid met drie kolommen, waarbij `.uitgelicht` twee kolommen breed is.
6. `.kaart` (vijf keer), gereedschap: flexbox in een kolom, met `flex: 1` op de beschrijving zodat de knop onderaan staat.

- Verklein het venster tot de helft: wat breekt er, en in welk hoofdstuk wordt dat opgelost?
alle inhoud wordt samengeduwt totdat het niet meer kan en de window het inhoud begint te bedekken. 

Dit komt doordat mijn layout vaste waarden gebruikt (`repeat(3, 1fr)`) die niet reageren op de schermbreedte. Dat wordt opgelost in hoofdstuk 6 (responsive) met media queries (6.4)!

## Thuis: B4.1 (met AI of zonder AI)

Welke route koos je? Bij de AI-route: prompt en onbewerkte output staan in `site/review/`, en dit corrigeerde ik (met verwijzing naar de sectie of het foutnummer):

1. Dubbele reset (3.3). Dit schendt een expliciete labo-regel (één gelinkte reset.css). Twee resets kunnen elkaar bovendien stilletjes tegenspreken dus heb ik die weggehaald 

2. main zonder width: 100% (4.7). heb `width: 100%` daar geplaatst want zonder dat werd de kolom te smal op korte pagina's (4.7).

3. `.uitgelicht` gebruikt nu `span 2` in plaats van `1 / 3`, zodat het ook werkt als de kaart niet eerst staat (4.6).