# Labo 5 - reflecties

Naam: Ilayda Yigit

## 1. Letterraster

- Wat gebeurt er als je in de template één gebied een L-vorm geeft, en waarom?
    Die gebied zal zig uit stretchen volgens die vorm en andere gebieden bedekken.

- Hoeveel declaraties zou dezelfde plaatsing met `grid-column` en `grid-row` vragen?
    voor hele opdracht (letterraster) is dat 8 'grid-column' en 8 'grid-row' , dus 16 declaraties

## 2. Citaten

- Waarom lijnt de tweede rij bij 1280 px niet uit met de eerste zoals een grid dat zou doen?
    Flexbox werkt per rij. Elke rij verdeelt zijn eigen ruimte en kijkt niet naar de rij erboven. Er zijn geen vaste kolommen. Een grid heeft die wel, dus daar staat alles netjes onder elkaar.

- Wat verandert er als je de basis van 18rem naar 30rem zet, en waarom?
    Dan passen er minder citaten op een rij. Bij mij is het van 4 kolomen naar twee gegaan.

## 3. Fotolijst

- Waar belanden de vlakjes als je `position: relative` van de lijst weghaalt, en waarom?
    Ze belanden in de hoeken van de pagina (het venster). Een `absolute` vlakje zoekt een voorouder met een `position` anders dan `static`. Zonder `relative` op de lijst is die er niet, en rekent het vanaf de hele pagina.

- Waarom ligt roze zonder `z-index` onder groen?
    Dat komt door z-index: met z-index kan je gegevens stappelen. Welke element een hogere z-index heeft staat bovenop.

## 4. Toonzaal

- Wat gebeurt er als je `top: 0` weghaalt, en waarom?
    dan zou position: sticky niks doen. Sticky heeft een drempel nodig om te weten waar het moet blijven plakken, anders zal hij verdwijnen bij het scrollen.

- Wat is het verschil met `position: fixed` voor de rest van de pagina, en welke extra declaratie zou fixed nodig hebben?
    bij fixed hangt de balk los van de pagina, waardoor de tekst erachter schuift. fixed zou daarom padding-top: 3.5rem nodig hebben. Bij sticky blijft de balk op zijn plek, dus is dat niet nodig.

## 5. Koffiebar Kaai 12

- Welke drie vragen van deze week (container, item, plaatsing) beantwoordde je waar in deze pagina?
    Container: 
    body is een grid met named areas en .kaart is een flex-column. 
    Item: de prijs krijgt margin-top: auto zodat hij onderaan staat. 
    Plaatsing: de badge ligt met position: absolute op de kaart, 
    en de balk blijft plakken met position: sticky.

- Haal `aspect-ratio` weg bij de foto's: wat gebeurt er met het rooster, en waarom?
    Elke foto krijgt dan zijn eigen hoogte, omdat ze allemaal een andere verhouding hebben. Ze zijn zonder aspect-ration niet meer even lang

## Thuis: B5.1 (met AI of zonder AI)

Welke route koos je? Bij de AI-route: prompt en onbewerkte output staan in `site/review/`, en dit corrigeerde ik (met verwijzing naar de sectie of het foutnummer):
    Zonder AI geprobeerd!