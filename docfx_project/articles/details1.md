**Succesvol Specification by Example Toepassen**

Specification by Example
========================

Wat is Specification by Example
-------------------------------

In een Agile of DevOps omgeving waar verwacht wordt dat teams steeds
sneller gaan opleveren en kwaliteit een continu proces is, zien we
steeds meer organisaties zoeken naar een geschikte aanpak om de
kwaliteit van het product te verhogen. Criteria die hierbij meespelen
zijn veelal de volgende:

-   Minder re-work;

-   Optimale balans tussen risico en klantwaarde;

-   Hogere efficiëntie.

Een manier om hier mee om te gaan is het toepassen van Specification by
Example (SbE). Hierbij wordt vroeg in het ontwikkelproces op functioneel
niveau acceptatiecriteria en scope beschreven op een manier waarbij deze
ook bruikbaar zijn als functionele documentatie en uitvoerbaar als test.
Het is echter geen testaanpak. Het is een kwaliteitsaanpak voor Agile en
DevOps omgevingen.

Vormen van Specification by Example
-----------------------------------

Er zijn meerdere verschijningsvormen van Specification by Example. De
meest voorkomende zijn Acceptance Driven Development (ATDD) en Behaviour
Driven Development (BDD). Het verschil zit hierbij in de manier van het
beschrijven van de voorbeelden. Bij ATDD wordt in het voorbeeld gericht
op beschrijven van het "Wat". Met andere woorden hierin beschrijft men
vooral het resultaat in een specifieke situatie. Bij BDD richt men zich
op het beschrijven van het "Hoe". Hierbij wordt dus het gedrag van de
applicatie beschreven in een bepaalde situatie. Beide vormen gebruiken
in de beschrijving business taal en geen Technische IT termen.

Naast deze twee vormen die gericht zijn op de functionele kant van het
product is het ook mogelijk dit concept toe te passen op de technische
kant van het product. Dan heeft men het over Test Driven Development
(TDD). Hierbij gaat het dan om het beschrijven van de werking op unit
niveau in de code.

Al deze aanpakken hebben een shift left doel. Met andere woorden, deze
aanpakken zorgen ervoor dat kwaliteit in een zo vroeg mogelijk stadium
in het ontwikkelproces wordt meegenomen. Hierin zit ook de grootste
overeenkomst tussen de verschillende aanpakken. In basis zijn het allen
technieken waarbij er in het ontwikkelproces vooraf gespecificeerd wordt
aan de hand van voorbeelden en verwacht gedrag alvorens er code wordt
ontwikkeld.

Hoe toe te passen
=================

Kwaliteit binnen Agile
----------------------

In 2003 introduceerde Brian Marick de Agile Testing Kwadranten. Dit is
een model wat verschillende perspectieven weergeeft die relevant zijn
bij productontwikkeling. Hieronder is een afbeelding van dit model.

![](media/image2.jpg){width="6.495833333333334in"
height="3.089583333333333in"}

In de kwadranten zijn voorbeelden gegeven van activiteiten die passen
bij het kwadrant. Specification by Example zit hier in de twee linker
kwadranten. Het is een manier om het ontwikkelproces te ondersteunen en
begeleiden. Hier zitten de vormen ATDD en BDD aan de bovenkant. Deze
zijn gericht op de business/functionele kant. TDD zit aan de techniek
kant, dit richt zich op het technische aspect van het product. Naast
deze verdeling kan er ook gekeken worden naar de Agile Testing Pyramid.
Wanneer we dan de verschillende vormen hierop plotten krijgen we een
volgende interpretatie. TDD vindt plaats onder in de pyramide, op unit
niveau. BDD zit in het midden dan hebben we het over integratie/service
niveau. ATDD tot slot zit vooral boven in de pyramide. Dan hebben we het
over E2E en gebruikersinterface niveau.

![](media/image3.png){width="3.4803149606299213in"
height="2.437007874015748in"}

TDD Concept
-----------

TDD is een practice uit Extreme Programming (XP). Hierbij is het
toegepast met het gebruik van Unit Testen. Hierbij schrijft men eerst
(een set aan) unit testen die het gewenste gedrag beschrijven. Daarna
wordt de productiecode ontwikkeld. Wanneer de testen slagen herschrijft
men de code zodanig dat het functioneel dezelfde werking houdt maar
zodat de code ook voldoet aan de coding standards die worden toegepast
binnen het team. Deze laatste stap noemt men het refactoren van de code.
In onderstaande afbeelding is het proces schematisch weergegeven.

![](media/image4.png){width="4.586111111111111in"
height="2.161111111111111in"}

Het grote voordeel van deze werkwijze is dat er in een vroeg stadium
duidelijkheid en afbakening van de scope plaatsvindt. Dit haalt
onduidelijkheden en vragen naar voren in het proces en voorkomt daarmee
een groot deel re-work. Daarnaast geeft het ook afbakening van het
werkpakket. Hiermee worden teams constanter en voorspelbaarder qua
output. Een ander voordeel is dat de geproduceerde code altijd testbaar
is. Voor toekomstige wijzigingen is er nu ook al een regressietest. Met
andere woorden weten we dan beter of er onbedoeld wijzigingen hebben
plaatsgevonden op plekken die we niet verwachten.

Een aspect waar wel bij stil gestaan dient te worden is dat een hoge
mate van code coverage (aantal unittesten per regel code) een vals
gevoel van veiligheid kan geven. Er zal kritisch gekeken moeten worden
naar de dekking van deze unittesten.

Werken met voorbeelden
----------------------

Door de testen te beschreven in de taal van de business worden deze ook
leesbaar voor rollen die meer vanuit een functioneel/business
perspectief bezig zijn met het product. De vorm waarin deze voorbeelden
worden beschreven kan per organisatie en product verschillen echter is
het wel altijd van belang dat deze in businesstaal worden geformuleerd.
Dit kan in verhalende vorm maar ook meer schematisch dmv tabellen. Deze
voorbeelden zijn het meest waardevol wanneer die worden opgesteld met
verschillende disciplines. De meest voorkomende samenstelling is
Business Analist, Developer en Tester, ook wel Three Amigos genaamd. Het
is aan te raden dit aan te vullen met andere rollen die bij het product
betrokken zijn. Dit kan per organisatie verschillen.

Wanneer we dit koppelen aan het TDD-concept ontstaat het volgende
plaatje:

Het start met bespreken van scope en wens door de Three
Amigo![](media/image5.JPG){width="6.495833333333334in"
height="3.452777777777778in"}'s en definiëren van de voorbeelden. Van
daaruit wordt de definitieve scope voor de komende iteratie vastgesteld.
Tijdens de iteratie wordt met behulp van de besproken scope en
specificaties de functionaliteit ontwikkeld. Hierin zal ook het
automatiseren van deze scenario's plaatsvinden. Dit kan bestaan uit
aanvullen en aanpassen van de bestaande set. Hierna kan op basis van
feedback van de verschillende stakeholders de volgende iteraties worden
bepaald.

Specificatie als documentatie
-----------------------------

De grootste kracht van Specification by Example is dat de beschreven
voorbeelden gelijk ook een groot deel van de documentatie kunnen vormen.
Voor ATDD en BDD gaat het dan om de functionele documentatie. Deze kan
door gebruikers geraadpleegd worden om de werking van het product te
leren. Bij TDD is het een deel technische documentatie en beschrijving
van de specifieke stukken code. Doordat deze voorbeelden uitvoerbaar
zijn als test is de kwaliteit van deze documentatie altijd inzichtelijk.
Zodra een test faalt betekend dit dat of de documentatie óf de werking
van de applicatie moet worden aangepast. Bij een succesvolle uitvoer van
de testen weet men ook dat dat de beschreven werking ook daadwerkelijk
de werking is.

![](media/image6.png){width="2.734027777777778in" height="1.61875in"}Rol van de tester
--------------------------------------------------------------------------------------

Zoals eerder beschreven is het essentieel om bij SbE een
multidisciplinaire aanpak te hanteren. Dit biedt diverse voordelen. Zo
is het op deze manier makkelijk om een gezamenlijk beeld te vormen
rondom een requirement. Eventuele verschillen in interpretatie kunnen al
vroeg worden afgevangen en besproken. Daarnaast brengt iedere rol andere
expertise mee in de discussie. In deze paragraaf gaan we vooral in op de
rol en inbreng van de tester. Voor dit te doen zullen we eerst kort
ingaan op de titel tester. Zeker in Agile of DevOps omgevingen zien we
de term tester steeds meer verdwijnen. Veelal hebben we het over
Developers of Engineers. Dit is ook zeker terecht. Vanuit Sogeti hebben
we het over het algemeen over T-Shaped professionals. Deze T-Shaped
professionals maken het mogelijk dat binnen een multidisciplinair team
er ook Cross-functional (X-functional) gedrag kan worden getoond. Dit
houdt in dat men ook taken oppakt die niet direct bij de kerncompetentie
passen. B.v. een tester die ontwikkel taken oppakt of een beheerder die
testtaken uitvoert. Over het algemeen zien we binnen deze teams alsnog
wel dat ieder teamlid een hoofdverantwoordelijkheid op zich neemt. Het
teamlid binnen het team wat zich bezighoudt met het kwaliteitsbewustzijn
van een team noemen we in dit document de tester.

Dan blijft de vraag, wat is de rol van deze tester in een SbE-aanpak? Om
te beginnen zien we dat testers de mindset hebben om in risico's te
denken. Waar andere rollen vaker in kansen en mogelijkheden denken zal
een tester hier een kritische houding aannemen en deze mogelijkheden
toetsen op eventuele risico's. Dit valt in de Agile Test Kwadranten aan
de Critique the Product kant (Q3 en Q4). Hierbij komt het gestructureerd
aanpakken van deze risico's als waardevol aspect. Dan gaat het om zowel
experience based als coverage based test approaches. Waar de overige
rollen veelal experience based met voorbeelden of scenario's komen kan
de tester dit aanvullen met coverage based aanpakken.

Een andere rol van een agile tester is *Guide Development* (Q1 en Q2).
Hier zien we ook termen terugkomen in de kwadranten die passen bij SbE.
Dit helpt het kwaliteitsbewustzijn in het team te vergroten en daarmee
een teamverantwoordelijkheid te maken.

Samengevat is het niet alleen aan de tester om deze taken op te pakken
maar wel om het team hierin te begeleiden.

Automatisering
==============

Waarom automatiseren
--------------------

Alles wat tot nu toe is beschreven in dit document is mogelijk zonder
automatisering. Wanneer SbE correct wordt toegepast is de stap naar
automatisering wel klein. Het voordeel hiervan is vooral het verhogen
van de doorloopsnelheid en mogelijkheid tot vergroten van de schaal. Dit
draagt ook bij aan het verkorten van de feedbackloop. Daarom zou het
automatiseren geen doel op zichzelf moeten zijn maar om succesvol SbE
toe te passen is het over het algemeen wel noodzakelijk om gebruik te
maken van tooling.

Welke tooling is geschikt
-------------------------

De keuze voor een tool of toolset is afhankelijk van de omgeving. Groot
deel van deze keuze hangt al af van de taal waarin ontwikkeld wordt.
Sommige tools zijn specifiek voor bepaalde talen, een aantal tools zijn
in meerdere talen beschikbaar. De meeste tools zijn ook opensource.
Hierbij is het dan ook belangrijk om te kijken naar hoe actief de
achterliggende community is en hoeveel informatie erover te vinden is
over het gebruik van de tool.

Bekende en veelgebruikte tools voor Java omgevingen zijn o.a.:

-   Cucumber

-   FitNesse

-   Robot Framework

Bekende tools voor .NET omgevingen zijn o.a.:

-   SpecFlow

-   Robot Framework

-   Behat

In hoofdlijnen zijn dit keyword-driven testtools welke een koppeling
maken tussen de in businesstaal beschreven voorbeelden en de
productiecode. Het implementeren van een dergelijke tool vraagt
specifieke kennis.

Roadmap
=======

In onderstaande afbeelding is een basis roadmap neergezet om succesvol
SbE toe te passen. Hiervoor zijn twee assen gedefinieerd: "People" en
"Technology". Beide aspecten zijn noodzakelijk om tot een succesvolle
toepassing van SbE te komen.

![](media/image7.jpg){width="6.495833333333334in"
height="3.654166666666667in"}

Resultaat
=========

Bij een goede toepassing van Specification by Example kan een
organisatie een aantal positieve resultaten bereiken. De belangrijkste
zijn:

1.  Minder re-work doordat verwachte resultaat in een eerder stadium
    helder en afgestemd is.

2.  Een optimale balans tussen risico en potentiele waarde binnen het
    ontwikkeltraject. Dit omdat de verschillende rollen gezamenlijk
    beoordelen wat de risico's en kansen zijn.

3.  Efficiënter ontwikkeltraject. Door de multidisciplinaire aanpak zijn
    er minder overdrachtsmomenten.

4.  Accurate documentatie. Bij het geautomatiseerd uitvoeren van de
    beschreven voorbeelden is direct de correctheid van de documentatie
    geborgd.

Zoals in het begin beschreven is SbE dus een kwaliteitsaanpak voor Agile
en DevOps omgevingen. Het draagt bij aan het verhogen van de kwaliteit
van het product en het invullen van de klantwens.
