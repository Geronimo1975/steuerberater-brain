---
description: Deschide un dosar nou, cu fișă completă și lista obligațiilor aplicabile
argument-hint: "<nume>  [formă juridică]  [data începerii activității]"
allowed-tools: Read, Write, Edit, Glob, Bash, Task
---

Deschide un dosar nou pentru: **$ARGUMENTS**

1. Invocă skill-ul `stb-mandant-onboarding`.
2. Întreabă doar ce nu poți deduce: formă juridică, activitate, data începerii, statut USt (Kleinunternehmer § 19 sau Regelbesteuerung), angajați, operațiuni transfrontaliere.
3. Creează `mandanten/<Nume>/AKTE.md` pornind de la `mandanten/_TEMPLATE/AKTE.md`.
4. Completează lista obligațiilor recurente aplicabile, derivată din forma juridică și statutul USt (vezi `stb-kanzlei/references/fristenkalender.md`).
5. Adaugă rândul corespunzător în `mandanten/index.md`.
6. Produ checklist-ul de onboarding: Fragebogen § 138 AO, Gewerbeanmeldung, Vollmacht + VDB, KYC GwG, Transparenzregister, BG, Betriebsnummer — după caz.
7. Semnalează termenele declanșate de dată (ex. Fragebogen § 138 AO: 1 lună de la începerea activității).
