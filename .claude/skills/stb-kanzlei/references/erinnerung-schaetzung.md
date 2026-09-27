# Scrisori de la Finanzamt — Erinnerung, Verspätungszuschlag, Schätzung

`Stand: 2026-09-25` · `Quelle: AO §§ 109, 149, 152, 162, 347, 361`

## 1. Scara escaladării

```
Abgabefrist (§149 AO)
      ↓ expirat
ERINNERUNG          →  scrisoare de reamintire, dă un termen administrativ nou
      ↓ ignorat
ANDROHUNG           →  Zwangsgeld angedroht (§§ 328-332 AO)
      ↓ ignorat
SCHÄTZUNG §162 AO   →  FA estimează bazele de impunere, de regulă în defavoarea contribuabilului
      +
VERSPÄTUNGSZUSCHLAG §152 AO
      +
ZINSEN §233a AO
```

**Erinnerung nu prelungește un termen deja expirat.** Formularul o spune literal: *„Dieses Schreiben verlängert keine bereits abgelaufene Abgabefrist. Die oben genannte Frist stellt keine Fristverlängerung dar."*

## 2. Termene de depunere — § 149 AO

| Caz | Temei | Termen |
|---|---|---|
| Fără consilier | § 149 Abs. 2 AO | 31.07 al anului următor |
| **Cu Steuerberater** | § 149 Abs. 3 AO | ultima zi din februarie, anul +2 |
| Vorabanforderung | § 149 Abs. 4 AO | FA poate cere mai devreme, min. 4 luni |

Termene efective după prelungirile post-Corona (Viertes Corona-Steuerhilfegesetz):

| VZ | Nebeeratene | **Beratene (§149 Abs.3)** |
|---|---|---|
| 2022 | 02.10.2023 | 31.07.2024 |
| 2023 | 02.09.2024 | 02.06.2025 |
| 2024 | 31.07.2025 | 30.04.2026 |
| **2025** | **31.07.2026** | **01.03.2027** ⚠️ (28.02.2027 = duminică → §108 Abs.3 AO) |
| 2026 | 02.08.2027 ⚠️ | 28.02.2028 ⚠️ |

> 🔑 **Levierul cel mai puternic**: dacă declarația e întocmită de un Steuerberater, se aplică termenul lung din § 149 Abs. 3 AO. Pentru VZ 2025 asta înseamnă **01.03.2027** în loc de 31.07.2026.
> ⚠️ De verificat live dacă FA acceptă aplicarea retroactivă când a emis deja o Erinnerung. Condiția practică: **Vollmacht înregistrată în Vollmachtsdatenbank (VDB)** a Steuerberaterkammer, astfel încât FA să vadă dosarul ca *beraten*. Vezi skill `stb-mandant-onboarding`.

## 3. Reacția imediată — arborele de decizie

```
A venit o Erinnerung
  │
  ├─ Pot depune declarația până la termen?
  │     └─ DA → depune. Erinnerung devine "gegenstandslos".
  │
  ├─ NU, dar termenul încă nu a expirat
  │     └─ ANTRAG AUF FRISTVERLÄNGERUNG (§ 109 AO), în scris, ÎNAINTE de expirare
  │        + motiv concret + dată propusă realistă
  │
  ├─ NU, termenul a expirat deja
  │     └─ Depune cât mai repede + Antrag pe §109 Abs.1 S.2 AO (prelungire retroactivă)
  │        + explică de ce întârzierea nu e culpabilă (§152 Abs.5 AO)
  │
  └─ Nu există obligație de depunere?
        └─ Comunică FA în scris, cu motivare. Erinnerung nu se ignoră niciodată.
```

## 4. Verspätungszuschlag — § 152 AO

| Regulă | Conținut |
|---|---|
| Kann-Zuschlag | § 152 Abs. 1 AO — la latitudinea FA |
| **Muss-Zuschlag** | § 152 Abs. 2 AO — **obligatoriu** dacă declarația e depusă cu peste 14 luni după sfârșitul anului fiscal (sau după Vorabanforderung) |
| Excepții de la Muss | § 152 Abs. 3 AO — ex. prelungire acordată, impozit = 0 sau rambursare |
| Cuantum | § 152 Abs. 5 AO — **0,25 % din impozitul stabilit minus avansuri/reţineri, per lună începută, minim 25 €/lună** |
| Plafon | **25.000 €** (§ 152 Abs. 10 AO) |

Pentru declarații fără impozit de plată (Erstattungsfall), Muss-Zuschlag nu se aplică — dar Kann-Zuschlag rămâne posibil.

## 5. Schätzung — § 162 AO

- FA estimează bazele de impunere dacă nu le poate determina (§162 Abs.1 AO).
- Estimarea trebuie să fie plauzibilă, dar FA poate folosi **Sicherheitszuschläge** — rezultatul e de regulă mai mare decât realitatea.
- **Obligația de depunere NU dispare** după Schätzung. Declarația rămâne datorată.
- Bescheid-ul de estimare e de obicei emis **unter Vorbehalt der Nachprüfung** (§ 164 AO) → poate fi corectat prin depunerea declarației reale.

## 6. Einspruch — § 347 AO

| Element | Regulă |
|---|---|
| Termen | **1 lună** de la comunicarea Bescheid-ului (§ 355 Abs. 1 AO) |
| Comunicare | § 122 Abs. 2 Nr. 1 AO — a 3-a zi după poștare (⚠️ din 2025 discutat 4 zile — verifică live) |
| Formă | scris sau electronic prin ELSTER |
| Efect | **Nu suspendă plata.** Pentru asta: `Antrag auf Aussetzung der Vollziehung` (§ 361 AO) |
| Risc | Verböserung (§ 367 Abs. 2 S. 2 AO) — FA poate înrăutăți, după avertizare prealabilă |

## 7. Șablon — Antrag auf Fristverlängerung (§ 109 AO)

```
An das Finanzamt Winsen (Luhe)
Von-Somnitz-Ring 6
21423 Winsen (Luhe)

Steuernummer: <StNr>
Betreff: Antrag auf Fristverlängerung gem. § 109 AO
        für die <Art der Erklärung> <VZ>
Bezug:  Ihre Erinnerung vom <Datum>

Sehr geehrte Damen und Herren,

hiermit beantrage ich, die Frist zur Abgabe der oben genannten
Steuererklärung(en) bis zum <konkretes Datum> zu verlängern.

Begründung: <motiv concret și verificabil>

Die Erklärung(en) werden bis zum genannten Termin vollständig
über ELSTER übermittelt.

Mit freundlichen Grüßen
<Name, Datum, Unterschrift>
```

> Motive acceptate în practică: documente lipsă de la terți, boală, schimbare de consilier, complexitate. Motive slabe: „nu am avut timp".

## 8. Checklist de aplicat la fiecare Erinnerung

- [ ] Extrage: Steuernummer, IdNr., data scrisorii, termenul, declarațiile lipsă, VZ
- [ ] Verifică dacă există obligație de depunere (§ 149 Abs. 1 AO + legea specială)
- [ ] Verifică dacă termenul legal era deja expirat
- [ ] Calculează expunerea la § 152 AO (0,25 %/lună, min. 25 €/lună, max. 25.000 €)
- [ ] Decide: depunere imediată / Antrag § 109 AO / clarificare
- [ ] Notează în `<Dosar>/AKTE.md` sub „Fristen & Status"
- [ ] Verifică dacă preluarea de un Steuerberater mută termenul la § 149 Abs. 3 AO
