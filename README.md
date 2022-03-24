# Team Dikdik

## Inhoudsopgave
- [Opdracht 2](#opdracht-2)
  * [1. Afbeeldingen (door Farrahton)](https://github.com/ROEL2407/Browser-tech-team1#1-afbeeldingen-door-farrahton)
  * [2. Custom fonts (door Marloes)](https://github.com/ROEL2407/Browser-tech-team1/#2-custom-fonts-door-marloes)
  * [3. Kleur & kleurenblindheid (door Marloes)](https://github.com/ROEL2407/Browser-tech-team1/#3-kleur-kleurenblindheid-door-marloes)
  * [4. Muis en trackpad (door Roel)](https://github.com/ROEL2407/Browser-tech-team1#4-muistrackpad-door-roel)
  * [5. Breedband internet (door Roel)](https://github.com/ROEL2407/Browser-tech-team1#5-breedband-internet-uitzetten-door-roel)
  * [6. JavaScript (door Farrahton)](https://github.com/ROEL2407/Browser-tech-team1#6-javascript-door-farrahton)
  * [7. Cookies (door Lisanne)](https://github.com/ROEL2407/Browser-tech-team1#7-cookies-door-lisanne)
  * [8. localStorage (door Lisanne)](https://github.com/ROEL2407/Browser-tech-team1#8-localstorage-door-lisanne)

## Opdracht 2
De website die wij hebben onderzocht is https://www.vegan-store.eu.

### 1. Afbeeldingen (door Farrahton)
In Chrome ga je naar preferences -> security & settings -> site setting -> content -> images 

Nu de foto's eenmaal uit staan, ziet de website er als volgt uit. Opvallend is dat de productafbeeldingen lazy worden geload en een styling hebben die de 'placeholder' voor een ongevonden foto wazig maakt. De foto bovenin de navigatiebalk heeft wel de 'placeholder'. 
<img src="https://user-images.githubusercontent.com/92303930/159916272-66a80e3f-d919-443e-9b63-e046779f25b0.png">

Hieruit kunnen we opmerken dat ze geen ALT-tekst hebben toegevoegd, terwijl ze wel een alt tag hebben. 
<img width="1228" alt="altTag" src="https://user-images.githubusercontent.com/92303930/159916367-9c604698-26d9-4a7e-ba7d-0434d017498b.png">

### 2. Custom fonts (door Marloes)
Het probleem met custom fonts zijn dat deze soms niet geladen worden of dat de gebruiker ervoor kiest om deze niet te gebruiken.
Via uBlock origin kan je extere letterypes blokkeren, de website veranderd verder niet dus ze maken geen gebruik van externe leterypes. 
De zoekbalk en winkelmandje maken gebruik van een icon font, zodra dit font er niet is het icoon niet meer zichtbaar. 

Ervoor

<img width="250" alt="Met iconen" src="https://user-images.githubusercontent.com/24413936/159945711-e6315fa7-fee2-43a9-b8a8-e14c0e62bf3d.png">

Erna

<img width="250" alt="Zonder iconen" src="https://user-images.githubusercontent.com/24413936/159945896-84ad259b-9c74-43db-930d-2093410ff88d.png">

### 3. Kleur & kleurenblindheid (door Marloes)
Via de instellingen van je Mac kan je kiezen voor grijswaarden om zo geen kleuren te zien, de website is al erg zwart wit en hierdoor is deze zonder kleur ook prima te gebruiken.

<img width="1280" alt="Zwart wit website" src="https://user-images.githubusercontent.com/24413936/159946373-b5fad3b0-630d-4e0e-a178-8166e13a3420.png">

De website is wit met zwarte tekst waardoor het voor iedereen leesbaar is. Via een contrast checker kan je zien dat het contrast bij een aantal elementen niet goed genoeg is zoals bij de tekst in de button en het jaar in de footer.

Contrast button

<img width="250" alt="contrastknop" src="https://user-images.githubusercontent.com/24413936/159946515-d8d3cb7c-e6c2-4f9b-a181-9d47f5512667.png">


Contrast jaar in footer

<img width="250" alt="contrastjaar" src="https://user-images.githubusercontent.com/24413936/159946531-66395e0d-0ee1-42f3-bfbb-d67d10bdf17a.png">

Met de contrast checker kan je ook meteen kijken hoe de website er voor iemand die kleurenblind is uitziet. Met deze extensie aan ben ik door de site heen gegaan. 
De roze accenten veranderen wel van kleur maar de iconen blijven leesbaar.


<img width="343" alt="Contrast checker" src="https://user-images.githubusercontent.com/24413936/159946711-332c492a-1293-460f-a399-e11ce528f383.png">


<img width="1280" alt="Kleurenblind" src="https://user-images.githubusercontent.com/24413936/159946771-86285012-22b5-476e-8add-3ac5637ccdfa.png">


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

<img src="https://user-images.githubusercontent.com/90243819/159915105-53e3f3fc-0e94-4d3c-bc76-c08a21c06b90.png">

### 6. JavaScript (door Farrahton)

In Chrome ga je naar preferences -> security & settings -> site setting -> content -> JavaScript

Opmerkelijk is dat in combinatie met het uitzetten va nde afbeeldingen dat er niets meer in de plaats komt van de afbeeldingen. Het is dan helemaal leeg. 
<img width="1223" alt="geenImages+Java" src="https://user-images.githubusercontent.com/92303930/159916618-77c0c167-6d14-492d-9c57-ffd5afc94d9e.png">


Alleen JavaScript uit zorgt voor een resultaat waarin de doorklik carousel niet meer werkt en de productfoto's daardoor allemaal onder elkaar staan. 
<img width="1227" alt="javaUit" src="https://user-images.githubusercontent.com/92303930/159916673-ba971349-fc99-43f8-aeef-f1329bcc8fbf.png">


Je kan zonder JavaScript nog wel klikken op de dropdown menu linkjes en doorverwezen worden naar een nieuwe path. Echter, als je daar aankomt is de pagina helemaal leeg op de navigatie balk en de footer na.
<img width="1280" alt="navMenShoes" src="https://user-images.githubusercontent.com/92303930/159916733-47f6f6d9-1700-49c5-98cb-96c72e0c191c.png">

Hetzelfde geldt voor de zoekbalk. Er komen geen resultaten uit. 
<img width="1280" alt="zoeken" src="https://user-images.githubusercontent.com/92303930/159916786-e9027e17-6e8c-4382-b14d-0604c551f8d1.png">


Je kan nog op login klikken en het formulier invullen en submitten, maar eenmaal op de volgende pagina is de Captcha gebroken. Je kan niet laten weten dat je geeb robot bent en kan daarom niet me de submit knop doorgaan. 
<img width="1280" alt="captcha" src="https://user-images.githubusercontent.com/92303930/159916838-f1021d2c-bd82-4df1-83b4-5913c3615f23.png">

De taal veranderen kan ook niet meer. 
Het is ook nog mogelijk om de betaalvaluta te veranderen. 
Informatie die volgt na het klikken op help doet het nog wel. 

Helaas als je een bestelling wilt volgen heb je weer pech, want alleen de path veranderd. Er komt geen informatie in beeld, zoals met JavaScript wel gebeurd.
<img width="1224" alt="orderTrack" src="https://user-images.githubusercontent.com/92303930/159916903-dc86aa94-3bad-443a-a9f1-3bfae22b4216.png">
<img width="1222" alt="orderWelGetracked" src="https://user-images.githubusercontent.com/92303930/159916933-90dbf3cc-84d7-480c-9f32-42748f59ca95.png">

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
