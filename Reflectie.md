# individuele opdracht proftaak Teun Luijken


## week 2
In week 2 zijn we begonnen met het opzetten van het versiebeheersysteem, de meeste van ons hebben weinig tot geen ervaring hiermee. ook zijn we begonnen aan het maken van de agenda module. We hebben ook het Framework van Sjoerd besproken of we deze moeten gebruiken of niet.

Voordelen van het framework:
-Het is al gemaakt dus is het minder werk voor ons om te maken
-Het geeft ons ervaring met het maken van een framework

Nadelen van het Framework:
-Wij maken zelf het framework niet, hierdoor krijgen wij geen ervaring
-Wij moeten zelf eerst goed inlezen om het framework te kunnen gebruiken.


ik vond dat het contact in de projectgroep wat beter kon. de communicatie onderling was nog niet stevig en iedereen was nog wat onzeker had ik het gevoel.


---
## week 3
Bij het opstartcollege hebben we Tiled uitgelegd gekregen.
Een deel van het team is verder gegaan aan het maken van de agenda, Timo en ik zijn begonnen met het maken van de map en het inlezen hiervan en van de sprites, de Tilemap zal in CSV formaat worden opgeslagen dus heb ik een klasse gemaakt die bestanden in het CSV formaat kan inladen. Ook heb ik een klasse gemaakt die de spritesheet van de Tilemap kan inladen zodat deze sprites apart gemaakt gebruikt kunnen worden. Ik heb deze klasse eerst in een apart project aangemaakt zodat ik deze vlug kon testen en zodat ik me puur op deze klassen kon focussen.



' int amount = ((sourceImage.getWidth() / singleWidth) * (sourceImage.getHeight() / singleHeight));
        BufferedImage[] images = new BufferedImage[amount];

        int id = 0;
        for (int i = 0; i < sourceImage.getHeight(); i += singleHeight) {
            for (int j = 0; j < sourceImage.getWidth(); j += singleWidth) {
                //Crop the source image in many individual sprites
                //And put them in an array with their ID according to their index
                images[id] = sourceImage.getSubimage(j, i, singleWidth, singleHeight);
                id++;
            }
        }
        return images;
    }

Omdat ik nog niet helemaal bekend was met het framework en omdat we nog niet helemaal besloten hadden of we het framework nou echt zouden gebruiken heb ik de keuze gemaakt om de klassen die ik vandaag maak statisch zou houden zodat we deze niet hoeven te gherschrijven als we ons focussen op een van de twee opties.

net als de week hiervoor vond ik het contact in de groep een beetje stijf verlopen, dit is ook mijn schuld aangezien ik ook niet de beste praten ben. dit ligt denk ik aan het feit dat we allemaal elkaar nog niet goed kennen omdat we allemaal uit andere klassen komen van vorige periode.


---
## week 4
De TiledMap wordt toch blijkbaar opgeslagen in een JSON formaat, hierdoor hebben we de CSVloader moeten herschrijven zodat het werkt met een JSON bestand. Timo en ik zijn hiermee deze week verder mee gegaan. Wij hadden beide geen ervaring met het JSON formaat dus moesten wij hier eerst nog onderzoek in moeten doen voordat we hiermee verder konden.

de rest van de week was dus gespendeert aan het aanpassen van de CSV loader zodat deze json kan lezen, we hebben gebruitk gemaakt van een library die dit werk grotendeels voor ons doet. daartussen hebben we een laag gemaakt om de library te vertalen naar iets dat wij wat beter begrijpen en wat dingen voor ons versimpeld

De communicatie is een beetje aan het verbeteren maar ik denk dat er nog wel wat spanning is tussen de projectgroep over het framework en de toepassing hiervan. hier moesten we van maurice eigeblijk een designsessie over houden maar dit hebben we niet uitgevoerd.





---
## week 5
Vanwege spanning rondom het Framework is de productiviteit van de projectgroep in mijn mening een beetje gekeldert. Omdat wij niet tot een beslissing zijn gekomen hebben wij samen met Maurice een bespreking gehouden over wat wij van het framework vinden en de beslissing die we moeten nemen.

in de besprekking is onder andere ten spraken gekomen wat wij vinden van het framework, hoe we verder moeten gaan en hoe wij als groep zijn omgegaan met het probleem. 

In de Bespreking zijn we tot de conclusie gekomen dat we verder gaan met het framework, onder andere omdat een groot deel van de code al gebaseerd is op het framework. Ook heb ik me kunnen uiten over mijn mening hoe met probleem is omgegaan.

ik vond de communicatie na deze bespreking een stuk soepeler verlopen omdat we allemaal elkaar een stuk beter begrepen 

---
## week 6
Deze week ben ik begonnen met het "Domme" deel van de Npc dat op basis van instructies een sprite door kan geven om te tekenen, deze Npc's hebben een loopanimatie in vier verschillende richtingen, alle docenten maken gebruik van dezelfde sprites, de leerlingen maken gebruik van 5 verschillende spritesheets waar ze allemaal een willekeurig selecteren.

![alt text](https://github.com/t-luijken/teun_luijken_FPindividu/blob/master/structuur-Simulation.png)


   int spriteSeed = random.nextInt(5);

    int spriteOffset; 
          switch (spriteSeed) {
            case 0:
                spriteOffset = 0;
                break;
            case 1:
                spriteOffset = 3;
                break;
            case 2:
                spriteOffset = 6;
                break;
            case 3:
                spriteOffset = 51;
                break;
            case 4:
                spriteOffset = 54;
                break;

            default:
                spriteOffset = 0;
                break;'
                

Zo hebben wij besloten om de simulatie ongeveer te laten werken, in de werkelekheid zal de simulatie waarschijnlijk niet precies dit diagram volgen maar het zal wel ongeveer dit diagram volgen.



---
## week 7

We zijn begonnen met de PathFinding van de simulatie, omdat we vanuit thuis moeten merken merk ik wel een negatieve impact op mijn werkvermogen, het is moeilijker hulp te vragen en het is makkelijker om afgeleid te worden. De deadline is ook een week versteld omdat het moeilijker is om thuis samen te werken. Deze week ben ik verder gegaan met het NPC renderen en om deze te integreren met de PathFinding NPC's ook ben ik begonnen met het toevoegen van commentaar aan de code. eerst dacht ik dat dit geen groot probleem zou worden maar dat bleek naderhand toch een grotere klus dan verwacht te zijn. Commentaar toevoegen aan code die je zelf niet geschreven hent en die de auteur zelf een maand geleden geschreven heeft is een grotere uitdaging dan dat ik verwacht had.

---
## “In het bedrijfsleven wordt gebruik gemaakt van JavaFX"
Er wordt tegenwoordig nog genoeg gebruik gemaakt van JavaFX, er wordt nog steeds open-source aan gewerkt en de laatste release was deze maand nog. 

of JavaFX in de toekoms nog veel gebruikt zal worden is de vraag. Tegenwoordig worden steeds meer applicaties webbased, deze worden gemaakt in talen zoals javascript of PHP, als deze trend zo doorgaat zal javaFX steeds minder gebruikt worden.

in conclusie wordt JavaFX nog wel gebruikt wordt, maar dat dit in de toekomst mischien minder gebruikt zal worden

### Bronnen:

https://jonathangiles.net/one-guys-perspective-on-javafx/

https://jaxenter.com/20-javafx-real-world-applications-123653.html

https://www.javacodegeeks.com/2016/07/javafx-real-world-apps-skedpal.html





---
## Applicaties die Json gebruiken

### Youtube
Als je gebruik maakt van de youtube API om met je eigen code een youtube search uit te voeren krijg je een antwoord in de vorm van een JSON bestand. Youtube doet dit waarschijnlijk omdat json zeer efficient is, youtube is een zeer groot platform en krijgen waarschijnlijk veel van dit soort requests binnen op een dag, als zij dit dus zo goed mogelijk kunnen streamlinen door een effiecient format te gebruiken bespaard ze dat al een hoop bandbreedte en servertijd.

### Minecraft
Minecraft gebruikt JSON bijvoorbeeld om tekst van boeken en texture pack informatie op te slaan. Ze hebben waarschijnlijk voor json gekozen omdat dit simpel te gebruiken is. Omdat dit soort informatie snel aangemaakt on opgehaald moet kunnen worden is het handig dat ze JSON gebruiken.

### Twitter
Twitter gebruikt JSON om tweets op te slaan, elke dag worden er ontzettend veel tweets getweet. Deze informatie moet zo efficient mogelijk worden opgeslagen om serverruimte te besparen.

---

