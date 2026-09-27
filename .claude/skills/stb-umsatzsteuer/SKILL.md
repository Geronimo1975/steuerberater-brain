---
name: stb-umsatzsteuer
description: Umsatzsteuer germană — Voranmeldung (UStVA), Dauerfristverlängerung, Jahreserklärung, Kleinunternehmerregelung §19 UStG (praguri noi din 2025), Zusammenfassende Meldung, OSS/IOSS, Reverse Charge §13b, eRechnung, Vorsteuerberichtigung §15a și consecințele USt la încetarea/suspendarea activității. Folosește când apare TVA, UStVA, USt-IdNr., factură germană, Kleinunternehmer, livrare intracomunitară sau Betriebsaufgabe.
---

# Umsatzsteuer

`Stand: 2026-09-25` · ⚠️ = de verificat live cu `rechts-recherche`.

## Arborele de decizie

```
Persoana e Unternehmer (§ 2 UStG)?
  │  NU → fără obligații USt
  └─ DA
      │
      ├─ Kleinunternehmer § 19 UStG? (≤25.000 € an precedent ȘI ≤100.000 € an curent)
      │     └─ DA → facturi FĂRĂ USt · fără Vorsteuerabzug · fără UStVA
      │              · fără USt-Jahreserklärung (§ 19 Abs. 1 S. 2 UStG)
      │              · ATENȚIE: §13b, achiziții intracomunitare și §19a rămân aplicabile
      │              → references/kleinunternehmer-erechnung.md
      │
      └─ NU (Regelbesteuerung)
            ├─ UStVA lunar / trimestrial / scutit? → references/voranmeldung.md
            ├─ Livrări/servicii în UE? → references/zm-oss.md
            ├─ Vânzări B2C în UE peste 10.000 €? → OSS
            └─ Încetare / suspendare activitate? → secțiunea ▼ de mai jos
```

## Praguri-cheie (cele care se schimbă cel mai des)

| Prag | Valoare | Temei |
|---|---|---|
| Kleinunternehmer — an precedent | **25.000 €** (din 01.01.2025; anterior 22.000 €) | § 19 Abs. 1 UStG |
| Kleinunternehmer — an curent | **100.000 €** (din 01.01.2025; anterior 50.000 €) | § 19 Abs. 1 UStG |
| UStVA lunară | USt an precedent **> 9.000 €** (din 2025; anterior 7.500 €) | § 18 Abs. 2 UStG |
| UStVA trimestrială | între 2.000 € și 9.000 € | § 18 Abs. 2 UStG |
| Scutire de UStVA | ≤ **2.000 €** (din 2025; anterior 1.000 €) | § 18 Abs. 2 S. 3 UStG |
| Prag livrări la distanță B2C UE | 10.000 € (total UE) | § 3c Abs. 4 UStG |
| Cote | 19 % standard · 7 % redus | §§ 12 Abs. 1, 2 UStG |

## ▼ USt la încetarea sau suspendarea activității

Aceasta este zona cu cel mai mare risc fiscal. Nu răspunde din intuiție.

| Situație | Consecință USt |
|---|---|
| **Betriebsaufgabe** (încetare definitivă) | Trecerea bunurilor în patrimoniul privat = `unentgeltliche Wertabgabe` **§ 3 Abs. 1b UStG** → impozabilă la valoarea de achiziție/costul actual (§ 10 Abs. 4 Nr. 1 UStG) |
| **Betriebsunterbrechung** (suspendare, ruhender Betrieb) | **Fără** Entnahme. Bunurile rămân în Unternehmensvermögen. Activitatea de Unternehmer continuă latent. |
| Bunuri de investiții | **§ 15a UStG** Vorsteuerberichtigung dacă se iese din perioada de corecție: **5 ani** mobile / **10 ani** imobile |
| Vânzarea întregii afaceri | `Geschäftsveräußerung im Ganzen` **§ 1 Abs. 1a UStG** — neimpozabilă |
| Declarații după oprire | **UStVA și USt-Jahreserklärung rămân datorate** pentru perioada în care semnalul USt e activ la FA — inclusiv `Nullmeldungen` |

> 🔴 **Capcana practică**: o simplă `Gewerbeabmeldung` la primărie **nu** oprește obligația de UStVA. Atâta timp cât Finanzamt nu a dezactivat semnalul USt, lipsa unei UStVA (chiar zero) produce Erinnerungen, Schätzungen și Verspätungszuschläge. Confirmă în scris cu FA dezactivarea și păstrează confirmarea în dosar.
> Distincția **Aufgabe vs. Unterbrechung** are efecte și mai mari la impozitul pe venit → skill `stb-jahresabschluss`, `references/betriebsaufgabe.md`.

## Termene

| Obligație | Termen | Temei |
|---|---|---|
| UStVA | ziua 10 după perioadă | § 18 Abs. 1 UStG |
| UStVA cu Dauerfristverlängerung | +1 lună | §§ 46-48 UStDV |
| Antrag Dauerfristverlängerung | **10.02** + Sondervorauszahlung 1/11 (doar la lunar) | § 48 UStDV |
| Zusammenfassende Meldung | ziua **25** după perioadă | § 18a Abs. 1 UStG |
| OSS | sfârșitul lunii următoare trimestrului | § 18j UStG |
| USt-Jahreserklärung | ca § 149 AO (cu StB: ultima zi febr., an +2) | § 18 Abs. 3 UStG |

## Anti-pattern-uri

| Gând | Realitate |
|---|---|
| „Pragul Kleinunternehmer e 22.000 €" | Din 01.01.2025 e **25.000 / 100.000**. Și e acum scutire reală, nu neimpunere. |
| „Nu mai am activitate, deci nu depun UStVA" | Obligația ține de semnalul USt la FA, nu de activitatea reală. Depune Nullmeldung. |
| „Am închis firma, gata cu TVA-ul" | Entnahme § 3 Abs. 1b UStG + corecție § 15a UStG pot genera USt de plată fără niciun încasat. |
| „Kleinunternehmer = zero obligații USt" | §13b Reverse Charge, achiziții intracomunitare și §19a rămân. |
| „Dauerfristverlängerung se reînnoiește automat" | La lunar da, dar **Sondervorauszahlung trebuie recalculată și plătită până 10.02** în fiecare an. |
| „eRechnung e obligatorie de emis din 2025" | Din 2025 e obligatorie doar **recepția**. Emiterea: 2027 / 2028. |
