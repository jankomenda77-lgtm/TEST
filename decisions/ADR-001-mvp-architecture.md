# ADR-001 MVP Architecture

## Kontext

Cílem je vytvořit jednotné UI a dashboard nad existujícími systémy:
- FLEETWARE
- ROAD PLAN
- PASPORT

Bez nahrazení těchto systémů.

## Primary Use Case

Operátor potřebuje v jednom pohledu vidět:

- aktuální stav vozidel
- plán tras
- stav výsypů / nádob

## Source of Truth

FLEETWARE → vozidla a události  
ROAD PLAN → plánování  
PASPORT → data o nádobách a smlouvách  

## Architektonický styl

MVP bude použivat:

Unified UI  
↓  
BFF / orchestration layer  
↓  
REST API integrace  
↓  
Existing systems

## Dashboard model

Dashboard bude read model:

- agregovaný pohled
- optimalizovaný pro dotazy
- není systém evidence

## Architektonické principy

- source of truth zůstává ve stávajících systémech
- orchestration vrstva zůstane tenká
- MVP preferuje read operace
- scope MVP je omezen na jeden hlavní use-case
