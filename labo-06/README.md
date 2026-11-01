# Labo 6 - reflecties

Naam: Ilayda yigit

Getest op dit echte toestel (merk, browser): apple iphone 13, safari

## 1. Kleurvlakken

- Wat gebeurt er als je de twee queries van plaats verwisselt, en waarom?
    bij een breed scherm winnen altijd de regels die onderaan staan. Staat de 600px-query onderaan, dan overschrijft die de 800px-query en krijg je dan altijd vier kolommen en nooit twee bij twee

- Waarom `100svh` en niet `100vh`?
    De kleine lettertjes op mobiel schuift de adresbalk in en uit beeld, en 100vh is dan nét te hoog


## 2. Dashboard

- Waarom staat `grid-column: 1 / -1` in de query van 50rem en niet in de basis, en waarom hoef je het in de query van 75rem niet te herhalen?
    want een query erft van de vorige, de regel blijft gelden zolang ik hem niet overschrijf 
    -> mobile-first

- Wat betekent `-1`, en wat gebeurt er als je bij de grafiek `grid-row: 2 / 4` vergeet?
    -1 is de laatste kolomlijn, dus aan de rechterkant. Zo loopt het element altijd tot het einde, ook als het aantal kolommen verandert. 

    En zonder `grid-row: 2 / 4` is de grafiek maar één rij hoog. Ze past dan niet naast de twee rijen kleine tegels waardoor de plattegrond niet meer klopt


## 3. Scheldekaai Festival

- Wat is de h1 met `clamp(2rem, 5vw + 1rem, 4rem)` op 400 px, op 800 px en op 1280 px?

- Waarom staat er een rem-term in het midden?
    5vw groeit alleen met het scherm. De 1rem zorgt dat de titel op een smal scherm niet te klein wordt en meegroeit met de tekstgrootte van de gebruiker.

- Waarom twee breekpunten voor de header, en niet één?
    1. bij 50rem komen de knoppen op één rij, 
    2. bij 75rem komt het logo links en de knoppen rechts. 
    met één breekpunt mis je de tussenstap van 900 px.

## 4. Tribune

- Waarom hoef je in de query geen `grid-row` te schrijven?
    omdat de rijen al automatisch onder elkaar komen te staan dankzij de volgorde van de HTML.

- Zou je deze tribune ook met `repeat(auto-fit, minmax())` kunnen bouwen? Waarom wel of niet?
    niet omdat met auto-fit de browser zelf kiest hoeveel kolommen er passen, dus dat aantal verandert met de breedte van het venster. dat is hier niet van toepassing aangezien de trap exact 10 vaste kolommen nodig heeft

## 5. Affiche

- Waarom zou `width: 28rem` op een telefoon een horizontale schuifbalk geven, en hoe vind je zo'n saboteur met DevTools?
    28rem is 448px en een telefoon is ongeveer 400px breed, dus de affiche is breder dan het scherm. 
    je vindt het door het venster smal te maken en in DevTools de elementen aan te klikken tot je er een vindt die breder is dan zijn ouder.

- Wat doet `top: auto` in de query, en wat gebeurt er als je het weglaat?
    top:auto haalt de top uit de basis weg, zodat de sticker niet meer vanaf boven wordt geplaatst. 

    Als je die weg haalt dan blijft de top uit de basis gelden en zit de sticker vast aan onder EN boven, waardoor hij uitrekt of op de verkeerde plek staat.

## Thuis: B6.1 (met AI of zonder AI)

Welke route koos je? Bij de AI-route: prompt en onbewerkte output staan in `site/review/`, en dit corrigeerde ik (met verwijzing naar de sectie of het foutnummer):
    zonder AI 
