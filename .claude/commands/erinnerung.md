---
description: Procesează o scrisoare de la Finanzamt (Erinnerung, Bescheid, Androhung) și propune reacția
argument-hint: "<cale către PDF sau nume dosar>"
allowed-tools: Read, Write, Edit, Glob, Grep, Bash, Task
---

Procesează documentul de la Finanzamt: **$ARGUMENTS**

1. Invocă skill-ul `stb-kanzlei` → `references/erinnerung-schaetzung.md`.
2. Extrage datele din document (dacă e scan fără text, citește-l vizual cu Read + `pages`):
   Steuernummer, IdNr., data scrisorii, Steuerart, VZ, termenul cerut, declarațiile lipsă.
3. Data de azi: !`date +%F`
4. Stabilește:
   - Există obligație legală de depunere? Pe ce temei?
   - Termenul legal (§ 149 Abs. 2 vs. Abs. 3 AO) era deja expirat?
   - Ce expunere la § 152 AO rezultă (0,25 %/lună, min. 25 €/lună, max. 25.000 €)?
   - Riscul de § 162 AO Schätzung.
5. Recomandă una dintre căi: depunere imediată · `Antrag auf Fristverlängerung` § 109 AO · clarificare scrisă.
6. Dacă se impune un Antrag, redactează-l complet, gata de semnat, pe baza șablonului din referință.
7. Actualizează `AKTE.md` al dosarului la secțiunea „Fristen & Status".

Nu trimite nimic la Finanzamt sau ELSTER. Pregătești; utilizatorul semnează și trimite.
