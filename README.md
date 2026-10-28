# Accessible Website

Ontwerp en maak voor een opdrachtgever een website toegankelijk volgens WCAG richtlijnen.

De instructie van deze leertaak staat in [WIKI](https://github.com/fdnd-task/all-human-accessible-website/wiki)

Live website: https://lyannebos.github.io/all-human-accessible-website/

## Inhoudsopgave Readme
  * [intro](#intro)
  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [toegankelijkheid](#toegankelijkheid)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Intro
Opdrachtgever: Charley Muhren, Dilia Porcelijn

Charley wil een platform waar studenten en docenten 
tekenmethodes kunnen vinden om hun (reflectieve) vakproces visueel te maken. 
oud-student Dilia had voor haar eindproject een een uitgewerkt design gemaakt voor de website 
Visual Thinking. Aan ons de vraag om die visie tot leven te brengen.

## Beschrijving
<!-- In de Beschrijving staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->
De pagina Tekenmethodes laat een overzicht zien van tekenmethodes binnen een categorie, zoals "Leren over jezelf en Reflecteren".
Sinds vorige sprint review zijn er een aantal dingen nieuw bijgekomen op de pagina. Zo is er nu een eerste versie van de filters en filterknop erbij gekomen, die van onderen
naar binnen springt.

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->
Ik heb gebruik gemaakt van semantische HTML, en van een popover knop voor de filters. In de css is die verder opgemaakt en door een media query ook responsive. De code staat voor nu nog echt in de steigers.

## Toegankelijkheid
Tijdens deze sprint lag de focus ook op toegankelijkheid. Zo hebben we veel tests moeten uitvoeren en de resultaten moeten noteren. Dit is waar ik de afgelopen tijd qua toegankelijkheid aan heb gewerkt:

- Zoekbalk kreeg een echt label: eerst alleen een `placeholder`. Nu zit er een `<label>` omheen...

- Filterknoppen hielden hun naam: eerst zat de tekst buiten de `<button>` in een `<p>`. De knoppen was daardoor naamloos voor een screenreader. Dus nu hebt ik de tekst teruggezet in de knop.

- Footer-afbeeldingen kregen alt: drie plaatjes hadden helemaal geen alt-attribuut. Het logo kreeg alt="" omdat het decoratief is, de social-iconen kregen echte tekst.

- <nav> uit de footer gehaald: twee navigaties zonder onderscheid. Opgelost zonder ARIA, volgens de HTML-spec.

## Bronnen
MDN, Popover API — voor je filterpaneel en popovertargetaction="hide"
https://developer.mozilla.org/en-US/docs/Web/API/Popover_API

MDN, <nav> — voor de opbouw van je breadcrumb met een <ol>
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav

HTML Standard, the nav element — waarom je footerlinks géén <nav> nodig hebben
https://html.spec.whatwg.org/multipage/sections.html#the-nav-element

The A11Y Project, How to hide content — voor je visueel verborgen label met clip-path
https://www.a11yproject.com/posts/how-to-hide-content/

W3Schools, filteren met JavaScript — 
](https://www.w3schools.com/howto/howto_js_filter_elements.asp#gsc.tab=0)

## Licentie
This project is licensed under the terms of the [MIT license](./LICENSE).
