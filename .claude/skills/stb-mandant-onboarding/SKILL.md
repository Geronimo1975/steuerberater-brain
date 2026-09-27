---
name: stb-mandant-onboarding
description: Preluarea unui dosar nou în cabinetul de Steuerberater — Fragebogen zur steuerlichen Erfassung §138 AO la înființare, obținerea Steuernummer și USt-IdNr., identificare GwG/KYC, Vollmacht și Vollmachtsdatenbank (VDB) pentru accesul electronic la datele Finanzamt, Mandatsvertrag, preluarea dosarului de la consilierul anterior. Folosește la „client nou", „firmă nouă", „am înființat", „Vollmacht", „vreau să preiau un dosar".
---

# Onboarding dosar / mandat

`Stand: 2026-09-25`

## 1. Firmă nouă — Fragebogen zur steuerlichen Erfassung

| Element | Regulă |
|---|---|
| Temei | § 138 Abs. 1, 1b AO |
| Termen | **1 lună** de la începerea activității |
| Formă | **obligatoriu electronic** prin ELSTER (din 2021) |
| Rezultat | Steuernummer, clasificarea obligațiilor, semnalul USt |

Puncte de decizie din formular care determină ani de consecințe:

- [ ] **Kleinunternehmer § 19 UStG** sau Regelbesteuerung? (Verzicht obligă 5 ani)
- [ ] **Soll- sau Istversteuerung**? Istversteuerung (§ 20 UStG) îmbunătățește semnificativ lichiditatea — cerere separată, prag 800.000 € ⚠️
- [ ] Estimarea cifrei de afaceri și a profitului → determină Vorauszahlungen ESt/GewSt și ritmul UStVA
- [ ] Gewerbe (§ 15 EStG) sau freie Beruf (§ 18 EStG)? Determină GewSt, IHK vs. lipsă de cameră, obligația de Gewerbeanmeldung
- [ ] Angajați? → declanșează Betriebsnummer, BG, ELStAM
- [ ] USt-IdNr. necesară? (servicii B2B transfrontaliere) — se cere la BZSt
- [ ] SEPA-Lastschriftmandat pentru FA

## 2. Pașii paraleli la înființare

| Pas | Unde | Termen |
|---|---|---|
| Gewerbeanmeldung (§ 14 GewO) | Gemeinde / Samtgemeinde Hanstedt | înainte de începere |
| Fragebogen § 138 AO | ELSTER | 1 lună |
| Handelsregister | Notar → Amtsgericht | la formele societare |
| Transparenzregister | transparenzregister.de | la înființare |
| IHK / HWK | automat prin Gewerbeanmeldung | — |
| Berufsgenossenschaft | BG competentă | 1 săptămână |
| Betriebsnummer | Bundesagentur für Arbeit | înainte de prima angajare |
| Rundfunkbeitrag | Beitragsservice | la înființare |
| LUCID (dacă ambalaje) | ZSVR | înainte de prima punere pe piață |

## 3. 🔑 Vollmacht & Vollmachtsdatenbank (VDB)

| Element | Regulă |
|---|---|
| Ce e | Registrul electronic al împuternicirilor, administrat de Steuerberaterkammern |
| Ce face | Finanzverwaltung preia împuternicirea electronic; Steuerberaterul poate prelua date (Vorausgefüllte Steuererklärung), primi Bescheide și corespondență |
| De ce contează | Marchează dosarul ca **`beraten`** → se aplică termenul lung din **§ 149 Abs. 3 AO** |
| Formular | `Amtliche Vollmacht` (Beiblatt pentru Bekanntgabevollmacht) |
| Condiție | Mandat activ + înregistrare în VDB |

> **Levier practic**: la un dosar întârziat, transmiterea împuternicirii și înregistrarea în VDB poate muta termenul de depunere cu până la 7 luni (§ 149 Abs. 3 AO vs. Abs. 2). ⚠️ Efectul la un dosar cu Erinnerung deja emisă trebuie verificat live și confirmat cu FA.

## 4. Identificare GwG (KYC) — obligatorie

`Quelle: §§ 10-13 GwG` · Steuerberaterul e **Verpflichteter** (§ 2 Abs. 1 Nr. 12 GwG)

- [ ] Identificarea clientului pe bază de act de identitate (copie arhivată)
- [ ] Identificarea **beneficiarului real** (§ 3 GwG) și verificarea în Transparenzregister
- [ ] Clarificarea scopului și naturii relației de afaceri
- [ ] Verificare **PEP** și țări cu risc ridicat → verstärkte Sorgfaltspflichten (§ 15 GwG)
- [ ] Clarificarea originii fondurilor la risc ridicat
- [ ] Arhivare **5 ani** (§ 8 GwG)
- [ ] `Unstimmigkeitsmeldung` (§ 23a GwG) dacă registrul nu corespunde realității

Fără KYC complet, relația de afaceri **nu poate fi începută** (§ 10 Abs. 9 GwG).

## 5. Preluarea de la consilierul anterior

- [ ] Mandatsvertrag scris + clauza de onorariu (StBVV)
- [ ] Revocarea vechii Vollmacht, înregistrarea celei noi în VDB
- [ ] Solicitarea dosarului (Handakte) — atenție la **Zurückbehaltungsrecht** pentru onorarii neplătite (§ 66 Abs. 4 StBerG)
- [ ] Preluarea datelor contabile (DATEV-Bestand, Saldenvorträge, registrul de imobilizări)
- [ ] Inventar al termenelor deschise și al perioadelor nedeclarate → **verifică imediat dacă există Erinnerungen sau Bescheide sub § 164 AO**
- [ ] Verificarea Festsetzungsverjährung (§§ 169-171 AO)
- [ ] Berufshaftpflicht: confirmarea acoperirii pentru mandatul preluat

## 6. Fișa de dosar

Orice dosar nou primește un `AKTE.md` pornit din `mandanten/_TEMPLATE/AKTE.md` și o linie în `mandanten/index.md`.
