# Architecture Draft

## Prehled architektury
Navrh je orientovan na lehkou orchestracni vrstvu nad existujicimi produkty (FLEETWARE, ROAD PLAN, PASPORT), aby bylo mozne dorucit jednotne UI, dashboard a postupnou automatizaci bez nahrazovani stavajicich systemu.

## Hlavni komponenty
- Unified UI: jednotne rozhrani pro hlavni workflow.
- Workflow/Orchestration layer: ridi kroky procesu napric systemy.
- Integration layer (REST): vola existujici API stavajicich produktu.
- Read model pro dashboard: agreguje klicova data pro centralni pohled.

## Integrace
- FLEETWARE: zdroj pozicnich dat/udalosti a prav uzivatelu (podle kontextu).
- ROAD PLAN: planovani a vykony.
- PASPORT: data o nadobach, vysypech, zakaznicich/smlouvach.
- Protokol: REST API (jedine explicitne potvrzene rozhrani).

## Datove toky
- Tok 1: UI -> orchestrace -> REST volani do stavajicich systemu -> odpoved do UI.
- Tok 2: Data ze stavajicich systemu -> agregace do dashboard read modelu -> dashboard.
- Tok 3: Uzivatelske akce v UI -> orchestrace automatizovanych rutin -> zapis/vyvolani ve zdrojovych systemech.

## Technicka rizika
- Chybi detailni system landscape a kontrakty API.
- Nejasne vlastnictvi dat a "source of truth" mezi produkty.
- Riziko scope creep kvuli tlaku na rychle MVP.
- Riziko vykonnosti dashboardu pri agregaci dat z vice systemu.

## Otevrene otazky
- Jaky je cilovy autentizacni/autorizacni model napric systemy?
- Ktere endpointy jsou stabilni a podporovane pro MVP?
- Ma byt dashboard near-real-time, nebo periodicky refresh?
- Kde bude provozovana orchestrace (stavajici stack vs. nova sluzba)?

## Zdroje
- outputs/requirements_draft.md
- outputs/knowledge_context.md
