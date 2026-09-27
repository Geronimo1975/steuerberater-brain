---
description: Verifică situația de TVA a unui dosar — ritm, praguri, Kleinunternehmer, termene
argument-hint: "<nume dosar>  [an]"
allowed-tools: Read, Glob, Grep, Bash, Task
---

Verifică situația Umsatzsteuer pentru: **$ARGUMENTS**

1. Invocă skill-ul `stb-umsatzsteuer`.
2. Citește `AKTE.md` al dosarului.
3. Verifică, pe rând:
   - Statut: Kleinunternehmer § 19 UStG sau Regelbesteuerung? Pragurile 25.000 / 100.000 € respectate?
   - Ritmul UStVA corect pentru anul curent (pe baza Zahllast anului precedent: praguri 9.000 / 2.000 €)?
   - Dauerfristverlängerung activă? Sondervorauszahlung plătită până 10.02?
   - Operațiuni intracomunitare → ZM depusă? USt-IdNr. verificate?
   - Vânzări B2C în UE peste 10.000 € → OSS necesar?
   - § 13b UStG aplicat corect?
   - eRechnung: capacitatea de recepție asigurată (obligatorie din 01.01.2025)?
   - **Dacă activitatea e oprită**: semnalul USt e dezactivat la FA? Altfel sunt datorate Nullmeldungen. Evaluează § 3 Abs. 1b și § 15a UStG.
4. Marchează cu ⚠️ orice prag pe care nu îl poți confirma pentru anul în cauză și verifică-l live.
5. Listează termenele USt deschise și declarațiile lipsă.
