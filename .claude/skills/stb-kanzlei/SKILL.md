---
name: stb-kanzlei
description: Router central al cabinetului Steuerberater (Hanstedt / Finanzamt Winsen-Luhe). Folosește-l PRIMUL la orice întrebare fiscală germană — termene (Fristen), scrisori de la Finanzamt (Erinnerung, Bescheid, Prüfungsanordnung), ce declarație trebuie depusă, ce portal se folosește, sau când nu e clar ce domeniu atinge întrebarea. Rutează spre stb-umsatzsteuer, stb-lohn-sv, stb-jahresabschluss, stb-meldepflichten, stb-mandant-onboarding, stb-berufsrecht.
---

# Kanzlei-Router

Punctul de intrare în creierul cabinetului. Nu conține reguli de fond — le are pe cele de navigație, calendarul consolidat de termene și procedura de urgență.

## Regula zero: Rechtsstand

Dreptul fiscal german se schimbă în fiecare an. Fiecare cifră din `references/` poartă `Stand:` și `Quelle: §`.

- Orice valoare marcată **⚠️** = neconfirmată → **verific-o live** înainte de a o folosi într-un sfat.
- Verificarea live se face cu agentul `rechts-recherche` (citare obligatorie de § și sursă oficială).
- Nu inventa termene. Dacă nu ai sursa, spune „nu știu, verific".
- **§ 108 Abs. 3 AO**: termenul care cade sâmbăta, duminica sau într-o sărbătoare legală se mută pe următoarea zi lucrătoare. Aplică asta la **fiecare** dată calculată.

## Pasul 1 — Triaj

| Simptom / întrebare | Mergi la |
|---|---|
| A venit o scrisoare de la Finanzamt (Erinnerung, Bescheid, Androhung, Schätzung) | `references/erinnerung-schaetzung.md` ⬅ **prioritar** |
| „Ce am de depus luna asta / anul ăsta?" | `references/fristenkalender.md` |
| UStVA, Dauerfristverlängerung, ZM, OSS, Kleinunternehmer, eRechnung, §13b | skill **`stb-umsatzsteuer`** |
| Angajați, salarii, LSt-Anmeldung, SV, minijob, A1, BG | skill **`stb-lohn-sv`** |
| EÜR, bilanț, E-Bilanz, ESt/KSt/GewSt-Erklärung, Offenlegung | skill **`stb-jahresabschluss`** |
| Transparenzregister, DAC6/DAC7, Intrastat, Bundesbank, statistici | skill **`stb-meldepflichten`** |
| Client nou, §138 AO, Vollmacht, KYC | skill **`stb-mandant-onboarding`** |
| Onorarii, StBVV, răspundere, GwG-ul cabinetului, DSGVO | skill **`stb-berufsrecht`** |
| „Ce lege reglementează X?" | `references/rechtsquellen.md` |
| **Praguri și sume 2025/2026** (Grundfreibetrag, GWG, GewSt, § 19 UStG, § 152 AO) | `references/werte-2025-2026.md` ✅ **verificat live** |
| „Pe ce portal se depune X?" | `references/portale.md` |

## Pasul 2 — Context de dosar

Înainte de a răspunde despre un dosar concret, **citește fișa**:
- `mandanten/index.md` — registrul tuturor dosarelor
- `<Dosar>/AKTE.md` — Stammdaten, Steuernummern, termene, status

Nu presupune forma juridică. Ea determină ce declarații sunt obligatorii:

```
Einzelunternehmer / Gewerbetreibender → ESt (Anlage G) + EÜR sau Bilanz + GewSt + USt
Freiberufler (§18 EStG)               → ESt (Anlage S) + EÜR + USt         [fără GewSt]
GbR / OHG / KG                        → Feststellung §180 AO + GewSt + USt [+ ESt la asociați]
GmbH / UG                             → KSt + GewSt + USt + E-Bilanz + Offenlegung
```

## Pasul 3 — Reguli de răspuns

1. Termeni germani nu se traduc: `Einnahmenüberschussrechnung`, `Verspätungszuschlag`, `Dauerfristverlängerung`.
2. Fiecare afirmație normativă citează paragraful: „§ 149 Abs. 3 AO".
3. Distinge clar **termen legal** (Gesetz) de **termen administrativ** dintr-o scrisoare (Erinnerung ≠ Fristverlängerung).
4. **Nimic nu se transmite la ELSTER/BZSt fără confirmarea explicită** a utilizatorului.
5. Datele personale (IdNr., Steuernummer, IBAN) rămân local. Niciodată în artifacts sau servicii externe.

## Anti-pattern-uri

| Gând | Realitate |
|---|---|
| „Știu termenul pentru UStVA, e pe 10" | Da — dar cu Dauerfristverlängerung e 10 luna următoare, iar §108 Abs.3 AO poate muta data. Verifică fișa. |
| „Pragul Kleinunternehmer e 22.000 €" | S-a schimbat din 01.01.2025. Citește `stb-umsatzsteuer`. |
| „Erinnerung înseamnă că mai am timp" | Erinnerung **nu** prelungește un termen deja expirat. Scrie asta chiar în scrisoare. |
| „Depun eu repede prin ELSTER" | Confirmarea utilizatorului e obligatorie înainte de orice transmitere. |
| „E doar o estimare, o corectez la cifra exactă mai târziu" | O cifră fiscală fără sursă e un risc de §152/§162 AO. Marchează-o `⚠️` explicit. |
