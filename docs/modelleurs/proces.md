---
title: Proces
parent: Modelleurs
---

# Proces

![Proces]({{ site.baseurl }}/assets/images/proces.drawio.svg)

## Opmerkingen per stap

* **Voer desk research uit**. Dit houdt in:
  * Inlezen op bestaande modellen en relevante regelgeving en standaarden
  * Eerste vragen aan domeinexperts voorbereiden

* **Dien usecase in en verfijn**: Productmanager levert waar mogelijk aan:
  * waarde en noodzaak van de usecase
  * contactgegevens van domeinexperts
  * gewenste opleverdatum

* **Maak en review model**: Er moet minimaal een peerreview zijn geweest binnen Team Semantiek voordat het model ter beoordeling wordt voorgelegd aan anderen.

* **Publiceer model**: Zodra de productmanager het model bouwklaar acht, wordt deze gepubliceerd. De beoordelingen door data-eigenaren mogen eventueel parallel plaatsvinden (op risico van de productmanager) en worden achteraf vermeld bij het model (zonder persoonsnaam).

* **Beoordeel model**: De data-eigenaren worden per netbeheerder benoemd door de betreffende Chief Data Officer (CDO) en zijn vindbaar via het Data Office of vergelijkbare afdeling. Team Semantiek kan faciliteren bij de communicatie met data-eigenaren.

## Versies

Versioneringspatroon `major`.`minor`:

* `major`: verhoog bij wijzigingen waardoor bestaande data niet eenduidig naar het nieuwe model kan worden gemigreerd, zoals een nieuwe verplichte eigenschap zonder duidelijke standaardwaarde.
* `minor`: verhoog bij alle andere wijzigingen met impact op de data.

De `patch` kennen wij dus niet: wijzigingen zonder impact op data leiden niet tot een nieuwe versie.

## E-mail om data-eigenaren te betrekken

> _Onderwerp: Betrokkenheid gezamenlijk model `[naam register]`_
>
> Beste `[naam]`,
>
> Onder de `[relevante wet- of regelgeving of sectorafspraken]` worden we als netbeheerders verantwoordelijk voor `(een nieuwe versie van)` het `[naam register]`. `[Naam epic owner/productmanager]` begeleidt als centrale `[epic owner/productmanager]` de realisatie hiervan.
>
> Voordat we gegevens uitwisselen, leggen we als netbeheerders eerst de gezamenlijke betekenis ervan vast. Dat doen we onder begeleiding van Team Semantiek (Netbeheer Nederland), zodat alle registers samen één consistent en uitlegbaar stelsel vormen ([bekijk hier waarom en hoe we dat doen](https://modellen.netbeheernederland.nl/stelsel/waarom)). Dit gebeurt onder mandaat van de CDO's van de netbeheerders.
>
>Via `[naam Data Office / CDO / collega]` begrepen wij dat jij binnen `[naam netbeheerder]` het juiste aanspreekpunt (data-eigenaar) bent voor de inhoudelijke betekenis van de gegevens in dit register. Een eerste conceptversie van het model vind je hier: `[URL naar registermodel]`.
>
> **Wat we nu van je vragen (graag uiterlijk `[datum]`)**:
>
> 1. **Eigenaarschap bevestigen**: Klopt het dat jij namens `[naam netbeheerder]` het aanspreekpunt bent voor dit registermodel? Zo niet, zou je deze e-mail willen doorsturen naar (of ons in contact brengen met) de juiste collega?
> 2. **Inhoudelijke experts aandragen**: Welke domeinexperts vanuit `[naam netbeheerder]` mogen wij betrekken voor inhoudelijke input en review bij de verdere uitwerking? (De verwachte tijdsinvestering is ongeveer 1 uur per week in de periode `[periode]`.)
>
> **Vervolg**:  
> Wanneer het model door de sector en Team Semantiek is gereviewd (`[verwachte periode]`), vragen wij jou als data-eigenaar om formele goedkeuring. Die goedkeuring vermelden we (zonder persoonsnaam) onder de modelpagina, zodat de status voor iedere organisatie helder is.
>
> Alvast hartelijk dank voor je reactie!  
> Met vriendelijke groet,  
> Namens Team Semantiek,  
> `[Naam afzender]`  
> `[Functie en organisatie]`

## E-mail voor formele goedkeuring

> _Onderwerp: Verzoek om goedkeuring: model van `[naam register]` (versie `[X.Y]`)_
>
> Beste `[naam]`,
>
> Het gezamenlijke model voor het `[naam register]` (versie `[X.Y]`) is gereed voor goedkeuring door de data-eigenaren. Graag vragen wij jouw akkoord namens `[naam netbeheerder]`.
>
> **Totstandkoming**
>
> * **Link naar het model**: `[URL naar specifieke versie]` _(Geen ervaring met het lezen van informatiemodellen? Onder het diagram staan alle begrippen en eigenschappen in gewoon Nederlands uitgelegd. Voor de symbolen in het diagram kun je de [Legenda](https://modellen.netbeheernederland.nl/stelsel/legenda) raadplegen.)_
> * **Inhoudelijke input**: Dit model is opgesteld op basis van `[relevante wetgeving / marktcodes / standaarden]` en tot stand gekomen met inbreng van domeinexperts uit de sector (namens `[naam netbeheerder]` waren `[namen experts]` betrokken) en een peerreview binnen Team Semantiek.
> * **Aandachtspunten**:
>   * `[een paar korte bullets over gemaakte keuzes]`
>
> **Waar geef je precies akkoord op?**  
> Jouw goedkeuring geldt voor de _betekenis_ (de definities van entiteiten, eigenschappen, relaties en waardelijsten als gedeeld sectorbegrip). Het model schrijft niet voor hoe systemen intern worden ingericht.
>
> **Zichtbaarheid op de website**  
> Na jouw akkoord vermelden we de goedkeuring onderaan de modelpagina in het goedkeuringsoverzicht:
>
> * **Bronhouder**: `[naam netbeheerder]`
> * **Vertegenwoordigd door**: jouw functie en afdeling
> * **Datum**: datum van goedkeuring
>
> **Wat we van je vragen (graag uiterlijk `[datum]`)**:
>
> 1. Kun je per reply op deze e-mail met CC naar teamsemantiek@netbeheernederland.nl bevestigen dat je akkoord bent met versie `[X.Y]` van het `[naam register]`? (Eventuele opmerkingen of wijzigingsverzoeken kun je daarbij uiteraard ook doorgeven. Kleine opmerkingen nemen we mee in een volgende versie. Bij eventuele blokkerende bezwaren stemmen we die eerst met je af.)
> 2. Wil je bij je akkoord aangeven welke exacte functie en afdeling we namens `[naam netbeheerder]` bij de goedkeuring mogen vermelden?
>
> **Vragen of behoefte aan een korte toelichting?**  
> We lopen het model graag samen met je door. Laat het gerust weten als je daar behoefte aan hebt, dan plannen we iets in.
>
> Alvast hartelijk dank voor de samenwerking!
>
> Met vriendelijke groet,  
> Namens Team Semantiek,  
> `[Naam afzender]`  
> `[Functie en organisatie]`
