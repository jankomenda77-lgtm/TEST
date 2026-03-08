# Architecture Draft

### Prehled architektury
MVP-oriented navrh pocita s lehkou orchestration a dashboard vrstvou nad existujicimi systemy FLEETWARE, ROAD PLAN a PASPORT. Cilem je dodat jednotne UI a centralni datovy pohled bez nahrady stavajicich aplikaci.

### Hlavni komponenty
- Unified UI pro hlavni uzivatelsky scenar.
- Orchestration vrstva pro volani API a rizeni procesu.
- Integracni konektory na FLEETWARE, ROAD PLAN, PASPORT.
- Dashboard model pro agregovany read pohled.

### Integrace
- Primarni integracni mechanizmus: interni REST API.
- Integrace vyuziji cteni a kombinaci dat ze stavajicich systemu.
- MVP ma zahrnout jen povinne integrace pro prvni use-case.

### Datove toky
- Uzivatel -> Unified UI -> orchestration -> REST API -> stavajici systemy -> odpoved do UI.
- Data ze stavajicich systemu -> agregace -> dashboard model -> centralni dashboard.

### Technicka rizika
- Chybi detailni API kontrakty a provozni limity.
- Nejasny source-of-truth model mezi produkty.
- Riziko scope creep pod tlakem rychleho MVP.
- Riziko nekonzistence agregovanych dat pri odlisnych datovych modelech.

## Predpoklady
- Predpoklad: Stavajici API budou pro MVP funkcne dostatecna.
- Predpoklad: V prvni fazi nebude potreba full real-time synchronizace vsech dat.

## Otevrene otazky
- Jaka je cilova frekvence aktualizace dashboardu?
- Ktera identita/prava se budou pouzivat v jednotnem UI?
- Ktery system je source of truth pro kazdou klicovou entitu?

## Zdroje
- outputs/requirements_draft.md
- outputs/knowledge_context.md
