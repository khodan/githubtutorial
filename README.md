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

# Add & Commit

Met *git add* kan je aanpassingen toevoegen aan de Index.

Met *git commit -m* voer je de aanpassingen door.

# Aanpassingen doorsturen

Je aanpassingen zitten nu in de HEAD van je lokale werk-repository.
Met *git push origin* kan je de aanpassingen sturen naar een repository op een andere locatie.

Als jij je lokale werkbestanden wilt synchroniseren met een bestaande repository op bijvoorbeeld een andere server dan kan dat met *git remote add origin*

# Branching

Branches worden gebruikt om verschillende features los van elkaar te ontwikkelen.

Deze verschillende branches kan je dan uiteindelijk samenvoegen met de master branch (de hoofd branch wanneer je een nieuwe repository maakt) wanneer je klaar bent.

Met *git checkout -b* maak je een nieuwe branch aan.

Met *git checkout master* ga je terug naar de master branch.

Met *git push origin branch* maak je een branch beschikbaar voor anderen door het te synchroniseren met de centrale repository.

# Update & Merge

Met *git pull* update jij je lokale repository naar de laatste versie. Hiermee kan je dus aanpassingen mergen en fetchen met je lokale bestanden.

Met *git merge branch* kan je een andere branch samen voegen met je huidige actieve branch.

Met *git add* kan je de aanpassingen opnieuw toevoegen aan je lokale repository. Dit is soms nodig omdat git de aanpassingen altijd automatisch probeert te mergen en dit gaat soms fout en resulteert dan in een conflict.

# Tagging

Met *git tag 1.0.0 xxxxxxxxxx* maak je een nieuwe tag aan met de naam 1.0.0. xxxxxxxxxx is de commit ID die je in een tag wilt zetten.

De commit ID kan je dan opvragen met *git log*

# Backup

Met *git checkout -- filename* kan je terug naar een vorige versie van een bestand. Dit zal het bestand in je huidige werkmap vervangen door de laatste versie die zich in de HEAD tree bevindt.

Met *git fetch origin* en *git reset --hard origin/master* kan je alle lokale aanpassingen vervangen door de laatste versie van de repository.


