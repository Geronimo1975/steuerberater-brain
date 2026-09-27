# EÜR, bilanț, E-Bilanz

`Stand: 2026-09-25` · `Quelle: § 4 Abs. 3, § 5b EStG · § 60 Abs. 4 EStDV · §§ 140-148 AO · §§ 238-263 HGB`

## 1. Einnahmenüberschussrechnung — § 4 Abs. 3 EStG

Principiul **Zufluss-/Abflussprinzip** (§ 11 EStG): contează data încasării/plății, nu a facturii.

Excepții de la Zufluss-/Abflussprinzip:

| Excepție | Regulă |
|---|---|
| Plăți regulat recurente | § 11 Abs. 1 S. 2 / Abs. 2 S. 2 EStG — „10 zile" în jurul finalului de an se alocă anului economic |
| Imobilizări amortizabile | Nu se deduc la plată, ci prin **AfA** (§ 4 Abs. 3 S. 3 EStG) |
| GWG | § 6 Abs. 2 EStG — deducere imediată până la 800 € net ⚠️ (verifică pragul actual) |
| Sammelposten | § 6 Abs. 2a EStG — 250–1.000 €, amortizat liniar pe 5 ani ⚠️ |
| Umlaufvermögen art. § 4 Abs. 3 S. 4 EStG | Terenuri, participații, titluri: deducere abia la ieșire |
| USt | USt încasată = venit; USt plătită = cheltuială; plățile către FA = cheltuială (metoda brută) |

### Anlage EÜR

- **Obligatoriu electronic** (§ 60 Abs. 4 EStDV), exceptând Härtefall (§ 150 Abs. 8 AO).
- Se depune **per întreprindere**, nu per persoană — cine are două activități depune două Anlagen EÜR.
- **Anlage AVEÜR** = registrul imobilizărilor, obligatoriu ca anexă.
- Se transmite odată cu ESt-Erklärung prin ELSTER.

### Obligații de evidență chiar și la EÜR

- Registrul imobilizărilor (`Anlageverzeichnis`) — § 4 Abs. 3 S. 5 EStG
- Evidența GWG peste 250 € — § 6 Abs. 2 S. 4 EStG
- Registrul de casă dacă există încasări în numerar + **TSE** la casă electronică (§ 146a AO)
- Respectarea **GoBD** (BMF 28.11.2019 / 11.03.2024): Unveränderbarkeit, Nachvollziehbarkeit, Verfahrensdokumentation
- Termen de arhivare: **8 ani** pentru documente contabile ⚠️ (redus de la 10 prin Wachstumschancengesetz — verifică aplicabilitatea în cazul concret)

## 2. Când devine obligatoriu bilanțul

| Temei | Prag |
|---|---|
| § 241a HGB | Umsatz > **800.000 €** sau Gewinn > **80.000 €** (exerciții care încep după 31.12.2023) |
| § 141 Abs. 1 AO | Idem, pentru Gewerbetreibende neînregistrați ca Kaufmann |
| §§ 1-6 HGB | Calitatea de Kaufmann (GmbH, UG, OHG, KG, e.K. înregistrat) — indiferent de praguri |

> **§ 141 Abs. 2 AO**: obligația începe abia din exercițiul **următor** celui în care FA a notificat depășirea. Nu retroactiv, nu automat.

**Freiberufler** (§ 18 EStG) nu au niciodată obligație de bilanț, indiferent de cifra de afaceri — dar pot opta.

## 3. Schimbarea metodei (Wechsel der Gewinnermittlungsart)

Trecerea EÜR → bilanț (sau invers) generează un **Übergangsgewinn/-verlust** (R 4.6 EStR):

| Corecție | Efect |
|---|---|
| Creanțe la data trecerii | (+) |
| Datorii la data trecerii | (−) |
| Stocuri | (+) |
| Rückstellungen | (−) |
| Rechnungsabgrenzungsposten | (±) |

- La trecerea EÜR → bilanț, Übergangsgewinn poate fi repartizat, la cerere, pe **3 ani** (R 4.6 Abs. 1 EStR).
- La **Betriebsaufgabe**, Übergangsgewinn e profit curent și **nu** beneficiază de §§ 16 Abs. 4 / 34 EStG → vezi `betriebsaufgabe.md`.

## 4. E-Bilanz — § 5b EStG

- Obligatorie pentru toți cei care întocmesc bilanț.
- Format: **XBRL**, taxonomia HGB publicată anual de BMF.
- Transmitere prin ELSTER, separat de declarațiile fiscale.
- Conținut minim: Bilanz + GuV după **Kerntaxonomie**; Anhang și Lagebericht doar opțional.
- Pentru diferențele fiscal/comercial: fie o **Steuerbilanz** proprie, fie bilanț comercial + **Überleitungsrechnung** (§ 60 Abs. 2 EStDV).
- Termen: odată cu declarația anuală.

## 5. Checklist EÜR

- [ ] Toate încasările/plățile alocate corect pe an (§ 11 EStG + regula celor 10 zile)
- [ ] AfA calculată; registrul imobilizărilor actualizat (Anlage AVEÜR)
- [ ] GWG / Sammelposten tratate corect
- [ ] USt tratată consecvent (metoda brută)
- [ ] Private Nutzung: autovehicul (1 %-Regelung sau Fahrtenbuch), telefon, birou la domiciliu
- [ ] Bewirtungskosten (70 % deductibil, § 4 Abs. 5 Nr. 2 EStG), Geschenke ≤ 50 €
- [ ] Concordanță EÜR ↔ USt-Jahreserklärung (cifra de afaceri declarată)
- [ ] Registrul de casă + TSE dacă există numerar
- [ ] Anul de încetare a activității: verificat `betriebsaufgabe.md`
