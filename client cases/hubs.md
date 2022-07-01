Title: 
# The ultimate guide to lean/agile translaiton with Contentful

Target Group: Contentful users who have problems with their localization pipeline: CEO's, marketing mensjes, ...

Goal: to give a blue print on how to work with Contentful and TMSs, how current solutions are not working, and what the key insight is to make it work, and to have content flow in all languages. 

## Intro:
The worlds of content management and translation management are, you could say, Venus and Mars. These different planets collide quite dramatically most of the time. For most companies, translation processes are the ones no-one in the content department wants to come close to, because they are too painful, always require rework and have a less than optimal result in terms of UX. 

So a lot of people turn to tools to solve this issue. (Or hire a translation project manager that will burn out within a year). They buy a content management system that promises to make sure you can publish to multiple channel and re-use your content. And the "mature" clients, as we call them, even buy a Translation Management System that integrates with that CMS. That should solve the problem. 

It appears that buying tools is not the answer. There are a lot of companies that have bought state of the art tools in both content management AND translation management and integrated this, and that are still struggling with their international content, in spite of the promise that everything would be solved by buying these tools. 

Somehow, there is no clear vision at CMS-companies on how to deal with translated content, and there is even less of a vision on how to create, manage and store your content on the side of translation tools. 

So in this article we will fill this gap. Written by Contentful-expert Dennis and Translation management expert Anouk, we have put together, from our own experiences, the ultimate guide to setting up both Contentful, and your integration with translation tools that will guarantee a happy ending: no defects, no rework, and re-usability in all languages. Which leads to the ultimate time to market, for all countries you want to reach.  

## Outline



### How are website typically built (- and translated)?
dit misschien maar een korte paragraag. 



### What do you run into? 



### how contentful is designed
This section describes the philosphy of contentful and how this translates to translation 
(dit hebben we in die presentatie ook een keer gezegd)

- Philosophy: chunks and blobs => structured blocks of content that fit together; 

Reden:
- reusability
- multi-channel
- ontkoppelen content van design (zeer belangrijk voor vertalen)
- meer complexiteit in pagina's mogelijk zonder dat je content model complex wordt

### Reality

Main problem: 
Mensen denken in termen van "oud" website bouwen, terwijl contentful een andere filosofie heeft. 

- Dit uit zich bijvoorbeeld in een design voor een gehele pagina
- bovendien is het vaak een waterval proces, waar eerst in Figma een design gemaakt wordt, en in Google docs de content. Dat geheel gaat naar de developer en die moet er maar wat van maken, zonder dat er in het design gewerkt is geweest met de structuur in contentful. 


- als de pagina niet in chunks gedesigned wordt - en waterval - dan moet de developer een pagina ontwerp in chunks gieten. 
- Allerlei design aspecten worden ad hoc opgelost in contentful, met html, markdown en code, in plaats van dat de designer wordt gevraagd om het een beetje netjes te maken. 

It creeps in: uiteindelijk is het developen van een pagina erg veel werk, doordat het design los staat van de structuur waarin het gegoten wordt. Maar: er is niet voldoende urgentie om dit aan te pakken. 

### Enter translation
This section describes what happens if, in this environment, translation is added to the process. 

- now there's a need to translate. We're going international!
- so after the pages are published, they're sent off for translation. Sounds logical, right? 

Not so much, actually. In the following sections we will describe why this approach leads to major problems that can actually stop you from international expansion. 




what happens:
- exceptions  (code, html, md) - unstructured text! in design lead to problems in translation - we will explain why
- 



### General problems with translation
This sections gives an overview of problems that arise when working in translation. 

- waterfall
- technical defects 
- rework on design 
- time to market




### Common setup with Contentful/TMS
This section explains how translation is usually viewed, as a waterfall project, and the tools are standardly designed to work that way.
(het is toch eigenlijk niet te geloven van zo'n localize hoe ze dit hebben opgezet he)
comment van een toehoorder van de Design Night: "My previous company was one of the CMS providers, and I looked in-depth into the translation feature of competitors. And they all are reinforcing the old model. Designers & developers create page templates first, then content creators fill the content in CMS and the translators deliver the content to multi-language sites."

- template a page
- waterfall approach: translate after everything is done, is reflected in the way the integrations are set up
- no means to really integrate with core process: you can't easily define what you want to send to the translators
- because the website is put together from the building blocks with code, and not in contentful, there was no context for the translator what they were doing
- big amounts of data were sent back and forth, selecting content only after data was transferred


### Problems when setting up a translation pipeline this way
This section describes the problems when viewing translation as a waterfall project

- process becomes complex because of having to account for exceptions that originates in the storage of content
  - for example: code in markdown, trying to fix it in the TMS, or by the translator => productiviteitsproblemen, toch technische defects, bladiebla


- rework in design
- designer and developer needed in operational process
- technical defects
- time to market is slow





### What is a TMS and why use it

This section explains why it is important to work with a translation tool and not have the translators work in contentful

why would you not: (hier nog even wat verzinnen!!!)
- direct publishing. 
- clarity on structure of components

But: 
- translators are used to working in their tools, can't learn all the CMSs, steep learning curve
- update management
- licensing
- terminnology
- old translations (???)

So we will have to find a way to get the first half and not lose the second half




### Practical implementation

1. tried to fix problems in the translation process that originated in the CMS: 

- complexity was too big, problem solving impossible

- freedom in design led to ad hoc development, leading to code/html/markdown





This section describes the practical implementation

- smaller pieces
=> complexity became too big, so we had to drill it down by looking at smaller pieces: pages to entries. 

- the design from 

- process: difference between operational and new stuff
- content model
- plug-in in Contentful
- middleware
- translators


### Things to think about
This section describes the things we had to make decisions about like:

- source of truth 
- level of segmentation


### Effects: 
This section describes what happens if you set this up this way

- time to market creating a page: times 5
- time to market translation: publish 3 days after last entry is done in creation process

### Next steps
This section describes what would be even better: translating the content when it is in Figma

- context, no screenshots necessary
- faster time to market
- Even less chance of design defects

### Stichtelijk woord
hier zeggen we nog iets leuks

problemen komen door waterval,
de meeste kun je oplossen door gewoon goed te kijken en het te fixen waar het gebeurt
maar het wordt zo ingewikkeld dat dat bijna niet gaat
dus daarom moet je naar kleinere pieces

EN: idealiter schrijf je je content in een omgeving waar ook op deze manier gewerkt wordt. Dus niet in docs, waar alles mag, en wat je vervolgens dan weer naar deze limitaties moet krijgen. Idem voor design. 


