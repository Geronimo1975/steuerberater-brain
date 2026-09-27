# Steuerberater Brain

Un „creier" Claude Code pentru un cabinet de **Steuerberater** din Germania: skill-uri, agenți și comenzi care acoperă obligațiile de raportare către Finanzamt.

Construit pentru un cabinet din **Niedersachsen** (Landkreis Harburg, Finanzamt Winsen/Luhe), dar structura e reutilizabilă pentru orice Land — se schimbă profilul din `CLAUDE.md`.

> ⚠️ **Nu este consultanță fiscală.** Dreptul fiscal german se schimbă anual. Fiecare valoare din `references/` poartă `Stand:` și `Quelle: §`, iar cele marcate `⚠️` sunt neconfirmate și trebuie verificate live înainte de folosire.

## Instalare

```bash
git clone <acest-repo> && cd steuerberater-brain
cp CLAUDE.template.md CLAUDE.md
cp mandanten/index.template.md mandanten/index.md
```

Completează `CLAUDE.md` cu datele cabinetului. Ambele fișiere completate sunt în `.gitignore` — datele reale nu se întorc niciodată în git.

## Structura

```
.claude/
├── skills/
│   ├── stb-kanzlei/            ROUTER — intrarea în tot sistemul
│   │   └── references/         fristenkalender · erinnerung-schaetzung
│   │                           rechtsquellen · portale · werte-2025-2026
│   ├── stb-umsatzsteuer/       UStVA · Dauerfristverlängerung · ZM · OSS
│   │                           § 19 Kleinunternehmer · eRechnung · § 13b
│   ├── stb-lohn-sv/            LSt-Anmeldung · DEÜV · BG · KSK · A1 · MiLoG
│   ├── stb-jahresabschluss/    EÜR · E-Bilanz · ESt/KSt/GewSt · § 180 AO
│   │                           Offenlegung · Betriebsaufgabe
│   ├── stb-meldepflichten/     Transparenzregister · DAC6/DAC7 · Intrastat
│   │                           Bundesbank AWV · LUCID
│   ├── stb-mandant-onboarding/ § 138 AO · GwG-KYC · Vollmacht · VDB
│   └── stb-berufsrecht/        StBerG · BOStB · StBVV · GwG · DSGVO
├── agents/
│   ├── rechts-recherche.md     verificare live a legii, citare § obligatorie
│   ├── fristen-auditor.md      scanează dosarele → ce e scadent
│   └── beleg-extraktor.md      extrage date din Bescheide scanate
└── commands/
    ├── /fristen                inventar de termene
    ├── /erinnerung             procesează o scrisoare de la Finanzamt
    ├── /mandant-neu            deschide un dosar nou
    └── /ust-check              verifică situația de TVA a unui dosar
```

## Cum se folosește

Routerul `stb-kanzlei` e punctul de intrare. Orice întrebare fiscală trece prin el, iar el trimite la skill-ul de domeniu. Fișierele din `references/` se încarcă doar când sunt necesare — contextul rămâne mic.

Fiecare dosar primește un `AKTE.md` pornit din `mandanten/_TEMPLATE/AKTE.md`: Stammdaten, statut fiscal, termene, corespondență cu Finanzamt, întrebări deschise.

## Principii

1. **Skill-first** — nu se răspunde din memorie la întrebări fiscale.
2. **Fiecare cifră are `Stand:` și `Quelle: §`** — fără sursă, nu se afirmă.
3. **Verificare live** înainte de a consilia despre termene, praguri sau sume.
4. **Nimic nu se transmite la ELSTER/BZSt fără confirmarea explicită** a utilizatorului.
5. **Datele personale rămân local** — IdNr., Steuernummer, IBAN nu ajung în git, în artifacts sau la servicii externe.
6. **§ 108 Abs. 3 AO** se aplică la fiecare dată calculată.

## Acoperire juridică

AO · EStG/EStDV · UStG/UStDV · KStG · GewStG · HGB · NGrStG · SGB IV/VII/IX · DEÜV · MiLoG · KSVG · StBerG · DVStB · BOStB · StBVV · GwG · PStTG · AWV · VerpackG
