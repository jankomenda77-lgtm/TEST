# Engineering Review

### Technicka proveditelnost
- Navrh je proveditelny jako MVP, pokud zustane omezenej na nadstavbovy pristup nad existujicimi systemy.
- Nejvetsi nejistoty jsou v integracnich detailech a neuzavrenem scope.

### Slozitost implementace
- Integracni vrstva: stredni slozitost (vice systemu, odlisna data).
- Unified UI + orchestrace: stredni az vyssi slozitost podle poctu scenaru v MVP.
- Dashboard agregace: stredni slozitost, citliva na kvalitu zdrojovych dat.

### Rizika
- Integracni riziko: nejasne povinne integrace a neoverene kontrakty.
- Datove riziko: nejasny source of truth.
- Scope riziko: tlak na rychly release muze zvetsit MVP nad realnou kapacitu.
- Provozni riziko: chybi konkretni NFR metriky a akceptacni limity.

### Doporuceni
- Omezit MVP na 1 hlavni use-case, 1 dashboard pohled a 1 priorizovanou automatizaci.
- Pred implementaci potvrdit API kontrakty povinnych integraci.
- Definovat source-of-truth mapu pro MVP entity.
- Zavest minimalni NFR baseline (latence, dostupnost, chybovost).

## Predpoklady
- Predpoklad: Tym dokaze realizovat MVP inkrementalne bez rozsahleho refaktoringu legacy systemu.

## Otevrene otazky
- Ktery use-case bude implementovan jako prvni?
- Jaka je pozadovana latence dashboardu pro MVP?
- Kdo je odpovedny za schvaleni integracnich kontraktu?

## Zdroje
- outputs/architecture_draft.md
- outputs/requirements_draft.md
