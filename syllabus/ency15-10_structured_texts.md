

Gestructureerde tekst
=====================

## Dienstmededeling:

* wieltjes!
* bompa heeft gelijk

## vraaggesprek readings en tools data handling vorige week

## principe 1: scheiden van inhoud/structuur en opmaak 

Borduurt verder op het html/css verhaal dat tijdends de OPO informatiekunde al aan bod kwam.

Ter herhaling een oude, maar nog steeds welsprekende presentatie:
[Gestructureerde tekst -- presentatie Andreas Bovens](http://japanologie.arts.kuleuven.be/bestanden/Gestructureerdetekst.pdf)

Moet ik dan html (of xml) kunnen schrijven?

## principe 2: duurzaam auteurschap 

Gebaseerd op workflow in [http://programminghistorian.org](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown). In de _philosophy_ en _principles_ paragrafen kan ik me helemaal vinden.


<!-- When you use MS Word, Google Docs, or Open Office to write documents, what you see is not what you get. Beneath the visible layer of words, sentences, and paragraphs lies a complicated layer of code understandable only to machines. Because of that hidden layer, your .docx and .pdf files depend on proprietary tools to be rendered correctly. Such documents are difficult to search, to print, and to convert into other file formats.

Moreover, time spent formatting your document in MS Word or Open Office is wasted, because all that formatting is removed by the publisher during submission. Both authors and publishers would benefit from exchanging files with minimal formatting, leaving the typesetting to the final typesetting stage of the publishing process. -->

### voordelen van plain text 

![](https://farm9.staticflickr.com/8512/8596614435_e91b832eb1_c.jpg)

>Briefly, plain text is a great format to use because (1) it can be read by any computer or device; (2) it’s future proof, since computers will always be able to read it; (3) it can be synced to all your devices; (4) it can be converted to virtually any format


### markdown

* geen taal, enkel een conventie, eenvoudige syntax
* Markdown is stilaan een de facto standaard aan het worden voor online schrijven
* _Writing in this way liberates the author from the tool_ - je kan schrijven met eender welke editor
* een markdown bestand kan als moederbestand dienen voor een breed gamma van documentformaten: wetenschappelijke artikels, wikis, syllabi, blog posts ...
* Wordpress en drupal hebben md filters
* er is ook de [markdown here extensie](https://github.com/adam-p/markdown-here) voor de browser 
> Above all, avoid the urge to format. 

<!-- Remember that you are identifying semantic units: sections, subsections, emphasis, footnotes, and figures. Even *italics* and **bold** in Markdown are not really formatting marks, but indicate different level of emphasis. The formatting will happen later, once you know the venue and the requirements of publication. -->


## demo: een totaal-workflow gebaseerd op platte tekst

### tools

- [sublime text](https://www.sublimetext.com/) (plugins marked, evernote, pandoc,git)
- git [^2]
- markdown
- iterm
- pandoc [^1]  (latex, j packages)
- zotero

> The command line is a friendly place, once you get used to it.


### publicatieformaten

- blogpost: drupal (full html, markdown filters)
- technische documentatie: github, jekyll, [read the docs](https://read-the-docs.readthedocs.org/en/latest/getting_started.html) 
- academisch: pdf (met toc)
- wiki-artikel: mediawiki
- presentatie: reveal.js

### nagare

1. folder en bestand ency15-10_structured_texts.md openen in Sublime Text
    - de tekst editor als console  
    - evernote plugin
    - distraction free mode     
    - Marked
2. tonen wat er allemaal in zit:
    - headings
    - code, blockquote (verwijs naar md syntax)
    - footnotes (plugin pandoc)[^3]
    - zotero export naar bibtex, toevoegen aan yaml info, default stijl is auteur-jaar
3.  drupal
    - c&p html (via Marked)
    - md filter 
4.  github
    - kleine aanpassing bestand en via git naar github
    - het kan ook iets mooier: jekyll
5. via pandoc naar een pdf
    - toc
    - toc links
    - footnotes & citations
    - `$ pandoc -S -o unified_workflow.pdf ency15-10_structured_texts.md -V geometry:margin=1in -N --toc --filter pandoc-citeproc`
6. via pandoc naar mediawiki & omgekeerd
    - `$ pandoc -t mediawiki -o unified_workflow.wiki ency15-10_structured_texts.md`
7. reveal.js
    - [github repo](https://github.com/hakimel/reveal.js), [features](http://lab.hakim.se/reveal-js/#/)
    - cp folder, edit index.html, koppel md-bestand
    - slides in bestand aangeven    
    - resultaat tonen op locale webserver (node.js,grunt)

<!-- Treat you source files as an authoritative version of your text, and you target files as disposable “print outs” that you can easily generate with Pandoc on the fly. -->


## oefeningen

1. Kies je qua opmaak meest gecompliceerde blogpost (ency15) en zet die manueel om naar markdown. Noteer de vragen en eventuele problemen die zich daarbij aandienen, én de oplossingen.
2. Indien die er niet niet zijn voeg dan de volgende elementen toe aan het markdown bestand: hyperlinks, beelden, lijsten (ol en ul), bibliografische verwijzing, voetnoten, blockquote, titels (h2, h3)
3. Zet het aangepast markdown bestand om naar html (welke tool?) en plak de html in een 'portfolio post' op het lab (in het 'body' veld). Gebruik het 'abstract' veld om aan te geven in welk kader deze oefening past, voor latere referentie. Noteer de vragen en eventuele problemen die zich daarbij aandienen, én de oplossingen.
4. Installeer pandoc. Noteer de vragen en eventuele problemen die zich daarbij aandienen, én de oplossingen.
5. Kopieer de broncode van je wiki-artikel voor geschiedenis naar een tekstbestand (.txt). Zet dat bestand met pandoc achtereenvolgens over naar markdown en html. Plak de html in een 'portfolio post' op het lab. Gebruik het 'abstract' veld om aan te geven in welk kader deze oefening past, voor latere referentie. Noteer de vragen en eventuele problemen die zich daarbij aandienen, én de oplossingen.
6. Combineer alle nota's in een razend interessante blogpost.
7. Voor wie durft proberen: genereer een academisch ogende pdf van je wiki-artikel met pandoc; of zet je blogpost/wiki-artikel om in een wervende presentatie met reveal.js.



Een zin die een verwijzing nodig heeft [@baker_counting_2014].


[^1]: <http://johnmacfarlane.net/pandoc/installing.html>

[^2]: <https://msysgit.github.io/>

[^3]: <http://inlustre.net/2014/01/pandoc-referencing-for-sublime-text-3-a-plugin/>