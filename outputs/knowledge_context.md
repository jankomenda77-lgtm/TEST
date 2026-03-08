# Knowledge Context

## Relevantni produkty
- FLEETWARE (FLWW2): evidence vozidel, telemetrie, poloha, ridic, prava uzivatelu i pristupy do dalsich systemu.
- ROAD PLAN (RP): evidence smluv a objednanych sluzeb, planovani denniho vykonu na vozidla, vyhodnoceni vykonu.
- PASPORT: evidence nadob, vysypu, terminu, zakazniku a smluv.

## Architektura systemu
- Podle PROJECT_CONTEXT vznikaji pozicni data a udalosti ve FLEETWARE.
- Uvedeno je, ze kazdy produkt ma samostatnou SQL DB.
- Vstup `databank/architecture/system_landscape.md` je prazdny (0 B), detailni landscape chybi.

## Integrace
- Explicitne uvedeno REST API.
- Integracni body mezi moduly nejsou detailne popsane.

## Omezeni
- Omezena kapacita vyvoje.
- Nutnost vyuzit stavajici systemy.
- Tlak na rychle MVP.

## Terminologie
- MVP: prvni realizovatelna verze s minimalnim rozsahem.
- Dashboard: prehled stavu dat/procesu v jednom rozhrani.
- Integrace: propojeni na existujici produkty (FLEETWARE, ROAD PLAN, PASPORT).

## Otevrene otazky
- Jaky je aktualni system landscape a vlastnictvi rozhrani?
- Ktere API endpointy jsou k dispozici a v jake kvalite (SLA, limity)?
- Ktera domanova data budou v MVP zdrojem pravdy?

## Zdroje
- PROJECT_CONTEXT.md
- databank/products/portfolio_overview.md
- databank/business/business_goals.md
- databank/architecture/system_landscape.md
- inputs/meeting_transcript.md
