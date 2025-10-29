# Installasjon og oppsett av Python og Git

## Forhåndskrav - MATLAB

**⚠️ VIKTIG:** Dette prosjektet krever MATLAB installert lokalt på datamaskinen din. Du må:

1. Ha betalt semesteravgift og fått NTNU-epost
2. Laste ned MATLAB fra [NTNU sin portal](https://se.mathworks.com/academia/tah-portal/ntnu-30833468.html)
3. **OBS:** Du må laste ned MATLAB lokalt på PC-en din - ikke bruk web-versjonen!
4. Du trenger også "Navigation Toolbox", "Industrial Communication Toolbox" og "Instrument Control Toolbox" installert i MATLAB samt Simulink

Hvis du ikke har dette på plass, gjør det før du fortsetter med resten av guiden.

## Windows-versjon

### Steg 1: Installer Python

Først må vi installere Python på datamaskinen din. Python er programmeringsspråket vi skal bruke noen av gangene.

Åpne **Command Prompt** (CMD) ved å trykke **Windows + R**, skriv `cmd`, og trykk **Enter**.

I terminalen, skriv følgende kommando for å installere Python:

```
winget install Python.Python.3.13 --accept-package-agreements
```

Vent til installasjonen er ferdig. For å sjekke at Python ble installert riktig, skriv:

```
python --version
```

Du skal nå se noe som ligner på `Python 3.x.x`. Hvis ikke, prøv å lukke terminalen og åpne en ny.

### Steg 2: Installer Git

Git er et verktøy for å laste ned og administrere kodeprosjekter. Vi installerer det med denne kommandoen:

```
winget install --id Git.Git -e --source winget
```

For å sjekke at Git ble installert riktig, skriv:

```
git --version
```

Du skal nå se noe som ligner på `git version 2.x.x`.

💡 **Tips:** Hvis Git ikke blir gjenkjent, prøv å lukke terminalen og åpne en ny.

### Steg 3: Klon prosjektet

Nå skal vi laste ned prosjektfilene fra internett. Et *repository* (eller "repo") er ganske enkelt et prosjektarkiv som lagres på nettet.

Først lager vi en mappe kalt "github" der vi kan samle alle våre prosjekter:

```
mkdir C:\github\
```

```
cd /d C:\github\
```

Nå kan vi klone (laste ned) prosjektet:

```
git clone https://github.com/Adriaeik/BIAIS_Oppstartsuka_25
```

**⚠️ Advarsel:** Får du en feilmelding om at mappen allerede finnes, kan du enten slette den eksisterende mappen eller klone til et annet navn:

```
git clone https://github.com/Adriaeik/BIAIS_Oppstartsuka_25 ny_mappe_navn
```

### Steg 4: Gå til prosjektmappen

Når nedlastingen er ferdig, naviger inn i prosjektmappen:

```
cd BIAIS_Oppstartsuka_25
```

💡 **Tips:** Hvis du endret mappenavnet over, bruk det nye navnet her.

### Steg 5: Start MATLAB

Skriv inn matlab i terminalen og trykk enter:

```
matlab
```

Vent tålmodig mens MATLAB starter opp, og utnytt muligheten til å bli kjent med gruppa di.

### Steg 6: Åpne første oppgave

I MATLAB: Naviger til `del1/del1_1_fartsregulering.slx` og åpne filen. Nå er dere klare til å sette i gang!

## Mac-versjon

**⚠️ Advarsel:** Mac-versjonen er ikke testet og vil ikke bli testet. Mac-brukere som får problemer må søke hjelp på Stack Overflow eller andre ressurser. Studentassistenter bruker ikke tid på dette.

### Forhåndskrav

På Mac trenger du først **Homebrew** (en pakkebehandler). Hvis du ikke har det, installer det først ved å følge instruksjonene på [brew.sh](https://brew.sh).

### Steg 1: Installer Python

Åpne **Terminal** (søk etter "Terminal" i Spotlight eller finn den i Applications/Utilities).

Installer Python med Homebrew:

```
brew install python
```

Sjekk at installasjonen fungerte:

```
python3 --version
```

### Steg 2: Installer Git

Git kommer ofte ferdig installert på Mac, men vi installerer den nyeste versjonen:

```
brew install git
```

Sjekk installasjonen:

```
git --version
```

💡 **Tips:** Hvis Git ikke blir gjenkjent, prøv å lukke terminalen og åpne en ny.

### Steg 3: Klon prosjektet

Naviger til ønsket mappe og opprett en "github"-mappe for å samle prosjekter:

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

### Steg 4-6: Felles for begge plattformer

Følg steg 4-6 fra Windows-delen ovenfor. De er identiske for begge plattformer.

💡 **Tips for Mac:** `matlab`-kommandoen kan variere avhengig av hvordan MATLAB er installert på din Mac.

## Liten forklaring av hva som skjer

- **Python** er programmeringsspråket som ofte brukes for dataanalyse og analyse - vi bruker det for å visualisere data i dag
- **Git** er et versjonskontrollsystem som lar oss laste ned og administrere kodeprosjekter
- **Kloning** betyr å laste ned en kopi av et prosjekt fra internett til din lokale maskin
- **Repository** (repo) er en samling av filer og mapper som utgjør et prosjekt
