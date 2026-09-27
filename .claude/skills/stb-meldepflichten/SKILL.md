---
name: stb-meldepflichten
description: Raportări germane non-fiscale și speciale — Transparenzregister și beneficiari reali (GwG), DAC6 (Steuergestaltungen transfrontaliere §§138d-k AO), DAC7/PStTG pentru operatori de platforme, Intrastat, statistici Destatis, raportări Bundesbank AWV Z4/Z5, Wirtschafts-Identifikationsnummer, LUCID/VerpackG, Rundfunkbeitrag, Meldepflicht case de marcat §146a AO. Folosește când întrebarea nu e o declarație fiscală clasică, ci o obligație de raportare către alt registru sau autoritate.
---

# Meldepflichten speciale

`Stand: 2026-09-25` · ⚠️ = de verificat live.

## Triaj rapid

| Întrebare | Mergi la |
|---|---|
| Beneficiar real, GwG, registru de transparență | `references/transparenzregister-gwg.md` |
| Structuri transfrontaliere, platforme online | `references/dac6-dac7.md` |
| Intrastat, statistici, plăți externe | `references/statistik-bundesbank.md` |

## Tabel sinoptic

| Raportare | Cine | Termen | Autoritate |
|---|---|---|---|
| **Transparenzregister** | Toate persoanele juridice și societățile înregistrate | „unverzüglich" la modificare | Bundesanzeiger Verlag |
| **DAC6** | Intermediari / contribuabili, structuri transfrontaliere | **30 zile** | BZSt |
| **DAC7 / PStTG** | Operatori de platforme digitale | **31.01** anul următor | BZSt |
| **Intrastat** | Comerț intra-UE peste prag | a 10-a zi lucrătoare | Destatis (IDEV) |
| **AWV Z4** | Plăți externe > 50.000 € | ziua **7** a lunii următoare | Bundesbank |
| **AWV Z5** | Creanțe/datorii față de nerezidenți > 5 Mio € | ziua 7 | Bundesbank |
| **§ 146a Abs. 4 AO** | Case de marcat electronice cu TSE | **1 lună** de la achiziție ⚠️ | ELSTER |
| **LUCID** | Cine pune ambalaje pe piață | înainte de prima punere pe piață + raportare anuală | ZSVR |
| **Rundfunkbeitrag** | Orice sediu de firmă | la înființare | Beitragsservice |
| **W-IdNr. § 139c AO** | Toți Wirtschaftlich Tätige | se alocă din oficiu, etapizat din 11.2024 ⚠️ | BZSt |
| **IHK / HWK** | Membru obligatoriu | la înregistrarea Gewerbe | Camera locală |

## Anti-pattern-uri

| Gând | Realitate |
|---|---|
| „Transparenzregister se completa automat din Handelsregister" | Fikcția de notificare a fost eliminată în 2021. Toate societățile trebuie să raporteze activ. |
| „DAC6 e doar pentru marile corporații" | Se aplică și la structuri mici, dacă bifează un Kennzeichen din § 138e AO. Termen: 30 de zile. |
| „Vând doar pe eBay/Amazon, nu raportez nimic" | Platforma raportează despre tine (DAC7). FA primește datele — necorelarea cu declarația generează control. |
| „Case de marcat — nimic de raportat" | § 146a Abs. 4 AO impune notificarea sistemelor electronice de casă din 2025. |
