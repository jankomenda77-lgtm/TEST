# Delivery Plan

### MVP scope
- 1 primarni use-case v jednotnem UI.
- Povinne integrace na existujici systemy pro tento use-case.
- 1 centralni dashboard pohled nad prioritnimi daty.
- 1 priorizovana automatizace rutinni cinnosti.

### Faze implementace
- Faze 1: Scope alignment (uzivatel, use-case, povinne integrace, prioritni data).
- Faze 2: API/datove kontrakty + technicky navrh MVP.
- Faze 3: Implementace unified UI + orchestrace + dashboard MVP.
- Faze 4: Integracni testy, pilotni nasazeni, vyhodnoceni MVP metrik.

### Zavislosti
- Dostupnost owneru API pro rychle potvrzeni kontraktu.
- Potvrzeni source-of-truth pro MVP entity.
- Potvrzeni role/prava v jednotnem UI.

### Rizika delivery
- Zpozdeni kvuli nejasnym integracnim kontraktum.
- Riziko rozsahoveho pretizeni MVP.
- Riziko nekonzistentnich dat v dashboardu pri nejasnem vlastnictvi dat.

### Doporuceny dalsi krok
- Usporat kratky decision workshop a formalne uzavrit:
  - primarniho uzivatele,
  - MVP use-case,
  - povinne integrace,
  - prioritni dashboard data.

## Predpoklady
- Predpoklad: Dodavka probiha inkrementalne v malych releasovych davkach.

## Otevrene otazky
- Jaky je cilovy termin pilotu?
- Kdo schvaluje zmeny scope mezi fazemi?
- Jake minimalni metriky uspechu budou sledovany po pilotu?

## Zdroje
- outputs/synthesis.md
- outputs/architecture_draft.md
- outputs/engineering_review.md
