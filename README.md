# Installasjon og Oppsett av Raspberry Pi, Ubuntu og Python


## Update og Upgrade av Ubuntu
1.	Når du er inni ubuntu opne Terminalen via CTRL + ALT + T.

2.	Skriv inn ``    Sudo apt update``  og put inn passored ditt. Vent til den er ferdig.

3.	Dersom den er ferdig med å oppdatere kommer det til å komme opp en melding om å restarte. Klikk ``Restart Now``, Og logg inn på nytt når den har restartet.

4.	Når du er tilbake inn og er i Terminalen skal du da skrive inn ``Sudo apt upgrade`` og vent til den er ferdig. Det gjør at du updater og upgrader alle programmer på Rasberry Pi’en.  

## Sette opp SSH og Brannmur på Ubuntu

1. Opne Terminalen via CTRL + ALT + T

2. Skriv inn ``Sudo apt install ufw``  Skriv inn passordet dersom det kommer opp. også vent til den er ferdig

3. Skriv in ``Sudo ufw enable`` Dette vil aktivere brannmuren ved oppstart.

4. Skriv in ``Sudo ufw allow ssh`` dette tillater SSH tilkoblinger.

5. Sjekk statusen på brannmuren via ``Sudo ufw status``

## Skru på SSH

1. Skriv in ``Sudo apt install openssh-server`` Dersom det kommer opp [y/n] skriv in ``Yes eller y`` Dette installerer SSH-serveren.

2. Skriv in ``Sudo systemctl enable ssh`` Dette gjør at SSH slår på ved oppstart.

3. Skriv in ``Sudo systemctl start ssh`` Dette vil starte opp SSH med en gang.

## Finne IP addresse

1. Skriv inn ``ip a`` på Inet nr: 2. finner du et adresse som ligner på ``10.x.x.xx`` X= nummeret. Dette vil da være IP adresse til serveren. Du vil trenge IP adresse ditt for å bruke SSH.





