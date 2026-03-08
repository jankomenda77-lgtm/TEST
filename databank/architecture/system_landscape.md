# System Landscape

## Hlavní systémy
- FLEETWARE: hlavní produktová aplikace pro práci s vozidly, uživateli a provozními daty
- ROAD PLAN: modul pro plánování a výkonové přehledy
- PASPORT: systém pro data o nadobách, výsypech a zákaznických smlouvách
- Dashboard / reporting vrstva: agreguje klíčová data pro centrální pohled

## Integrace
- interní REST API mezi moduly
- čtení dat ze stávajících systémů
- agregace dat do dashboard modelu

## Datové toky
- uživatel pracuje v UI
- orchestrace volá existující systémy přes API
- data jsou agregována do centrálního dashboard pohledu

## Omezení
- nutnost využít existující systémy
- omezená kapacita vývoje
- tlak na rychlé MVP