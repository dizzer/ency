Gestructureerde tekst en tekst analyse
======================================

## Barbara Bordalejo

over 

1. Waarom studenten japanologie zich iets zouden aantrekken van Digital Humanities
2. Een voorbeeld van Digital Humanities research

## Feedback blogs ency15-10

* [voetnoten in pandoc](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown.html), markdown smaken ([coggle markdown](http://bloggle.coggle.it/coggle-markdown-reference))
* zotero citation 2 pandoc - [howto: Working with bibliographies](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown.html)
* (La)TeX en Japans
* beelden?
* _digital resilience_

## Waar zitten die data?

Concept open data, voorbeelden: [New York City](http://www.nyc.gov/html/datamine/html/home/home.shtml), [Dublin](http://dublindashboard.ie/pages/index). Te volgen trend.

> Open data is information that is freely available & accessible, with no restrictions imposed by copyright, patents or other control mechanisms.

Maar je krijgt zelden de gewenste data in één pak, vaak moet je die op verschillende plaatsen gaan zoeken, en even zelden krijg je ze mooi gestructureerd.

Idealiter kunnen we de hand leggen op gegevens in de vorm van tekstbestanden met rijen en kolommen, dit soort bestanden heet csv (_comma separated values_). Data in csv formaat zetten is één manier om die te structureren. Wanneer we verschillende bestanden gaan verbinden komen we tot een relationele database.

Niet alle data leent zich er evenwel toe om op deze manier weer te geven. Een andere structureringsmethode is met markup ("tags"), dan hebben we het over xml.

Aan de basis van al die (Open) Data, en van al de tools die we gaan zien liggen dus bestanden in platte tekst bestaande uit:

  1. lijstjes (gestructureerd in csv), of 
  2. gestructureerde [xml](http://www.w3schools.com/xml/default.asp)/html

Naast gestructureerde tekstbestanden is er natuurlijk ook heel veel ongestructureerd materiaal. Je kan ook hier tools gebruiken om dat soort teksten te gaan manipuleren en onderzoeken (cfr. infra).

In elk geval zijn, naast persoonlijke informatiestromen, publieke data een tweede soort informatiestromen waarmee we moeten leren omgaan.

### Manovich

Concreet voorbeeld verschil traditioneel kwalitatief onderzoek en DH: [Manovich](http://ojs.arts.kuleuven.be/index.php/imagenarrative/article/view/133)  

>This article presents the first project in digital humanities which uses digital image analysis and visualization for the study of a massive image collection - one million manga pages. These pages correspond to 883 manga series that were available as “scanlations” (manga digitized and translated by fans) in the fall 2009. Using computational techniques we were able to systematically analyze the visual language of special pages inserted by fans in scanlated versions, and also study visual differences between the pages from original Japanese publications and official English translations. The result is a better understanding of the multiple "mangas" which make up the "manga universe."

### Text analysis

[TAPoR - Text Analysis Portal for Research](http://www.tapor.ca/)

Demo Virtualbox & unix shell (hoe je met de unix shell onderzoeksgegevens kunt manipuleren) - chasen: morfologische parser voor Japans 

Bron: [History 9877A: Digital Research Methods - William J Turkel ](http://williamjturkel.net/teaching/history-9877a-digital-research-methods-fall-2013/)

Meer specifiek:

“Basic Text Analysis with Command Line Tools in Linux.” 2015. William J Turkel. Accessed May 5. http://williamjturkel.net/2013/06/15/basic-text-analysis-with-command-line-tools-in-linux/.

“Working with Structured Data Using Command Line Tools in Linux.” 2014. William J Turkel. Accessed February 19. http://williamjturkel.net/2013/09/03/working-with-structured-data-using-command-line-tools-in-linux/.

“Simple XML Parsing and Graph Visualization with Command Line Tools in Linux.” 2014. William J Turkel. Accessed February 19. http://williamjturkel.net/2013/09/16/simple-xml-parsing-and-graph-visualization-with-command-line-tools-in-linux/.


### Network analysis

[NodeXL Graph Gallery](https://www.nodexlgraphgallery.org/Pages/Default.aspx)

[Palladio](http://palladio.designhumanities.org)


### Social media analysis

twitter mining -- hfdst 1 

Russell, Matthew A. 2014. _Mining the Social Web: [data Mining Facebook, Twitter, Linkedin, Google+, GitHub, and More]_. 2. ed. Beijing: O’Reilly.

<!-- (vermeld rmarkdown en i-python notebooks) -->

### Cleaning data

OpenRefine 

- [Introduction](http://openrefine.org/), 2de filmpje "Clean and transform data"
- Hooland, Seth van, Ruben Verborgh, and Max De Wilde. 2013. “Cleaning Data with OpenRefine.” Programming Historian. August 5. http://programminghistorian.org/lessons/cleaning-data-with-openrefine.html.

## Oefeningen 

1. Exporteer je zotero database (of een deel daarvan) naar een csv-bestand. Deze export-optie zit standaard niet in zotero. [Dit forumbericht](https://forums.zotero.org/discussion/23259/export-to-excel-spreadsheet/) suggereert een aantal mogelijkheden, de ene al wat ingewikkelder dan de andere. Kies de beste voor jou.
    *  Open het geëxporteerde csv-bestand in een spreadsheet. Spoel terug naar je cursus informatiekunde en bekijk wat je met de daar aangeleerde excel-technieken kan doen met deze data. 
    *  Kan je iets met openrefine doen om deze data properder te maken of is data-cleaning hier niet van toepassing?
    *  Kan je iets met [Palladio](http://palladio.designhumanities.org) doen? 
2. Installeer [paper machines](http://papermachines.org) voor je versie van zotero. Selecteer een collectie en probeer uit te vissen wat papermachines (een tool voor topic modeling) precies doet met je gegevens. Een alternatieve vorm van 'literatuurstudie'?
3. Oefening op zotero database met [SQLite Manager](http://royce.kimmons.me/tutorials/zotero_to_excel). Je kan je zotero db ook gebruiken om de structuur van een database te leren zien en om stoemelings wat SQL te leren.  Gebruik [dit script](https://github.com/RoyceKimmons/Zotero-to-Excel-SQLite-Export) op een __kopie__ van je database en probeer een aantal SQL commando's, [select](http://www.sqlcommands.net/sql%2Bselect/)bijvoorbeeld.
