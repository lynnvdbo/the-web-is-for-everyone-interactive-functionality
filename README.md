# Interactive Functionality

Ontwerp en maak voor een opdrachtgever een interactieve toepassing die voor iedereen toegankelijk is

# Bloemenveld Frankendael - Webapp
Het Bloemenveld in Park Frankendael is een bijzondere plek in het park, waar veel groeit en leeft. Toch blijft de waarde van het veld voor veel voorbijgangers verborgen. Wat er groeit, bloeit en leeft, is niet altijd zichtbaar of makkelijk te begrijpen. Terwijl juist dit soort plekken een grote rol spelen in het versterken van stedelijke natuur en het vergroten van het bewustzijn rondom een duurzame leefomgeving. Daarom is er een duidelijke behoefte aan manieren om bewoners van Amsterdam Oost (Watergraafsmeer) op een laagdrempelige manier kennis te laten maken met de natuur dichtbij huis. Een ervaring die verder gaat dan alleen kijken en waarin bezoekers actief kunnen ontdekken, beleven en leren wat er in hun omgeving leeft.

#### Vraag van de opdrachtgever
Ontwerp en ontwikkel een webapp met een interactieve veldverkenner waarbij bezoekers in verschillende zones van de Bloementuin aan de hand van opdrachten planten en bloemen kunnen ontdekken. Bij het goed maken van de opdrachten kunnen badges worden verdiend

Check [hier](https://server-side-rendering-server-side-website-qfhx.onrender.com/) de website.

## Inhoudsopgave Readme

  * [Beschrijving](#beschrijving)
  * [Huisstijl](#huisstijl)
  * [Responsive](#responsive)
  * [Kenmerken](#kenmerken)
  * [Installatie](#installatie)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
<!-- In de Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->
Voor de opdrachtgever maken wij een website wat eigenlijk een webapp is. Het is de bedoeling dat de bezoeker een QR code kan scannen en dan vervolgens op de webapp komt. Er is dan een veldverkenner die je laat zien waar je op dat moment bevindt in het bloemenveld en dan kan je zelf op verschillende zones drukken in de app. Vervolgens krijg je een opdracht en infformatie over de de debetreffende plant.

De afgelopen weken heb ik mij gefocust op een interactieve toepassing die voor iedereen toegankelijk is. We hebben deze sprint vooraal geleerd hoe je data naar Directus kan POSTen met behup van een formulier.

### Comment plaatsen

De interactie die ik heb gemaakt is dat de gebruiker een comment kan achterlaten op een nieuwsartikel. Om dit te laten werken heb ik gebruik gemaakt van een POST.
Als gebruiker kan je ook zien hoeveel berichten er zijn verstuurd. Dit is feedforward, omdat je de gebruker laat weten hoeveel berichten hij/zij kan verwachten. Daarnaast heb ik ook een empty state, dus zodra er nog geen berichten zijn versuurd komt 'Er zijn nog geen berichten voor dit artikel' te staan.

Ik heb ook nog een kleine animaie toegevoegd aan het berichtje die de gebruiker net heeft verstuurd. Er komt namelijk een zwarte border om je bericht heen zodat de gebruiker duidelijk kan zien waar zijn berichtje is geplaatst en een paar seconde later verdwijnt de border weer.

https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/4164811805140ce2526fdada9d5f864f40f07a54/server.js#L154-L180

<img width="160" height="650" alt="mobile-black(3)" src="https://github.com/user-attachments/assets/eb0c7d28-729f-4b1f-aaca-8e4a90c830cf" />

<img width="160" height="650" alt="mobile-black" src="https://github.com/user-attachments/assets/8eca9e50-9c77-49e4-b174-9866a5990cdd" />

<img width="160" height="650" alt="mobile-black kopie 2" src="https://github.com/user-attachments/assets/ab0db54d-da9f-4e41-a23b-cc3f51688503" />

https://github.com/user-attachments/assets/a2ade118-df71-42ce-8d40-5097aaeeda31

### Comment deleten

Na het plaatsen van een comment is er ook een mogelijkheid om een comment te verwijderen. Hiervoor heb ik ook gebruik gemaakt van een POST
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/4164811805140ce2526fdada9d5f864f40f07a54/server.js#L182-L193

https://github.com/user-attachments/assets/59ccb1a8-8f6e-4549-b7dd-dbb2893492e6

### Active state

In heb ook active states toegevoegd op de filters bij het nieuws en in de navigatie zodat de gebruiker weet waar hij/zij zicht bevindt. Ik heb bij de filters gekozen voor een zwarte border om het duidelijk te laten zien aan de gebruiker. Voor de navigatie heb ik ervoor gekozen om het subtiel te houden, dus zit er een streepje onder het desbetreffende pagina. Ook heb ik op de homepage alle nieuwsartikelen geplaatst met een scroll.

HTML
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/d467b780fcfe87ef766edd0888f2cf9139949493/views/nieuws.liquid#L14-L16
CSS
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/d467b780fcfe87ef766edd0888f2cf9139949493/public/style.css#L304-L322
server.JS
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/d467b780fcfe87ef766edd0888f2cf9139949493/server.js#L91-L95

<img width="160" height="650" alt="mobile-black kopie" src="https://github.com/user-attachments/assets/151d772d-0809-4116-8cf2-8ceca46cd002" />

<img width="160" height="650" alt="mobile-black(1)" src="https://github.com/user-attachments/assets/068ec21e-9635-4021-8c82-3709ac6073eb" />

<img width="160" height="650" alt="mobile-black(2)" src="https://github.com/user-attachments/assets/fbf7ae12-5e26-4a36-a2a5-c88a937a001f" />

<img width="392" height="89" alt="Scherm­afbeelding 2026-04-02 om 22 27 31" src="https://github.com/user-attachments/assets/7cb5c74e-e259-4fa3-b048-66203f8932f8" />

https://github.com/user-attachments/assets/0dfec0d1-dfa7-47a6-9f94-fd9bf0631ea6

## Huisstijl
Van de opdrachtgever hebben wij een prototype gekregen van het design in een [figma bestand](https://www.figma.com/design/9UctVXSWnspKX72xtLvNQ5/Prototype-Bloemenveld?node-id=0-1&p=f&t=qHEk4ifRm1wbrbWr-0) Op basis van dat prototype design ben ik mijn website gaan maken. Ik heb dezelfde kleuren, afbeeldingen, fonts etc gebruikt en toegepast op de website.

## Responsive
<!-- In de Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->
Doordat de website een webapp is, is het niet noodzakelijk om een ipad of desktop versie te maken. Waarschijnlijk gebruiken de meeste bezoekers hun telefoon om de QR code te scannen. Het is ook ontworpen met de intensie voor een telefoon. Tijdens de sprintreview hebben we het er wel over responsive gehad en er is toen gezegd dat ipad versie nog wel handig zou kunnen zijn en desktop nu niet een prioriteit. Dit geldt voornamelijk voor de veldverkenner. Nieuws en collectie zouden wel sowieso handgin zijn voor als bezoekers nog eens het nieuws willen bekijken of zijn/haar collectie.

<!--Bij Gebruik staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->
De website is gebouwd met HTML, CSS en JS, NodeJS, Express, JSON en Liquid

###  @media (prefers-reduced-motion:no-preference)

In mijn CSS code maak ik gebruik @media (prefers-reduced-motion:no-preference).
Dit zrogt ervoor dat de mensen die minder beweging hebben ingesteld geen amimaties te zijn krijgt.
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/a59dec1848139960f125f7d8a4a389aff6e6ca10/public/style.css#L726-L732

In het filmpje hierboven bij een comment plaatsen zie je de animatie dat er een zwarte border om je bericht komt als je hem hebt geplaatst en dat hij na een paar secondes weg gaat. Als iemand geen animatie wil dan krijgt verdwijnt de border niet en blijf hij staan.

https://github.com/user-attachments/assets/a8c9ab25-02d9-4db6-b64b-6495bfa32dd3

### Liquid filters

Ik heb ook gebruik gemaakt van liquid filters

truncate: 20 -> zorgt ervoor dat de laatste 3 letters van de 20 ... worden 
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/d467b780fcfe87ef766edd0888f2cf9139949493/views/artikel.liquid#L46

date: '%d-%m-%Y %H:%M -> zorgt dat de meest recente berichtje boveaan staat
https://github.com/lynnvdbo/the-web-is-for-everyone-interactive-functionality/blob/d467b780fcfe87ef766edd0888f2cf9139949493/views/artikel.liquid#L53

## Installatie
<!-- Bij Instalatie staat hoe een andere developer aan jouw repo kan werken -->
1. Clone als eerst deze repository
2. Open hem in VSCodium of een code editor
3. Open dan de terminal en type npm install
4. Start vervolgens de website door npm start in te typen

## Bronnen
[Figm bestand prototpye](https://www.figma.com/design/9UctVXSWnspKX72xtLvNQ5/Prototype-Bloemenveld?node-id=0-1&p=f&t=qHEk4ifRm1wbrbWr-0)

https://liquidjs.com/filters/overview.html

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).









