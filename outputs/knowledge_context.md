# Knowledge Context

### Relevantni produkty
- FLEETWARE/FLWW2: prace s vozidly, provoznimi daty, pozicnimi daty a opravnenimi.
- ROAD PLAN: planovani objednanych sluzeb a vykonove prehledy.
- PASPORT: data o nadobach, vysypech a zakaznickych smlouvach.

### Architektura systemu
- Kazdy produkt ma samostatnou SQL DB.
- FLEETWARE je popsany jako zdroj pozicnich dat a udalosti.
- System landscape uvadi dashboard/reporting vrstvu pro agregaci klicovych dat.

### Integrace
- Uvedene integrace: interni REST API mezi moduly.
- Uvedeny principy: cteni dat ze stavajicich systemu a agregace do dashboard modelu.

### Omezeni
- Nutnost vyuzit existujici systemy.
- Omezena kapacita vyvoje.
- Tlak na rychle MVP.

### Terminologie
- FLEETWARE: hlavni aplikace pro pozicni data, udalosti a opravneni.
- ROAD PLAN: modul planovani a vykonovych prehledu.
- PASPORT: system dat o nadobach, vysypech a smlouvach.
- Dashboard model: agregacni vrstva pro centralni prehled.
- MVP: prvni omezena verze reseni s nejvyssi hodnotou.

## Predpoklady
- Predpoklad: Pro MVP bude vyuzit existujici REST API bez zasadni zmeny jadra systemu.
- Predpoklad: Dashboard model bude v MVP prioritne read-only agregacni vrstva.

## Otevrene otazky
- Ktere konkretni API endpointy jsou stabilni a dostupne pro MVP?
- Kdo je owner dat jednotlivych entit napric moduly?
- Jake role a opravneni musi byt pokryty uz v prvni fazi?

## Citace zdroju
- PROJECT_CONTEXT.md
- databank/products/portfolio_overview.md
- databank/business/business_goals.md
- databank/architecture/system_landscape.md
- databank/terminology.md
