---
title: Begripsverwijzingen
parent: Modelleurs
---

# Begripsverwijzingen

Registermodellen verwijzen naar het [begrippenkader](https://begrippen.netbeheernederland.nl) om aan te sluiten bij de gedeelde sectortaal en om het eigenaarschap traceerbaar te maken.

We maken onderscheid tussen het doel van het registermodel als geheel en de betekenis van losse onderdelen:

## Het model als geheel

Koppel het registermodel als geheel via `related_mappings` in de root van het LinkML-schema. Hiermee leg je het hoofdonderwerp van het register vast. We gebruiken `related_mappings` (en geen `exact_mappings`) omdat het model geen synoniem is van het begrip, maar een manier van kijken naar de wereld die helpt om het bedrijfsdoel te bereiken dat impliciet met dat begrip samenhangt.

## De elementen van het model

Op het niveau van entiteiten, eigenschappen en waardelijsten:

**Wel opnemen:**

* **Exacte semantische match** (`exact_mappings`): wanneer er in het begrippenkader een begrip bestaat dat exact dezelfde betekenis dekt.
* **Afwijkend domein** (`broad_mappings` of `related_mappings`): als een entiteit (zonder exacte match) onder een ander begrip valt dan het register als geheel.

**Niet opnemen:**

* **Herhaling van het registerbegrip**: herhaal de verwijzing van het registerniveau niet op afzonderlijke entiteiten, tenzij het om een exacte match (`exact_mappings`) gaat.
* **Ondergeschikte entiteiten**: entiteiten die puur dienen ter detaillering, indeling of specialisatie krijgen geen eigen verwijzing, tenzij er een exacte match bestaat.
