---
description: Inventar al termenelor fiscale — ce e depășit, ce e scadent, ce urmează
argument-hint: "[luna|an|nume dosar]  (gol = toate dosarele, starea de azi)"
allowed-tools: Read, Glob, Grep, Bash, Task
---

Fă un audit de termene pentru: **$ARGUMENTS** (dacă e gol: toate dosarele, la data de azi).

1. Invocă skill-ul `stb-kanzlei` și citește `references/fristenkalender.md`.
2. Citește `mandanten/index.md` și fiecare `AKTE.md`.
3. Data de azi: !`date +%F`
4. Aplică § 108 Abs. 3 AO la fiecare termen calculat (weekend/sărbătoare în Niedersachsen → următoarea zi lucrătoare).
5. Produ raportul: 🔴 depășite · 🟠 ≤ 14 zile · 🟡 ≤ 60 zile · ⚪ status necunoscut.
6. Estimează expunerea la § 152 AO pentru fiecare termen depășit, marcând-o explicit ca estimare.
7. Termină cu acțiunile recomandate, în ordinea urgenței.

Nu transmite nimic nicăieri. Nu presupune că o obligație e îndeplinită dacă fișa nu o confirmă.
