# Kleinunternehmerregelung § 19 UStG & eRechnung

`Stand: 2026-09-25`

## 1. Reforma § 19 UStG din 01.01.2025

| Element | Până 2024 | **Din 01.01.2025** |
|---|---|---|
| Prag an precedent | 22.000 € | **25.000 €** |
| Prag an curent | 50.000 € (estimat) | **100.000 €** (efectiv) |
| Natură juridică | USt „nu se percepe" | **Steuerbefreiung reală** (§ 19 Abs. 1 UStG) |
| Depășire în cursul anului | efect abia din anul următor | **impozitare de la tranzacția care depășește 100.000 €**, în cursul anului |
| USt-Jahreserklärung | obligatorie | **nu mai e obligatorie** (§ 19 Abs. 1 **S. 2** UStG) |
| Regim UE | inexistent | **§ 19a UStG** — EU-Kleinunternehmerregelung |

### Firme noi (Neugründung)

- În anul înființării, pragul decisiv este **100.000 €**, nu 25.000 € — nu există an precedent de referință.
  > `Quelle: UStAE Abschn. 19.1 Abs. 3, în versiunea BMF-Schreiben v. 18.03.2025`:
  > *Entsprechend der Zweckbestimmung des § 19 Abs. 1 UStG ist im Jahr der Aufnahme der Tätigkeit die Grenze von 100.000 € maßgebend.*
- **Hochrechnung** (extrapolarea la an întreg) a fost **eliminată**. Se compară cifra de afaceri **efectivă** a anului curent cu cele 100.000 €.
- Depășirea celor 100.000 € în anul înființării → impozitare normală **de la tranzacția respectivă**.
- Depășirea celor 25.000 € în anul înființării → impozitare normală **de la tranzacția respectivă**.

### Ce rămâne valabil și pentru Kleinunternehmer

- **§ 13b UStG** Reverse Charge la prestații primite din străinătate → USt datorată, **fără** drept de deducere.
- **Achiziții intracomunitare** peste 12.500 € sau la opțiune (§ 1a Abs. 3 UStG).
- Nevoia unei **USt-IdNr.** pentru servicii B2B transfrontaliere (§ 3a Abs. 2 UStG) + **ZM**.
- Obligația de a **recepționa eRechnung** (vezi §3 mai jos).

### Verzicht (opțiunea pentru Regelbesteuerung) — § 19 Abs. 3 UStG

- Se declară la FA; obligă **5 ani calendaristici**.
- Util când investițiile inițiale generează Vorsteuer mare sau clientela e exclusiv B2B.
- ⚠️ Termenul exact de declarare și de revocare sub noul regim: verifică live.

### Factura de Kleinunternehmer

- Fără USt afișată. **Niciodată** nu se menționează cota sau suma USt — altfel § 14c Abs. 2 UStG: USt datorată deși nu era cazul.
- Obligatorie mențiunea scutirii (ex. *„Steuerfrei nach § 19 UStG"*).

## 2. § 19a UStG — Kleinunternehmer în alt stat UE

- Permite aplicarea regimului de scutire în alte state membre.
- Necesită înregistrare la **BZSt** și un **număr de identificare cu sufixul „-EX"**.
- **Meldung trimestrială** a cifrei de afaceri pe state membre, în termen de 1 lună de la sfârșitul trimestrului.
- Prag UE: 100.000 € cifră de afaceri totală în UE.

## 3. eRechnung — calendarul obligațiilor

`Quelle: § 14 UStG, Wachstumschancengesetz; BMF-Schreiben 15.10.2024`

| De la | Obligație |
|---|---|
| **01.01.2025** | **Recepția** de eRechnung structurată e obligatorie pentru **toate** firmele germane în relații B2B naționale. Nu e nevoie de acordul destinatarului. Practic: o adresă de e-mail e suficientă. |
| până 31.12.2026 | Tranzitoriu: se poate **emite** pe hârtie sau PDF, cu acordul destinatarului |
| **01.01.2027** | **Emitere** obligatorie pentru firme cu cifră de afaceri an precedent **> 800.000 €** |
| **01.01.2028** | **Emitere** obligatorie pentru **toate** firmele |
| până 31.12.2027 | EDI rămâne admis în regim tranzitoriu |

### Format

- Standard european **EN 16931**.
- Admise: **XRechnung** și **ZUGFeRD ≥ 2.0.1** (profil EN 16931/Comfort sau superior).
- **Nu** sunt eRechnung: PDF simplu, imagine scanată, ZUGFeRD profil MINIMUM sau BASIC-WL.

### Excepții de la obligația de emitere

- Facturi de valoare mică ≤ 250 € (§ 33 UStDV)
- Bilete de transport (§ 34 UStDV)
- Prestații scutite conform § 4 Nr. 8–29 UStG
- **Kleinunternehmer** — scutiți de obligația de **emitere** (§ 14 Abs. 2 UStG), dar **nu** de cea de recepție

### Arhivare

- Partea structurată (XML) se păstrează în original, needitată, **8 ani** (§ 147 Abs. 3 AO, termen redus de la 10 la 8 ani prin Wachstumschancengesetz, aplicabil documentelor al căror termen nu expirase la 01.01.2025 ⚠️).
- Cerințe GoBD: Unveränderbarkeit, Nachvollziehbarkeit, Verfahrensdokumentation.
