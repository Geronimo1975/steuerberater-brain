---
name: stb-jahresabschluss
description: Încheierea exercițiului și declarațiile anuale germane — Einnahmenüberschussrechnung (EÜR) §4 Abs.3 EStG, bilanț și E-Bilanz §5b EStG, Einkommensteuererklärung cu anexele G/S/EÜR, Körperschaftsteuer, Gewerbesteuer, Feststellungserklärung §180 AO, Größenklassen HGB, Offenlegung §325 HGB, precum și încetarea sau suspendarea activității (Betriebsaufgabe vs. Betriebsunterbrechung). Folosește la orice întrebare despre EÜR, bilanț, declarație anuală, închidere de firmă sau depunere la Unternehmensregister.
---

# Jahresabschluss & declarații anuale

`Stand: 2026-09-25` · ⚠️ = de verificat live.

## 1. Ce tip de determinare a profitului?

```
Buchführungspflicht?
  │
  ├─ Kaufmann §§ 1-6 HGB (GmbH, UG, OHG, KG, e.K. peste praguri)  → BILANZ
  ├─ Depășire praguri § 141 AO / § 241a HGB                        → BILANZ
  │      Umsatz > 800.000 €  SAU  Gewinn > 80.000 €
  │      (praguri din exercițiile care încep după 31.12.2023)
  │      ⚠️ Obligația începe abia din exercițiul URMĂTOR notificării FA (§141 Abs.2 AO)
  ├─ Freiberufler § 18 EStG (indiferent de cifră)                  → EÜR (drept de opțiune)
  └─ Sub praguri, fără calitate de Kaufmann                        → EÜR § 4 Abs. 3 EStG
```

## 2. Ce declarații, pe formă juridică

| Formă | Declarații obligatorii |
|---|---|
| **Einzelunternehmer (Gewerbe)** | ESt + **Anlage G** + **Anlage EÜR** (sau bilanț/E-Bilanz) + **GewSt** (dacă profit > 24.500 € Freibetrag) + USt |
| **Freiberufler** | ESt + **Anlage S** + **Anlage EÜR** + USt · **fără GewSt** |
| **GbR / OHG / KG** | **Feststellungserklärung § 180 AO** + GewSt + USt · asociații declară cota în ESt |
| **GmbH / UG** | **KSt** + GewSt + USt + **E-Bilanz § 5b EStG** + **Offenlegung § 325 HGB** |

## 3. Anexele ESt uzuale

| Anexă | Pentru |
|---|---|
| Anlage G | Venituri din activitate comercială (Gewerbebetrieb) |
| Anlage S | Venituri din profesii liberale |
| Anlage EÜR | Determinarea profitului §4 Abs.3 EStG — **obligatoriu electronic** (§ 60 Abs. 4 EStDV) |
| Anlage AVEÜR | Registrul imobilizărilor aferent EÜR |
| Anlage N | Venituri salariale |
| Anlage V | Chirii |
| Anlage KAP | Venituri din capital |
| Anlage SO | Venituri diverse, inclusiv § 23 EStG |
| Anlage Vorsorgeaufwand | Asigurări |
| Anlage Kind | Copii |

## 4. Größenklassen HGB

`Quelle: §§ 267, 267a HGB · praguri noi din Gesetz v. 11.04.2024, obligatorii pentru exerciții ≥ 01.01.2024`

| Clasă | Bilanzsumme | Umsatz | Angajați |
|---|---|---|---|
| Kleinstkapitalgesellschaft (§ 267a) | ≤ 450.000 € | ≤ 900.000 € | ≤ 10 |
| Klein | ≤ 7.500.000 € | ≤ 15.000.000 € | ≤ 50 |
| Mittelgroß | ≤ 25.000.000 € | ≤ 50.000.000 € | ≤ 250 |
| Groß | peste | peste | peste |

Încadrarea cere depășirea a **două din trei** criterii, la **două** date de bilanț consecutive (§ 267 Abs. 4 HGB).

## 5. Termene

| Obligație | Termen |
|---|---|
| Declarații anuale, fără Steuerberater | 31.07 anul următor (§ 149 Abs. 2 AO) |
| Declarații anuale, **cu Steuerberater** | ultima zi din februarie, an +2 (§ 149 Abs. 3 AO) |
| Offenlegung Jahresabschluss | 12 luni de la Bilanzstichtag (§ 325 Abs. 1a HGB) |
| Aufstellung Jahresabschluss — Kapitalgesellschaft | 3 luni (mici: 6 luni) de la Bilanzstichtag (§ 264 Abs. 1 HGB) |

Tabel complet cu prelungirile post-Corona: `stb-kanzlei/references/erinnerung-schaetzung.md`.

## 6. Zone cu risc ridicat → citește referința

| Temă | Fișier |
|---|---|
| **Încetare / suspendare de activitate** | `references/betriebsaufgabe.md` 🔴 |
| EÜR, E-Bilanz, trecerea între metode | `references/euer-bilanz.md` |
| Offenlegung, Ordnungsgeld, Unternehmensregister | `references/offenlegung.md` |

## Anti-pattern-uri

| Gând | Realitate |
|---|---|
| „Am depășit 800.000 €, deci trebuie să țin contabilitate în partidă dublă de anul ăsta" | Obligația începe din exercițiul **următor** notificării FA (§ 141 Abs. 2 AO). |
| „Închid firma, doar nu mai declar nimic" | Betriebsaufgabe declanșează **Aufgabegewinn** impozabil pe rezervele latente. Vezi `betriebsaufgabe.md`. |
| „Freiberufler datorează Gewerbesteuer" | Nu. § 18 EStG ≠ § 15 EStG. Dar atenție la **Abfärbetheorie** § 15 Abs. 3 Nr. 1 EStG la societăți mixte. |
| „EÜR o pot trimite pe hârtie" | Anlage EÜR e obligatoriu electronică (§ 60 Abs. 4 EStDV), exceptând Härtefall § 150 Abs. 8 AO. |
| „GewSt se datorează de la primul euro" | Freibetrag 24.500 € pentru persoane fizice și societăți de persoane (§ 11 Abs. 1 GewStG). Nu și pentru Kapitalgesellschaften. |
