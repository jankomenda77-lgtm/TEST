# Engineering Review

## Technicka proveditelnost
- Navrh je proveditelny, protoze stavi na existujicich systemech a REST integracich.
- Nejvetsi blokator je nekompletni vstup: chybi detailni landscape a API kontrakty.

## Slozitost implementace
- Stredni az vyssi slozitost kvuli orchestraci workflow napric vice produkty.
- Stredni slozitost pro dashboard agregujici data z vice zdroju.
- Vyssi slozitost hrozi pri nejasnem datovem vlastnictvi a rozdilnych modelech entit.

## Rizika
- Riziko chybneho scope MVP bez jasnych prioritnich use-cases.
- Riziko integracnich zpozdeni (nejasne povinne integrace v 1. fazi).
- Riziko nekonzistence dat mezi systemy.
- Riziko provoznich problemu bez definovanych NFR (SLA, monitoring, audit).

## Doporuceni
- Nejdriv potvrdit 1-2 hlavni MVP use-cases a primarni roli uzivatele.
- Sepsat minimalni integracni kontrakt pro MVP (endpointy, chyby, latence).
- Zavest jednoduche mapovani datovych entit a source-of-truth tabulku.
- Dodavat iterativne: nejdriv unified UI + 1 dashboard view + minimum automatizace.

## Otevrene otazky
- Ktere integrace jsou absolutne nutne pro prvni release?
- Jake jsou meritelne vykonnostni cile dashboardu?
- Jaka je cilova observabilita (logy, metriky, tracing)?

## Zdroje
- outputs/architecture_draft.md
- outputs/requirements_draft.md
