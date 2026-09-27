# Kanzleiprofil — `<denumire cabinet>`

## 1. Identitate & competențe teritoriale

| Câmp | Valoare |
|---|---|
| Sediu | `<stradă, nr.>`, `<PLZ>` `<localitate>` |
| Samtgemeinde | Hanstedt, **Landkreis Harburg** |
| Bundesland | **Niedersachsen** (⇒ NGrStG, Landesrecht Niedersachsen) |
| Finanzamt competent | **Finanzamt Winsen (Luhe)** |
| Adresă FA | Von-Somnitz-Ring 6, 21423 Winsen · Postfach: 21413 Winsen PF 13 29 |
| Telefon FA | (04171) 656-200 |
| Öffnungszeiten FA | Mo, Di, Do, Fr 08–12 · Do 13–17 |
| Oberbehörde | Landesamt für Steuern Niedersachsen (LStN) |
| Kammer | Steuerberaterkammer Niedersachsen, Hannover |
| Gewerbesteuer-Hebesatz | ⚠️ **de verificat** la Samtgemeinde/Gemeinde Hanstedt |

## 2. Dosare active (Akten)

| Dosar | Steuernummer | Obiect | Fișier |
|---|---|---|---|
| `<nume>` | `<NN/NNN/NNNNN>` | `<ESt / EÜR+USt / KSt …>` | `mandanten/<nume>/AKTE.md` |

Registrul complet: `mandanten/index.md`. Dosare noi → `mandanten/<Nume>/`, pornind de la `mandanten/_TEMPLATE/AKTE.md` sau cu `/mandant-neu`.

## 3. Stare curentă

Termene deschise și dosare cu risc: rulează `/fristen`.

## 4. Reguli de lucru (obligatorii)

1. **Skill-first.** Orice întrebare fiscală → întâi `stb-kanzlei` (router), care trimite la skill-ul de domeniu. Nu răspunde din memorie.
2. **Orice cifră poartă `Stand:` și `Quelle: §`.** Fără sursă = nu se afirmă.
3. **Verificare live obligatorie** înainte de a consilia despre termene, praguri sau sume: agentul `rechts-recherche`. Dreptul fiscal german se schimbă anual (JStG, Wachstumschancengesetz, BEG IV …). Orice marcat `⚠️` este neconfirmat.
4. **Nu se depune nimic la ELSTER/BZSt fără confirmarea explicită** a utilizatorului. Claude pregătește, utilizatorul semnează și trimite.
5. **Date personale.** IdNr., Steuernummer, date bancare rămân **strict local**. Nu se publică în artifacts, nu se trimit către servicii externe, nu apar în commit-uri publice.
6. **Limba:** conversație în română, termenii tehnici și denumirile formularelor **în germană**, netraduse (Einnahmenüberschussrechnung, nu „decont de venituri").
7. **Termene:** când apare o dată, se verifică §108 Abs.3 AO — dacă termenul cade sâmbătă/duminică/sărbătoare legală, se mută pe următoarea zi lucrătoare.

## 5. Harta skill-urilor

| Skill | Când |
|---|---|
| `stb-kanzlei` | **router** · fristenkalender · Erinnerung/Schätzung · portaluri |
| `stb-umsatzsteuer` | UStVA, Dauerfristverlängerung, ZM, OSS, §19 Kleinunternehmer, eRechnung |
| `stb-lohn-sv` | Lohnsteuer-Anmeldung, DEÜV, BG, A1, KSK, Mindestlohn |
| `stb-jahresabschluss` | EÜR, E-Bilanz, ESt/KSt/GewSt-Erklärung, §180 AO, Offenlegung |
| `stb-meldepflichten` | Transparenzregister, DAC6/DAC7, Intrastat, Bundesbank, LUCID |
| `stb-mandant-onboarding` | §138 AO Fragebogen, GwG-KYC, Vollmachten, VDB |
| `stb-berufsrecht` | StBerG, BOStB, StBVV, GwG-Kanzleipflichten, DSGVO |
