# git tutorial

# Algemeen

Git is software dat aanpassingen in code bij kan houden. Lokaal wordt er een repository aangemaakt in een projectfolder. Hierin kunnen wijzigingen worden bijgehouden door een "commit" uit te voeren. Deze lokale repository kan dan worden gesynchroniseerd met een remote repository zoals Github.
  
Github is handig omdat het alle aanpassingen in je code kan bijhouden, er kunnen meerdere programmeurs werken aan een code, het is efficient en Github kan worden gebruikt als portfolio.

# Setup

Git installeren
- Windows: http://git-scm.com/downloads
- Mac: *brew install git*
- Ubuntu: *apt-get install git*

Account aanmaken
Ga naar: https://github.com/

# Configuratie

Voer dit uit in bash:

- *$ git config --global user.name "Jou Naam"*
- *$ git config --global user.email "email@email.nl"*

# Repository aanmaken

Maak een nieuwe map en voer dit uit om een nieuwe repository aan te maken.
- *git init*

Een lokale repository kan je met dit binnen halen:
- *git clone /path/to/repository*

Als je git server niet lokaal staat moet je dit uitvoeren:
- *git clone gebruikersnaam@host:/path/to/repository*

# Werkwijze

Je lokale repository bestaat uit 3 verschillende 'trees' beheerd door git.
- Je Working Directory waarin je bestanden staan.
- Je Index dat zich als tussen stadium gedraagt.
- Je HEAD die verwijst naar de laatste 'commit' die je hebt gemaakt.


