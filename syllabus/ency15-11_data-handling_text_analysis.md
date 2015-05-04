Gestructureerde tekst en tekst analyse
======================================

## Barbara Bordalejo

over 
1. Waarom studenten japanologie zich iets zouden aantrekken van Digital Humanities
2. Een voorbeeld van Digital Humanities research

## Feedback blogs ency15-10

* footnotes in pandoc, markdown flavours
* LaTeX and Japanese characters
* _digital resilience_

## Waar zitten die data?

Concept open data, voorbeelden: [New York City](http://www.nyc.gov/html/datamine/html/home/home.shtml), [Dublin](http://dublindashboard.ie/pages/index)Te volgen trend.

> Open data is information that is freely available & accessible, with no restrictions imposed by copyright, patents or other control mechanisms.

Maar je krijgt zelden de gewenste data in één pak, vaak moet je die op verschillende plaatsen gaan zoeken, en even zelden krijg je ze mooi gestructureerd.

Idealiter kunnen we de hand leggen op gegevens in de vorm van tekstbestanden met rijen en kolommen, dit soort bestanden heet csv (comma separated values). Data in csv formaat zetten is één manier om die te structureren.

Niet alle data leent zich daar evenwel toe. Een andere structureringsmethode is met markup ("tags"), dan hebben we het over xml.

Aan de basis van al die (Open) Data, en van al de tools die we gaan zien liggen:

  1. lijstjes (gestructureerd in csv), of 
  2. gestructureerde [xml](http://www.w3schools.com/xml/default.asp)/html

Naast gestructureerde tekstbestanden is er natuurlijk ook heel veel ongestructureerd materiaal. Je kan dan tools gebruiken om dat soort teksten te gaan manipuleren en onderzoeken (cfr. infra).


In elk geval zijn, naast persoonlijke informatiestromen, publieke data een tweede soort informatiestromen waarmee we moeten leren omgaan.


### Manovich

Concreet voorbeeld verschil traditioneel kwalitatief onderzoek en DH: [Manovich](http://ojs.arts.kuleuven.be/index.php/imagenarrative/article/view/133)  

>This article presents the first project in digital humanities which uses digital image analysis and visualization for the study of a massive image collection - one million manga pages. These pages correspond to 883 manga series that were available as “scanlations” (manga digitized and translated by fans) in the fall 2009. Using computational techniques we were able to systematically analyze the visual language of special pages inserted by fans in scanlated versions, and also study visual differences between the pages from original Japanese publications and official English translations. The result is a better understanding of the multiple "mangas" which make up the "manga universe."

### Text analysis

<!-- Tapor vermelden -->

demo Virtualbox & unix shell (hoe je met de unix shell onderzoeksgegevens kunt manipuleren)

### Network analysis

palladio

[NodeXL Graph Gallery](https://www.nodexlgraphgallery.org/Pages/Default.aspx)

### Social media analysis

demo twitter mining -- hfdst 1 o'reilly 

<!-- (vermeld rmarkdown en i-python notebooks) -->

### Cleaning data

demo open refine

## Oefeningen 

1. Exporteer je zotero database (of een deel daarvan) naar een csv-bestand. 
2. Installeer [paper machines](http://papermachines.org) voor je versie van zotero. Selecteer een collectie en probeer uit te vissen wat papermachines (een tool voor topic modeling) precies doet met je gegevens. Een alternatieve vorm van 'literatuurstudie'?