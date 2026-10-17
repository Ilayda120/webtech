# Labo 3 - reflecties

Naam: Ilayda yigit

## 1. Kleurenstalen

- Welke twee waarden uit de user agent stylesheet moest je op de lijst wegwerken, en waar las je ze af?
- Wat verandert er aan de banden als je het venster hoger maakt, en wat verandert er niet?

## 2. Slogan

- Welke property centreerde de tekst, en welke de kolom?
text-align: center centreerd het tekst en margin: 0 auto centreerde de kolom.

- Waarom werkte de padding op de knop pas na `display: inline-block`?
Dat is omdat `<a>` een standaard `display: inline` is. Bij een inline-element telt de browser de verticale padding niet mee in de lay-out, dus de knop werd niet hoger. Met `display: inline-block` wordt het element een blok dat wel ruimte inneemt voor zijn padding, breedte en hoogte.

## 3. Tabblad

- Wat is de visuele breedte van het tabblad, en waarom is dat exact 15rem en geen 15rem plus padding plus border?
Het is een standaard instelling zodat je zelf niet alles handmatig moet opgeven?

## 4. Donut

- Waarom werkt `height: 70%` op de cirkel, terwijl F3.2 zegt dat een procentuele hoogte meestal niets doet?
height werkt enkel als de ouder een vaste waarde heeft (wat ik dus heb gedaan)

- Tegen welke maat van de ouder rekende de browser `margin: 15%`: de breedte of de hoogte?
padding en margin in procenten rekenen altijd tegen de breedte van de ouder, ook boven en onder.        slide 11 :D

## 5. Landingspagina

- Gaf je `main` een `height` of een `min-height`, en waarom?
min-height omdat bij een vaste `height` de inhoud eruit kan lopen.

- Wat gebeurt er met de twee helften als je een regeleinde zet tussen `</article>` en `<div class="afbeelding">`?
Bij mij is er niks gebeurd? volgens theorie zou de afbeelding er niet bij paasen en naar onder springen?

## Thuis: B3.1 (met AI of zonder AI)

Welke route koos je? Bij de AI-route: prompt en onbewerkte output staan in `site/review/`, en dit corrigeerde ik (met verwijzing naar de sectie of het foutnummer):

1. Code die opzich niet echt nodig was (bv: spacing-schaal bij root)
2. Niet echt mooi (saaie kleuren en design)
3. Geen gewenste resultaten (bv alles was niet perfect gecentreerd)

AI (claude) prompt:
/*

Zie onderstaand opdracht en maak css
Werk de nabouwen af die in de sessie niet lukten. Doe daarna B3.1 uit de syllabus voor je site, met AI of zonder AI: reset.css uit template.zip (Digitap) in site/css/ , gelinkt vóór stijl.css op elke pagina, een gecentreerde leeskolom ( max-width en margin: 0 auto ), minstens drie kaartjes met padding, border-radius en een zachte schaduw (3.5), en consistente spacing via tokens en de eenrichtingsstrategie (3.6). Kies je de AI-route, bewaar dan je prompt en de onbewerkte output in site/review/ en schrijf in je README wat je corrigeerde: vaste maten waar grenzen hoorden, magic-number-marges, een nuke-reset (AI-kader hoofdstuk 3). Push met "site: boxmodel". Lees voor de theorieles 4.1 tot en met 4.3 van de syllabus

onderstaand is reset.css
/* reset.css - the project reset of Web Technology (syllabus 3.3)
   Link it before stijl.css and leave it alone: your own CSS goes in stijl.css. */

/* 1. A predictable box: width and height include padding and border */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* 2. Browser margins are our decision, not the browser's */
body, h1, h2, h3, h4, h5, h6,
p, figure, blockquote, dl, dd {
  margin: 0;
}

/* 3. Media never spills out of its container, and is a block, not a letter */
img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}

/* 4. Form controls use the same typography as the page */
input, button, textarea, select {
  font: inherit;
}

zie ook code van één van mijn site pagina
<!doctype html>
<html lang="nl">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Mijn Hobby's</title>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="over-mij.html">Over mij</a></li>
                <li><a href="hobby.html">Mijn Hobby's</a></li>
                <li><a href="boodschappenlijst.html">Mijn Boodschappenlijst</a></li>
            </ul>
        </nav>
    </head>
    <body>
        <header>
            <h1>Mijn Hobby's</h1>        
        </header>
        <main>
            <h2>Series (anime) bekijken</h2>
                <p>Ik ben dol op Japanse media zoal anime en manga. 
                <p> Voor anime's raad ik zeker Witch Hat Atelier aan!</p>
                <img src="witch-hat-atelier.jpg" alt="Foto van Hoofdpersonage Coco van Witch Hat Atelier">
                </p><a href="https://www.crunchyroll.com/" target="_blank">Crunchyroll</a> is een website waar je anime kan bekijken!</p>
        </main>
        <footer>
            <p>Ilayda Yigit</p>
            <p>1IT4</p>
            <p>AP Hogeschool, Ellermanstraat</p>
        </footer>
    </body>
</html>
