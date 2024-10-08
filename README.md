# Installasjon og Oppsett av Raspberry Pi, Ubuntu og Python


## innholdsfortegnelse


1. [Update og IUpgrade av Ubuntu](#update-og-upgrade-av-ubuntu)
2. [Sette opp SSH og Brannmur på Ubuntu](#sette-opp-ssh-og-brannmur-på-ubuntu)
3. [Skru på SSH](#skru-på-ssh)
4. [Finne IP adresse](#finne-ip-addresse)
5. [Laste Python, Git, Mariadb og sql](#laste-python-git-mariadb-og-sql)


## 1. Update og Upgrade av Ubuntu
1.	Når du er inni ubuntu opne Terminalen via ``CTRL + ALT + T``

2.	Skriv inn ``sudo apt update``  og put inn passored ditt. Vent til den er ferdig.

3.	Dersom den er ferdig med å oppdatere kommer det til å komme opp en melding om å restarte. Klikk ``Restart Now``, Og logg inn på nytt når den har restartet.

4.	Når du er tilbake inn og er i Terminalen skal du da skrive inn ``sudo apt upgrade`` og vent til den er ferdig. Det gjør at du updater og upgrader alle programmer på Rasberry Pi’en.  

## Sette opp SSH og Brannmur på Ubuntu


1. Opne Terminalen via ``CTRL + ALT + T``

 ```bash
 sudo apt install ufw 
 sudo ufw enable 
 sudo ufw allow ssh
```
Skiv in passordet dersom det kommer opp. også vent til den er ferdig

Dette vil aktivere brannmuren ved oppstart og tillate SSH tilkoblinger.

2. Sjekk statusen på brannmuren via ``sudo ufw status``

## Skru på SSH
1. 
```bash
sudo apt install openssh-server
```
Dersom det kommer opp [y/n] skriv in ``Yes eller y`` Dette installerer SSH-serveren.

2. 
```bash
sudo systemctl enable ssh 
sudo systemctl start ssh
```
Dette gjør at SSH slår på ved oppstart og starter opp SSH med en gang.

## Finne IP addresse

1. Skriv inn ``ip a``.

2. på "Inet" nr: 2. finner du et adresse som ligner på ``10.x.x.xx`` X= IP adresse.

 Du vil trenge IP adresse ditt for å bruke SSH.


## Laste Python, Git, Mariadb og sql
1. Dette vil laste ned alt.
```bash
sudo apt install python3-pip

sudo apt install git

sudo apt install mariadb-server

sudo mysql_secure_installation
```
Skriv inn Y/Yes på alle installasjoner dersom det kommer opp "Do you want to contuinue".

For sql skal du skrive inn ``N/No`` på alle.
