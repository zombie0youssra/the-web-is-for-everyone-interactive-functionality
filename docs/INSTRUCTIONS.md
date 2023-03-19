# Interactive functionality

Ontwerp en maak voor een opdrachtgever een interactieve toepassing die voor iedereen toegankelijk is.


## Context

Deze leertaak hoort bij sprint 9 "The Web is for Everyone". Dit is een leertaak die je individueel uitvoert voor een opdrachtgever.

In het college S09W1-01-Sprintplanning-the-web-is-for-everyone wordt de opdracht uitgelegd.

Bij deze leertaak hoort de deeltaak:
- [Activity Diagram](https://github.com/fdnd-task/the-web-is-for-everyone-activity-diagram)


## Doel van deze opdracht

Tim Berners-Lee, de uitvinder van het internet zei: "The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect."

Één van de mooiste [principes](https://www.w3.org/DesignIssues/Principles.html) van het web is dat iedereen met een computer en een browser het web kan gebruik. [Het web is voor iedereen](https://www.youtube.com/watch?v=UMNFehJIi0E). 

Maar het web is geen gecontroleerde (programmeer) omgeving, je kan er gerust van uit gaan dat niemand precies hetzelfde te zien krijgt als wat jij in je browser ziet. Er zijn technische beperkingen, zoals afmetingen van de browser, grootte van het apparaat, manier van interactie, kwaliteit van de hardware, kwaliteit van het netwerk en er zijn mensen, allemaal verschillende mensen ...

Het doel van deze opdracht is te leren hoe je een interactieve functionalteit kan ontwerpen en maken met behulp van _Progressive Enhancement_ en _Feature Detection_ zodat de website het altijd doet.



## Werkwijze

Ontwerp en maak een functionaliteit voor je opdrachtgever op basis van een _user story_. De _user story_ voor sprint 9 gaat over het posten van data met behulp van de REST-API. Je bouwt je website in 3 lagen, volgens het principe van _Progressive Enhancement_.

[Progressive enhancement](https://briefs.video/videos/is-progressive-enhancement-dead-yet/) is een _(coding) strategy_ waarmee je er voor kan zorgen dat je website het altijd doet. 

1. Content: Eerst bouw je de _core functionality_ van je website in HTML en met behulp van formulieren en NodeJS, voor het server-side afhandelen van het posten van data. 
2. Presentation: Daarna voeg je CSS toe voor feedback voor de gebruiker en om de huisstijl toe te passen.
3. Client-side scripting: Tot slot ga je JavaScript (en CSS) toevoegen om de User Experience te verbeteren.

![image](https://user-images.githubusercontent.com/1391509/226204781-5594ea1b-56c3-45ac-87d4-56dd25e35e58.png)
<br><small>_The Chocolatey Layers of Progressive Enhancement_</small>


Voor deze opdracht doorloop je alle fases van de DLC [analyseren](#analyseren), [ontwerpen](#ontwerpen), [bouwen](#bouwen), [integreren](#integreren) en [testen](#testen).


### Analyseren

In de analysefase kies je een User Story waar je aan gaat werken en bekijk je hoe het posten van data werkt met de REST-API. 

#### User Stories
Kies een user story, met het label **sprint-9**, uit de backlog van het project waar je aan gaat werken. De projecten staan bij [FDND Agency](https://github.com/fdnd-agency).

#### REST-API
Bekijk in de documentatie van de API of er voor de User Story een POST endpoint is en hoe je die werkt.

### Bronnen analyseerfase

* [Wat is een REST API nou echt: het basisidee](https://blog.wearefrank.nl/wat-is-een-rest-api-nou-echt-het-basisidee)


### Ontwerpen

In de ontwerpfase ga je eerst bedenken en schetsen wat je gaat maken. Voor deze opdracht doorloop je meerdere keren de DLC omdat je de functionaliteit in 3 lagen gaat opbouwen. Je gaat dan ook meerdere keren schetsen. Eerst ontwerp en bouw je de _core functionality_ van je website in HTML en met behulp van formulieren en NodeJS, voor het server-side afhandelen van het posten van data. 

#### Wireflow
Teken de _core-functionalty_ van de _User Story_ in een wireflow. Zorg dat je de verschillende states van het formulier, het versturen van data, een _succes state_ en mogelijke _errors_ ook tekent. 

#### Breakdown
Maak een breakdown-schets waarin je de juiste HTML formulier-elementen die je nodig hebt beschrijft en pseudeo-code voor wat er server-side in NodeJS gebeurt. 

### Bronnen ontwerpfase

* [Wireflows: A UX Deliverable for Workflows and Apps](https://www.nngroup.com/articles/wireflows/)
* [The Role of Enhancement in Web Design](https://www.nngroup.com/articles/enhancement/)
* [The Input (Form Input) element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Input)
* [The Form element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)


  
### Bouwen

#### Inrichten ontwikkelomgeving
Je gaat een server-side website bouwen met Node/Express/EJS gebaseerd op een REST API met JSON. 
Installeer de Node ontwikkelomgeving en installeer de packages die je nodig hebt. Maak de files en folders aan die je nodig hebt op de Node server. 

#### Progressive enhancement
Progressive enhancement is een _(coding) strategy_ waarmee je er voor kan zorgen dat je website het altijd doet. 

1. Eerst bouw je de _core functionality_ van je website in HTML en met behulp van formulieren en NodeJS, voor het server-side afhandelen van het posten van data. 
2. Daarna voeg je CSS toe voor feedback voor de gebruiker en om de huisstijl toe te passen.
3. Tot slot ga je client-side Javascript toevoegen om de User Experience te verbeteren.

### Bronnen bouwfase

* [JavaScript Fetch API Ultimate Guide](https://blog.webdevsimplified.com/2022-01/js-fetch-api/)
* [Understanding Progressive Enhancement](https://alistapart.com/article/understandingprogressiveenhancement/)
* [The power of progressive enhancement](https://archive.hankchizljaw.com/wrote/the-power-of-progressive-enhancement/)
<!-- * [Progressive Enhancement and Data Visualizations](https://css-tricks.com/progressive-enhancement-data-visualizations/) -->


### Integreren
In de integratiefase voer je de aanpassingen door zodat iedereen ze kan zien.

Als je helemaal klaar bent en alles lokaal werkt ga je verder met het publiceren van jouw project op internet. Omdat we met Node werken is dit iets ingewikkelder dan voorheen, er moet namelijk een serveromgeving opgestart worden. Wij gebruiken cyclic.sh als hostingpartij maar je mag natuurlijk je eigen voorkeur volgen als die anders is.


### Testen

het web is geen gecontroleerde (programmeer) omgeving, je kan er gerust van uit gaan dat niemand precies hetzelfde te zien krijgt als wat jij in je browser ziet. Er zijn technische beperkingen, zoals afmetingen van de browser, grootte van het apparaat, manier van interactie, kwaliteit van de hardware, kwaliteit van het netwerk en er zijn mensen, allemaal verschillende mensen ...

In de testfase test je website in verschillende browsere en verschillende _devices_.

Gebruik [caniuse.com](https://caniuse.com), [html5test.com](https://html5test.com), [css3test.com](http://css3test.com) en [kangax.github.io/compat-table/es6/](https://kangax.github.io/compat-table/es6/) om je code te testen en te achterhalen welke technieken browsers ondersteunen. 


## Criteria
*Definitions of done*

Focus sprint 9 - De focus van deze sprint ligt op Progressive Enhancement, toegankelijkheid en testresultaten gebruiken voor het verbeteren van een ontwerp.

Doel van deze opdracht:

* je leert hoe je een interactieve functionalteit kan ontwerpen en maken met behulp van _Progressive Enhancement_ en _Feature Detection_ zodat de website het altijd doet.

Voor deze leertaak gelden de gedragscriteria:

* M: Je houdt in beginnende mate rekening met de belangen van de eindgebruiker bij het realiseren van een oplossing voor een opdrachtgever
* S: Je draagt verantwoording voor eigen resultaten, verwerkt ontvangen feedback en wijst teamleden op hun verantwoording
* C: Je kan ontwerpkeuzes, eigen ideeën en producten begrijpelijk overbrengen aan belanghebbenden
* P: Je analyseert een vraag, signaleert knelpunten en volgt de aangeboden oplossingsrichting
* P: Je schetst om gedachten en processen te verkennen en abstracte begrippen over te brengen

Deze opdracht is done als:

- [ ] Je hebt een interactieve functionaliteit ontworpen en gemaakt met Node, Express en EJS en een REST API
- [ ] Je website is online gepubliceerd
- [ ] Je hebt gewerkt volgens de verschillende fases van de development-lifecycle en je hebt je proces bijgehouden in de Wiki
- [ ] Je hebt je werk getest in verschillende browsers en devices en de test gedocumenteerd in je wiki
- [ ] Je hebt comments in je Node-code waarmee de server-side code is uitgelegd
- [ ] Je hebt in de Readme bij 'Kenmerken' uitgelegd wat Progressive Enhancement is en hoe je dit hebt toegepast

