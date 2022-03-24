# Team Dikdik

## Inhoudsopgave
- [Opdracht 2](#opdracht-2)
  * [4. Muis en trackpad (door Roel)](https://github.com/ROEL2407/Browser-tech-team1#4-muistrackpad-door-roel)
  * [5. Breedband internet (door Roel)](https://github.com/ROEL2407/Browser-tech-team1#5-breedband-internet-uitzetten-door-roel)
  * [7. Cookies (door Lisanne)](https://github.com/ROEL2407/Browser-tech-team1#7-cookies-door-lisanne)
  * [8. localStorage (door Lisanne)](https://github.com/ROEL2407/Browser-tech-team1#8-localstorage-door-lisanne)
  * [B. Ad blockers (privacy) (door Lisanne)](https://github.com/ROEL2407/Browser-tech-team1#b-ad-blockers-privacy-door-lisanne)

## Opdracht 2
De website die wij hebben onderzocht is https://www.vegan-store.eu.

### 4. Muis/trackpad (door Roel)
Mensen met cognitieve problemen, fysieke problemen en mensen met problemen met de zintuigen. 
Hierbij kan je bijvoorbeeld denken aan blinde mensen.

Door de pagina heen tabben gaat niet goed. Ik heb hiervoor gekozen om bij de login pagina te gaan tabben. Allereerst begin je gelijk bij de login. Hierna krijg je een aantal set tabs die niet zichtbaar zijn.
Daarna ga je langs de bovenste header. In deze header staat een language preference die uitklapt, hier tab je overigens niet door heen als je terug tabt. Focus state is voor sommige dingen wel anders vormgegeven dus hier kan een kleine verwarring van ontstaan.

Als je enige tijd door tabt kom je bij de forgot password en signup links. Deze had ik persoonlijk bij het formulier zelf verwacht. 

Je zou dit laatste probleem kunnen oplossen door de links binnen de form in de HTML te zetten of ten minste deze eronder.

Hulpbron: [https://www.abilitynet.org.uk/factsheets/keyboard-and-mouse-alternatives-and-adaptations](https://www.abilitynet.org.uk/factsheets/keyboard-and-mouse-alternatives-and-adaptations)

### 5. Breedband internet uitzetten (door Roel)
Door middel van throttling binnen de chrome browser heb ik getest hoe de ervaring is op een langzame 3g verbinding.

Dit kan je doen door de volgende stappen te volgen:
Inspecteren > netwerk > dropdown waar standaard geen throttling in staat

Hierbij zie ik geen erge fouten. De website wordt ingeladen, enkele blokken verschijnen eerst over elkaar maar dat wordt later opgelost. Afbeeldingen worden ook na de tekst pas ingeladen en worden eerst als onscherpe afbeelding ingeladen waarna deze scherper wordt.

Je zou rekening kunnen houden met mensen die reizen, bijvoorbeeld met de trein. Deze wifi is niet geheel sterk en ook open dus er kunnen extra problemen hiermee doorkomen zoals het aantal gebruikers op de verbinding. In mijn is dit een probleem die verschilt per situatie. 

In mijn ogen zijn zullen de verschillen tussen landen zonder (100%) 4G en tijdelijke problemen niet heel veel verschillen met elkaar. De pagina laadt namelijk goed in op zowel langzaam als snel 3G.

<img src="https://github.com/ROEL2407/Browser-tech-team1/blob/main/readme-images/breedband.png">

### 7. Cookies (door Lisanne)
Op de voorpagina komt er een pop-up in beeld, die met cookies in één klik te verbergen is. Zonder cookies blijft de pop-up een keer of vijf terugkomen, voordat het verdwijnt. Als de pagina herladen wordt, verschijnt de pop-up weer, evenals de "Visiting from outside Europe?" pop-up.

![](https://user-images.githubusercontent.com/90243819/159908306-3bb654cf-a9d1-4882-9be3-4f2b2d0437aa.png)

Op de pagina waarop klanten kunnen inloggen, kom ik erachter dat het probleem met de pop-up websitebreed is. Na de inloggegevens te hebben ingevuld en te hebben geklikt op "Login", kom ik op een 404 Not Found pagina. Na een seconde verschijnt de pop-up uiteraard weer (niet te zien in de screenshot).

![](https://user-images.githubusercontent.com/90243819/159909533-3dde424d-5689-4ef0-a82f-7c866f16cfac.png)

Na het aanzetten van de cookies en het inloggen op de website, zijn de onderstaande cookies aangemaakt voor het domein https://www.vegan-store.eu.

![](https://user-images.githubusercontent.com/90243819/159912493-5ca97dcc-363c-4cbd-ac98-18e32aa4723c.png)

### 8. localStorage (door Lisanne)
Omdat localStorage alleen uitgeschakeld kan worden samen met de cookies, is het niet mogelijk om erachter te komen wat er zou gebeuren als enkel de localStorage uitstaat. Het pop-up probleeem lijkt enkel te liggen aan de cookies, omdat er in de localStorage geen data staat die hier invloed op zou kunnen hebben. Het niet kunnen inloggen zou hier wel te maken mee kunnen hebben, omdat mijn e-mailadres in de key "swym-authn" staat.

![](https://user-images.githubusercontent.com/90243819/159914159-7d35bd9a-7907-4abe-9a6a-4e0dbfee50c6.png)
