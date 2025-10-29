# Installasjon og oppsett av Python og Git

## Førehandskrav – MATLAB

**⚠️ VIKTIG:** Dette prosjektet krev at du har MATLAB installert lokalt på datamaskina di. Du må:

1. Ha betalt semesteravgifta og fått NTNU-epost
2. Lasta ned MATLAB frå [NTNU-portalen](https://se.mathworks.com/academia/tah-portal/ntnu-30833468.html)
3. **OBS:** Du må laste ned MATLAB lokalt på PC-en din – ikkje bruk webversjonen!
4. Du treng òg “Navigation Toolbox”, “Industrial Communication Toolbox” og “Instrument Control Toolbox” installert i MATLAB, samt Simulink

Om du ikkje har dette på plass, gjer det før du held fram med resten av rettleiinga.

---

## Windows-versjon

### Steg 1: Installer Python

Først må vi installere Python på maskina di. Python er programmeringsspråket vi skal bruke av og til.

> Sjølv om du allereie har Anaconda, Spyder eller liknande frå vidaregåande, må du framleis gjere dette steget.

Opne **Command Prompt (CMD)** ved å trykkje **Windows + R**, skriv `cmd`, og trykk **Enter**.

Skriv så denne kommandoen for å installere Python:

```
winget install Python.Python.3.13 --accept-package-agreements
```

> Dette kan òg gjerast via Microsoft Store.

Vent til installasjonen er ferdig. For å sjekke at Python vart installert rett, skriv:

```
python --version
```

Du skal no sjå noko som liknar på `Python 3.x.x`. Om ikkje, prøv å lukke terminalen og opne ei ny.

---

### Steg 2: Installer Git

Git er eit verktøy for å laste ned og administrere kodeprosjekt. Vi installerer det med denne kommandoen:

```
winget install --id Git.Git -e --source winget
```

For å sjekke at Git vart installert rett, skriv:

```
git --version
```

Du skal no sjå noko som liknar på `git version 2.x.x`.

💡 **Tips:** Dersom Git ikkje blir gjenkjent, prøv å lukke terminalen og opne ei ny.

---

### Steg 3: Klon prosjektet

No skal vi laste ned prosjektfilene frå internett. Eit *repository* (eller “repo”) er ganske enkelt eit prosjektarkiv som ligg på nettet.

Først lagar vi ei mappe kalla “github” der vi kan samle alle prosjekta våre:

```
mkdir C:\github\
```

```
cd /d C:\github\
```

No kan vi klone (laste ned) prosjektet:

```
git clone https://github.com/Adriaeik/BIAIS_Oppstartsuka_25
```

**⚠️ Merk:** Får du feilmelding om at mappa alt finst, kan du anten slette den gamle eller klone til eit nytt namn:

```
git clone https://github.com/Adriaeik/BIAIS_Oppstartsuka_25 ny_mappe_namn
```

---

### Steg 4: Gå til prosjektmappa

Når nedlastinga er ferdig, naviger inn i prosjektmappa:

```
cd BIAIS_Oppstartsuka_25
```

💡 **Tips:** Dersom du endra mappenamnet over, bruk det nye her.

---

### Steg 5: Start MATLAB

Skriv inn matlab i terminalen og trykk enter:

```
matlab
```

Vent medan MATLAB startar opp, og bruk tida til å bli kjend med gruppa di.

---

### Steg 6: Opne første oppgåve

I MATLAB: Naviger til `del1/del1_1_fartsregulering.slx` og opne fila. No er de klare til å starte!

---

## Mac-versjon

**⚠️ Merk:** Mac-versjonen er ikkje testa og vil heller ikkje bli testa. Mac-brukarar som får problem må søkje hjelp på Stack Overflow eller liknande. Studentassistentar brukar ikkje tid på dette.

---

### Førehandskrav

På Mac treng du først **Homebrew** (ein pakkebehandlar). Dersom du ikkje har det, installer det ved å følgje instruksjonane på [brew.sh](https://brew.sh).

---

### Steg 1: Installer Python

Opne **Terminal** (søk etter “Terminal” i Spotlight eller finn det i Applications/Utilities).

Installer Python med Homebrew:

```
brew install python
```

Sjekk at installasjonen fungerte:

```
python3 --version
```

---

### Steg 2: Installer Git

Git kjem ofte ferdig installert på Mac, men vi installerer den nyaste versjonen:

```
brew install git
```

Sjekk installasjonen:

```
git --version
```

💡 **Tips:** Dersom Git ikkje blir gjenkjent, prøv å lukke terminalen og opne ei ny.

---

### Steg 3: Klon prosjektet

Naviger til ønskja mappe og opprett ei “github”-mappe for å samle prosjekt:

```
mkdir ~/github/
```

```
cd ~/github/
```

Klon prosjektet:

```
git clone https://github.com/Adriaeik/BIAIS_Oppstartsuka_25
```

---

### Steg 4–6: Felles for begge plattformer

Følg steg 4–6 frå Windows-delen ovanfor. Dei er identiske for begge plattformer.

💡 **Tips for Mac:** `matlab`-kommandoen kan variere avhengig av korleis MATLAB er installert på din Mac.

---

## Kort forklaring av kva som skjer

* **Python** er eit programmeringsspråk som ofte blir brukt til dataanalyse – vi brukar det her for å visualisere data
* **Git** er eit versjonskontrollsystem som let oss laste ned og administrere kodeprosjekt
* **Kloning** betyr å laste ned ein kopi av eit prosjekt frå nettet til di eiga maskin
* **Repository** (repo) er ei samling av filer og mapper som utgjer eit prosjekt

