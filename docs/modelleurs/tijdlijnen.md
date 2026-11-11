---
title: Tijdlijnen
parent: Modelleurs
---

# Tijdlijnen

Een conceptueel informatiemodel beschrijft de toestand van de wereld op abstract niveau: welke soorten entiteiten er zijn, met welke eigenschappen en relaties. Het model representeert de wereld zoals die bedoeld of waargenomen wordt, maar bevat geen informatie over veranderingen in de tijd, versies of individuele voorkomens.

Toch is tijd vaak wél een essentieel onderdeel van de betekenis van entiteiten. Daarom nemen we in het conceptueel model een expliciete tijdlijnmarkering op. In het logisch model worden deze tijdlijnen vervolgens uitgewerkt in attributen en versiestructuren. We volgen hierbij [NEN 3610](https://www.geonovum.nl/geo-standaarden/nen-3610-basismodel-voor-informatiemodellen) §8.3. Daarin geeft de 'tijdlijn geldigheid' aan wanneer een entiteit in de werkelijke wereld van toestand verandert, onafhankelijk van het moment van registratie. De 'tijdlijn registratie' representeert het moment waarop informatie in een systeem bekend is, en kan verschillen van de feitelijke geldigheid in de werkelijkheid. Omdat we de 'tijdlijn registratie' beschouwen als een generiek implementatiekader voor het hele register, richten we ons bij conceptueel modelleren enkel op de tijdlijn geldigheid.

Een geldigheidstijdlijn is alleen van toepassing op *enduranten*: entiteiten die op meerdere tijdstippen kunnen bestaan en daarbij hun identiteit behouden (zoals een gebouw, aansluiting of tarief). *Perduranten* (zoals gebeurtenissen, metingen of processen) bestaan uit meerdere fasen in de tijd en zijn niet als geheel aanwezig op één moment. Bij perduranten maakt tijd deel uit van de definitie van de entiteit zelf (bijvoorbeeld via `tijdstip`, `begintijd` of `duur`). Een geldigheidstijdlijn kan daarnaast alleen worden toegepast op enduranten met een niet-herbruikbare identificatie, om te voorkomen dat er gaten of 'reïncarnaties' in de tijdlijn ontstaan.

De markering op een entiteit gebeurt als volgt:

- In draw.io: `⏲` achter de entiteitnaam.
- In LinkML: `tijdlijn_geldigheid: true` binnen `annotations`.

Bij een verwijzing naar een entiteit met geldigheidstijdlijn is het van belang of deze verwijzing voor een specifieke versie in de tijd geldt (de toestand). In dat geval markeren we deze relatie als volgt:

- In draw.io: `⏲` voor de relatienaam, maar volgend op een eventueel hekje (`#`).
- In LinkML: `volgt_tijdlijn_geldigheid: true` binnen `annotations`.

Deze tijdslijnmarkeringen in het conceptuele model helpen bij consistente versiemodellering in het gegevensmodel conform NEN 3610:

![Tijdlijnen in een gegevensmodel]({{ site.baseurl }}/assets/images/tijdlijnen.drawio.svg)
