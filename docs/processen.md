# Bedrijfsprocessen: Werkgevers ↔ Verzekeraars

Dit document beschrijft de interacties tussen werkgevers en inkomensverzekeraars voor dekking, premie en schadeclaims.

---

## 1. Polisdekking & Werknemersbestand
* **Trigger:** Aanvang verzekeringsjaar, wijziging van de collectieve polis of mutaties in de werknemerspopulatie.
* **Actie werkgever:** Aanlevering van `PolisdekkingAanmelding` met actuele BSN/identificatienummers en de geldende loongegevens.
* **Actie verzekeraar:** Toetsing aan de acceptatievoorwaarden en vaststelling van de actuele dekkingsgraad.

## 2. Verzuimclaim Loondoorbetaling
* **Trigger:** Een werknemer overschrijdt het overeengekomen eigen risico (bijvoorbeeld wachttijd van 10, 30 of 60 dagen).
* **Actie werkgever:** Verzending van `VerzuimClaim` met opgave van het verzuimperpercentage en historische loongegevens voor de dagloonberekening.
* **Actie verzekeraar:** Toetsing van de polisvoorwaarden en reservering van het uitkeringsbedrag.

## 3. Periodieke Declaratie & Uitkering
* **Trigger:** Maandelijkse verwerking van het doorbetaalde loon tijdens ziekte.
* **Actie:** Afstemming tussen de geclaimde loonkosten en de overeengekomen dekkingspercentages (bijv. 70% of 100% loonwaarde).
