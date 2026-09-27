# 🔴 Betriebsaufgabe vs. Betriebsunterbrechung

`Stand: 2026-09-25` · `Quelle: §§ 16, 34 EStG · R 16 EStR · BFH-Rspr. la ruhender Gewerbebetrieb`

> Cea mai scumpă distincție din dreptul fiscal al întreprinderilor mici. Diferența dintre cele două poate fi de zeci de mii de euro. **Nu răspunde niciodată din intuiție la „am închis firma".**

## 1. Cele două regimuri

| | **Betriebsaufgabe** (§ 16 Abs. 3 EStG) | **Betriebsunterbrechung** (ruhender Gewerbebetrieb) |
|---|---|---|
| Ce se întâmplă | Întreprinderea încetează definitiv; activele trec în patrimoniul privat | Activitatea se oprește temporar; întreprinderea continuă latent |
| Impozitare | **Aufgabegewinn** — toate rezervele latente (stille Reserven) devin impozabile dintr-odată | **Fără impozitare** la momentul opririi |
| Activele | Devin Privatvermögen la valoarea comună (gemeiner Wert) | Rămân **Betriebsvermögen** |
| Facilități | Freibetrag § 16 Abs. 4 EStG + cotă redusă § 34 EStG | — |
| Reluarea activității | Necesită o înființare nouă | Se poate relua oricând |

## 2. Regula decisivă: Wahlrecht, nu automatism

Jurisprudența constantă a BFH:

> Simpla încetare a activității **nu** produce prin ea însăși o Betriebsaufgabe. Atâta timp cât activele esențiale (`wesentliche Betriebsgrundlagen`) rămân disponibile și activitatea ar putea fi reluată într-o formă în esență identică, se prezumă o **Betriebsunterbrechung**.

Consecința practică:

```
A încetat activitatea
  │
  ├─ S-a dat o AUFGABEERKLÄRUNG expresă și neechivocă către FA?
  │     └─ DA  → Betriebsaufgabe la data indicată → Aufgabegewinn impozabil
  │
  └─ NU (doar Gewerbeabmeldung, scrisoare de „suspendare", tăcere)
        └─ Prezumție de BETRIEBSUNTERBRECHUNG → fără impozitare acum
           Întreprinderea rămâne latentă, cu obligații declarative reduse
```

> ⚠️ **Gewerbeabmeldung la primărie (§ 14 GewO) NU este o Aufgabeerklärung.** Sunt două acte distincte, cu destinatari diferiți (Gemeinde vs. Finanzamt) și efecte diferite.

## 3. Ce trebuie verificat concret în dosar

- [ ] **Textul exact** al adresei trimise la Finanzamt. Conține cuvântul `Betriebsaufgabe` / `Aufgabe des Betriebs` și o **dată** precisă?
- [ ] Sau spune doar `Ruhen des Betriebs`, `vorübergehende Einstellung`, `Abmeldung`?
- [ ] Există o Gewerbeabmeldung separată la Samtgemeinde Hanstedt? Cu ce dată?
- [ ] Au rămas active esențiale (utilaje, autovehicul, stoc, contracte, clientelă, spațiu)?
- [ ] Ce a răspuns Finanzamt? A dezactivat semnalul USt? A cerut o Aufgabebilanz?
- [ ] Ce rezerve latente ar exista (bunuri amortizate sub valoarea reală, autovehicul, imobil)?

> 🔑 Dacă adresa trimisă e ambiguă, situația e încă modelabilă. Alegerea regimului influențează direct EÜR 2025 și ESt 2025. Clarifică **înainte** de a depune.

## 4. Dacă e Betriebsaufgabe — ce trebuie calculat

### a) Übergangsgewinn (la EÜR)

Cine determină profitul prin EÜR **trebuie să treacă la Bestandsvergleich** pentru calculul Aufgabegewinn (R 4.5 Abs. 6 EStR).

Corecții tipice:
- (+) Creanțe neîncasate (Forderungen)
- (−) Datorii neplătite (Verbindlichkeiten)
- (+) Stocuri (Warenbestand)
- (±) Avansuri, Rechnungsabgrenzungsposten

Übergangsgewinn e **profit curent** (laufender Gewinn) — **nu** beneficiază de § 16 Abs. 4 / § 34 EStG.

### b) Aufgabegewinn — § 16 Abs. 3 EStG

```
  Valoarea comună (gemeiner Wert) a activelor trecute în patrimoniul privat
+ Prețurile obținute din vânzarea activelor
− Valoarea contabilă reziduală (Buchwert)
− Aufgabekosten (costuri de lichidare)
= Aufgabegewinn
```

### c) Facilități

| Facilitate | Condiții |
|---|---|
| **Freibetrag § 16 Abs. 4 EStG** | 45.000 €, **doar dacă** ≥ 55 ani sau invaliditate permanentă; **o singură dată în viață**; se reduce euro cu euro peste un Aufgabegewinn de 136.000 € |
| **§ 34 Abs. 1 EStG** Fünftelregelung | Aplicabilă din oficiu |
| **§ 34 Abs. 3 EStG** cotă redusă | 56 % din cota medie, min. 14 %; doar dacă ≥ 55 ani sau invaliditate; **o singură dată în viață**; plafon 5 Mio € |

### d) Consecințe USt

- Trecerea activelor în patrimoniul privat = `unentgeltliche Wertabgabe` **§ 3 Abs. 1b UStG**, impozabilă.
- **§ 15a UStG** Vorsteuerberichtigung dacă bunurile sunt în perioada de corecție (5 ani mobile / 10 ani imobile).
- Detalii: skill `stb-umsatzsteuer`.

### e) Gewerbesteuer

Aufgabegewinn al unei persoane fizice **nu** e supus Gewerbesteuer (§ 7 S. 1 GewStG coroborat cu jurisprudența) — spre deosebire de Kapitalgesellschaften.

## 5. Obligații declarative după oprirea activității

| Obligație | Se menține? |
|---|---|
| ESt-Erklärung | **Da**, cât timp există venituri impozabile |
| EÜR / Anlage EÜR | **Da**, pentru anul în care a existat activitate, inclusiv parțial |
| USt-Jahreserklärung | **Da**, pentru anul respectiv |
| UStVA | **Da**, cât timp semnalul USt e activ la FA — inclusiv **Nullmeldungen** |
| GewSt-Erklärung | Da, pentru anul cu activitate |
| Gewerbeabmeldung § 14 GewO | Act separat, la Gemeinde |

> 🔴 Capcana cea mai frecventă: activitatea s-a oprit, dar FA nu a dezactivat semnalul USt → lipsesc UStVA pentru anul următor → Erinnerungen, Schätzungen, Verspätungszuschläge pentru o firmă care nu mai are cifră de afaceri. **Cere confirmarea scrisă a dezactivării și arhiveaz-o.**

## 6. Checklist de aplicat

- [ ] Calificat corect: Aufgabe sau Unterbrechung? (pe baza textului adresei, nu a intenției)
- [ ] Dacă Aufgabe: dată exactă stabilită
- [ ] Übergangsgewinn calculat (EÜR → Bestandsvergleich)
- [ ] Aufgabegewinn calculat cu gemeiner Wert al fiecărui activ
- [ ] Verificat dacă se aplică § 16 Abs. 4 și § 34 Abs. 3 EStG (vârstă ≥ 55 ani?)
- [ ] USt: § 3 Abs. 1b + § 15a UStG evaluate
- [ ] Semnal USt la FA: dezactivat și confirmat în scris?
- [ ] Gewerbeabmeldung depusă la Gemeinde?
- [ ] Toate declarațiile anului cu activitate depuse
