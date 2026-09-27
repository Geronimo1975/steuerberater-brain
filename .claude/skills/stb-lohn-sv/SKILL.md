---
name: stb-lohn-sv
description: Salarizare și asigurări sociale în Germania — Lohnsteuer-Anmeldung §41a EStG, Lohnsteuerbescheinigung, ELStAM, contribuții SV și Beitragsnachweis, DEÜV-Meldungen, Minijob și Midijob, Mindestlohn, Berufsgenossenschaft, Künstlersozialabgabe, Ausgleichsabgabe Schwerbehinderte, A1-Bescheinigung la detașări. Folosește la orice întrebare despre angajați, salarii, contribuții sociale, minijob sau raportări de personal.
---

# Lohn & Sozialversicherung

`Stand: 2026-09-25` · ⚠️ = de verificat live (valorile SV se schimbă **în fiecare an**).

## Triaj

| Situație | Mergi la |
|---|---|
| Lohnsteuer-Anmeldung, ELStAM, Lohnsteuerbescheinigung, Pauschalierung | `references/lohnsteuer.md` |
| Contribuții SV, Beitragsnachweis, DEÜV, Minijob/Midijob, Rechengrößen | `references/sozialversicherung.md` |
| Berufsgenossenschaft, KSK, Schwerbehinderte, A1, Mindestlohn | `references/sondermeldungen.md` |

## Ritmul de bază

| Obligație | Termen | Temei |
|---|---|---|
| Lohnsteuer-Anmeldung | ziua 10 după perioadă | § 41a Abs. 1 EStG |
| SV-Beitragsnachweis | a 5-a ultimă zi lucrătoare a lunii | § 28f Abs. 3 SGB IV |
| **Fälligkeit** contribuții SV | a **3-a** ultimă zi lucrătoare a lunii | § 23 Abs. 1 SGB IV |
| DEÜV-Jahresmeldung | 15.02 | § 10 DEÜV |
| Lohnnachweis Berufsgenossenschaft | 16.02 | § 165 SGB VII |
| Lohnsteuerbescheinigung | 28./29.02 | § 41b Abs. 1 EStG |
| Künstlersozialabgabe | 31.03 | § 27 KSVG |
| Ausgleichsabgabe Schwerbehinderte | 31.03 | § 163 SGB IX |

> Contribuțiile SV **nu** beneficiază de Zahlungsschonfrist. Întârzierea produce imediat Säumniszuschläge de **1 %/lună** (§ 24 SGB IV) — și, în cazuri grave, răspundere penală pentru administrator (§ 266a StGB).

## Înainte de prima angajare

- [ ] **Betriebsnummer** de la Bundesagentur für Arbeit (§ 28a Abs. 3 SGB IV)
- [ ] Înregistrare la **Berufsgenossenschaft** competentă — în 1 săptămână de la începerea activității (§ 192 SGB VII)
- [ ] Acces la **SV-Meldeportal** și la **ELStAM** prin ELSTER
- [ ] Unfallversicherung, Arbeitsschutz, evidența timpului de lucru (§ 17 MiLoG)

## Anti-pattern-uri

| Gând | Realitate |
|---|---|
| „Minijob = fără obligații" | Anmeldung la Minijob-Zentrale, contribuții forfetare, evidența orelor obligatorie (§ 17 MiLoG). |
| „Contribuțiile SV se plătesc pe 15, ca impozitele" | A 3-a ultimă zi lucrătoare a **lunii curente**, estimat. Fără Schonfrist. |
| „Freelancerul își plătește singur asigurările" | Risc de **Scheinselbständigkeit** → contribuții retroactive 4 ani (30 ani la intenție), § 25 SGB IV. Verifică cu Statusfeststellungsverfahren § 7a SGB IV. |
| „Valorile SV le știu din anul trecut" | Rechengrößen se modifică anual prin Verordnung. **Verifică întotdeauna live.** |
| „Am doar contractori, nu datorez KSA" | Künstlersozialabgabe se datorează pe onorariile plătite artiștilor/publiciștilor independenți, chiar ocazional. |
