
#### inhoudsopgave

[Responsive webdesign](#resposive-webdesign)





# Resposive webdesign 

Omdat het gebruik van mobiele telefoons en tablets etc.. op het internet toeneemt, is het belangrijk dat wij als toekomstige developers rekening houden om content op een manier te ontwerpen dat deze goed werkt voor verschillende schermformaten. Responsive webdesign wordt dit genoemt, is een ontwerpstratergie dat zich aanpast aan de behoeftes van gebruikers en de apparaten door de lay-out van de webpagina aan te passen aan de grootte van het scherm.

Naast dat de lay-out zich moet aanpassen aan het scherm is het ook van belang dat alle interactieve-functionaliteiten werken naar behoren, omdat tegenwoordig alle hand-on devices touchscreen hebben.

denk hierbij bijvoorbeeld aan hover-effecten.

## Responsive-design

###html-meta-tag

Bovenaan de html-pagina tussen de <head> tag, hebben we de <meta> tag:

<!DOCTYPE html>
<html lang="en">
  <head>
    …
    <meta name="viewport" content="width=device-width, initial-scale=1">
    …
  </head>

In de <head> staan allerlei gegevens voor de browser en zoekmachines om de pagina op de juiste manier weer te geven. De data is niet zichtbaar op de pagina , maar werkt in de browser. 

Deze <meta name="viewport" content="width=device-width, initial-scale=1"> tag zorgt ervoor dat de pagina's er beter uit zien op devices van verschillende grootte. Dat het zich aanpast aan de viewport van het device. Dit is verre van genoeg.

Dit is een minimale optie om je pagina goed weer te geven op andere devices. Om het lay-out te optimaliseren maken we gebruik van media-queries.

### Media-queries

Met @media queries kunnen we de css-properties aanpassen, als de pagina om een bepaalde grote wordt weergegeven.

-------------------------------------

#infomain {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 1em;
    justify-content: center;
    align-items: center;

    @media only screen and (max-width: 640px) {
        display: grid;
        grid-template-columns: 1fr;
    }
  }

  In dit geval zal de grid-display-columns veranderen van 3 columns naar 1 column als de pagina een breedte krijgt van 640px. De foto's worden nu elk onder elkaar weergegeven en niet naast elkaar.

![Pagina op mac](../Ravi/assets/images/pagina-op-lappie.png)

-------------------------------------

  li p {
	margin:0;
	top:0;
	right:50%;
	translate:50%;
	position:absolute;
	white-space:nowrap;
	opacity:0;
	transition:.5s;

    @media only screen and (max-width: 640px) {
        opacity: 1;
    }
}

Op de pagina zijn de namen van de personen alleen zichtbaar zodra je erover hovert. Bij schermen kleiner dan 640px worden de namen altijd zichtbaar gemaakt omdat je niet kunt hoveren met een touchscreen device.

![Pagina op iphone](../Ravi/assets/images/pagina-op-smartphone.jpg)


# het team
Ik ben Ravi en ik heb mijn studie afgerond in Electrical Engineering. Hoewel ik dat altijd interessant vond, merkte ik na een tijdje dat het niet meer echt bij me paste. Daarom ben ik me gaan richten op development. Inmiddels heb ik wat ervaring opgedaan in HTML, CSS en JavaScript. Daarnaast heb ik ook gewerkt met backend-technologieën, zoals databases, crud-systemen en het express api.

Mijn github:
https://github.com/Ravirkt

# Aanpak
Voor de squadpage heeft elk lid van het team zijn eigen versie van de pagina gemaakt, zodat iedereen het volledige codeerproces kon doorlopen en zelf uitvoeren. Hoewel we dezelfde opzet hebben aangehouden, is elke versie uniek op zijn eigen manier. Uiteindelijk hebben we de verschillende stijlen en functionaliteiten van ieders pagina gecombineerd om tot de definitieve versie te komen. Hierdoor hebben we een gevarieerde en gezamenlijke pagina gecreëerd die de input van elk teamlid weerspiegelt.


# over ons zelf, retrospective , wat ging goed en slecht, wat kan de volgende keer beter.

Het verloop van het project is soepel en goed verlopen. Het teamwork verliep uitstekend; iedereen kwam zijn taken na en hield zich aan de gemaakte afspraken. Er was een sterke teamspirit, waarbij ieder teamlid initiatief toonde om het project succesvol af te ronden. Daarnaast was het fijn om te zien dat iedereen bereid was elkaar te helpen wanneer dat nodig was, wat de samenwerking nog beter maakte. Dankzij deze gezamenlijke inspanning hebben we het project tijdig en naar tevredenheid afgerond. 