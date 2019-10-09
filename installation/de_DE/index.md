Hardware
========

Jeedom kann auf verschiedenen Hardware-Komponenten installiert werden:

-   ein Raspberry Pi 2 oder 3

-   eine Synology NAS

-   tout système Linux basé sur Debian 9 (stretch)

Sie können auch eine fertige Box mit vorinstalliertem Jeedom kaufen,
die auch ein Service Pack (mehr Unterstützung und Dienste) enthält und 
angebotenen Plugins :

-   [Jeedom Smart
    Z-Wave+](https://www.domadoo.fr/fr/box-domotique/3959-jeedom-controleur-domotique-jeedom-smart-z-wave.html)

-   [Jeedom Smart Z-Wave+ und
    RFXCOM](https://www.domadoo.fr/fr/box-domotique/4043-jeedom-controleur-domotique-jeedom-smart-z-wave-et-interface-rfxcom.html)

-   [Jeedom Smart
    EnOcean](https://www.domadoo.fr/fr/box-domotique/4041-jeedom-controleur-domotique-jeedom-smart-enocean.html)

-   [Jeedom Smart EnOcean und
    RFXCOM](https://www.domadoo.fr/fr/box-domotique/4044-jeedom-controleur-domotique-jeedom-smart-enocean-et-interface-rfxcom.html)

Hier ist ein Konfiguriertes "Beispiel" um gut mit Z-Wave in Jeedom zu starten :

1.  Raspberry Pi 3 :

    -   Ein Raspberry+Gehäuse ~ 50 €

    -   Ein Aeon-Stick Gen5 ~ 60 €

    -   Eine Micro SD Karte ~ 7 €

    -   Eine Stromversorgung über USB ~ 8 €

Insgesamt 125 € für eine Open-Source Haus-Automatisierungs Box mit
vollständiger Kontrolle der Installation.

> **Tipp**
>
> Es ist möglich, eine Rfxcom Antenne oder ein enOcean Schlüssel
> hinzuzufügen oder zu ändern.

> **Tipp**
>
>Jeedom ist eine Software, die Open Source ist und bleibt, ihre Nutzung ist
> völlig kostenlos und hängt nicht von einer Cloud oder einem Abonnement
> ab. Einige Plugins, die die Fähigkeiten von Jeedom oder dessen Nutzung
> erhöhen, können jedoch kostenpflichtig sein **und benötigen
> möglicherweise eine Internetverbindung**. Sie können die Liste der Plugins
> [hier](http://market.jeedom.fr/index.php?v=d&p=market&type=plugin)
> finden.

> **Tipp**
>
> Service pack ? Was bedeutet das ? Sie können 
> [hier](https://blog.jeedom.fr/?p=1215) die Vorteile von Service Packs sehen.


Jeedom Smart
===========

Sie finden hier die Dokumentation Schritt für Schritt, um Jeedom zu installieren oder wiederherzustellen

[Hier](https://jeedom.github.io/documentation/howto/fr_FR/recovery_mode_jeedom_smart)

Jeedom mini+
===========

> **Tipp**
>
> Der Name des heruntergeladenen Jeedom-Abbilds kann sich von dem in
> dieser Dokumentation unterscheiden.

Schritt 1 : Etcher installieren
---

Sie müssen die Etcher Software [hier](https://etcher.io/) herunterladen und auf Ihrem PC installieren.

Schritt 2 : Wiederherstellung Jeedom-Abbild
---

Sie müssen
[hier](https://www.amazon.fr/clouddrive/share/OwYXPEKiIMdsGhkFeI3eUQ0VcvTEBq0qxQevlXPvPIy/folder/IT3WZ3N0RqGzaLBnBo0qog) hin gehen,
dann im Ordner Images das Abbild jeedom-jeeboard-\*.rar oder
Jeedomboard\_\_Debian\_Jessie\*.rar herrunterladen.

![install humming 1](../images/install_humming_1.PNG)

Schritt 3 : Jeedom-Abbild Dekomprimieren
---

Das Jeedom-Abbild dekomprimieren (falls Sie nichts zum dekomprimieren haben können Sie hier [winrar](http://www.clubic.com/telecharger-fiche9632-winrar.html) herunterladen), Sie müssen erhalten : 

![install humming 2](../images/install_humming_2.PNG)

![install humming 8](../images/install_humming_8.PNG)

Schritt 4: Das Abbild auf die SD-Karte brennen
---

Legen Sie Ihre SD-Karte in Ihren Computer ein und starten Sie die Etcher
Software, geben Sie den Pfad des Abbildes, den Pfad der SD-Karte und
klicken Sie auf "Flash!". Die Software wird die SD-Karte brennen und die
Gravur überprüfen.

Sie müssen nur die SD-Karte in das Jeedomboard stecken (oder Hummingboard), das Netzwerk und die Stromversorgung anschließen, Ihr Jeedom wird starten (5 min) und Sie sollen es im Netzwerk sehen.

> **Tipp**
>
> Die SSH Zugangsdaten sind jeedom/Mjeedom96 .

Danach können Sie die Dokumentation [Erste Schritte mit Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index.html) folgen.


Raspberry Pi
===========

Sie finden hier die Dokumentation, um Jeedom auf einem Raspberry PI **mit einer SD-Karte** zu installieren.

> **Important**
>
> Debian 9 (Stretch) est la distribution officiellement supportée pour
> la version 3.1.5 de jeedom.

**1/ Laden Sie das neueste Abbild "lite" herunter, das ist ohne Grafik 
Schnittstelle**
[Hier](https://downloads.raspberrypi.org/raspbian_lite/images/raspbian_lite-2018-04-19/2018-04-18-raspbian-stretch-lite.zip)

**2/ Dekomprimieren Sie das Abbild mit Winrar** [Hier](http://www.win-rar.com)

**3/ Brennen Sie dieses Abbild zum Beispiel mit Etcher auf eine SD-Karte**
[Hier](https://etcher.io/)

> **Notiz**
>
> Wenn Sie Etcher verwenden, um Ihr Abbild zu brennen, ist der
> Dekomprimierungsschritt nutzlos (das Zip-Format wird direkt bei der Auswahl
> der Abbilddatei erkannt).

**4/ Einen SSH-Zugriff aktivieren**

> **Warnung**
>
> Aus Sicherheitsgründen ist der SSH-Zugriff in dieser Distribution nicht mehr
> standardmäßig aktiviert. Er muss daher aktiviert werden.

Es ist notwendig, auf der boot Partition (dem einzigen unter Windows zugänglichen) eine leere Datei ssh zu erstellen.

Nur Rechtsklick : neues / Textdokument und umbenennen in "ssh" **ohne Erweiterung**

> **Wichtig**
>
> Unter Windows müssen Sie im Explorer Ihre Einstellungen 
> in der Ansicht / Optionen /  Ordner- und Suchenoptionen
>  ändern / überprüfen

![ExtensionFichier](../images/ExtensionFichier.PNG)

**5/ PI starten**

Legen Sie Ihre SD-Karte ein, verbinden Sie das Netzwerkkabel und schließen Sie das Netzteil an.

**6/ Sich mit SSH verbinden**

Identifizieren Sie Ihr Pi im Netzwerk

Sie müssen die IP-Adresse Ihres Pi wissen. Es gibt mehrere Lösungen :

-   Sehen Sie sich die DHCP-Konfiguration in Ihrem Router an

-   Verwenden Sie einen Port-Scanner "Angyipscanner"
    [Hier](http://angryip.org/download/#windows)

Stellen Sie die Verbindung her

Verwenden Sie zum Beispiel putty, um Ihre Verbindung herstellen
[Hier](http://www.putty.org/)

Geben Sie die IP-Adresse Ihres PIs ein (hier 192.168.0.10) und klicken Sie auf
Öffnen. Akzeptieren Sie die Standardsicherheitsnachricht für die erste
Anmeldung.

Verbinden Sie sich mit den Anmeldedaten **pi / raspberry**

> **Wichtig**
>
> Aus Sicherheitsgründen muss das Standardkennwort unbedingt geändert
> werden. Hacking-Angriffe, die auf der Verwendung des Standard-Login/
> Passwort-Paares des Raspberry basieren, sind besonders weit verbreitet.
> (passwd und sudo passwd Befehl)                                                                                                                                                                                                               

**7/ Starten Sie das Jeedom Installationsskript**

    wget -O- https://raw.githubusercontent.com/jeedom/core/master/install/install.sh | sudo bash

**Das sudo Passwort ist auch raspberry**

> **Notiz**
>
> Abhängig von Ihrer Internetgeschwindigkeit kann die Installation 45
> bis 90 Minuten dauern. Sie dürfen den Prozess vor dem Ende nicht
> unterbrechen. Andernfalls muss das gesamte Verfahren wiederholt werden.

Sie müssen danach nur noch auf IP\_MACHINE\_JEEDOM gehen

> **Notiz**
>
> Die standard Zugangsdaten sind admin/admin

> **Notiz**
>
> Die folgenden Argumente sind verwendbar: -w = Datei-Webserver -z =
> Abhängigkeiten Installations z-wave -m = gewünschtes mysql root Passwort

    ./install.sh -w /var/www/html -z -m Jeedom

**8/ Systemoptimierung

Wenn Sie Ihren Raspberry für Jeedom ohne angeschlossenen Bildschirm verwenden, wird empfohlen, die Mindestmenge an RAM für den Videoteil zu verwenden.

Melden Sie sich einfach unter **SSH** an und bearbeiten Sie die Konfigurationsdatei : `sudo nano /boot/config.txt`

Hinzufügen **und/oder**den-Kommentar (durch Entfernen von #)**und/oder** ändern der Zeilen :

`gpu_mem=16`

`disable_l2cache=0`

`gpu_freq=250`

Beenden durch Speichern : `CTRL+X` dann `N` dann `ENTER`

Starten Sie den RPI neu

Danach können Sie der Dokumentation [Erste Schritte mit Jeedom]
(https://jeedom.github.io/documentation/premiers-pas/fr_FR/index) folgen.

Freebox Delta
=============

Il est possible d'installer sur Freebox Delta Jeedom via le système de VMs.

Etape 1 : Connexion à la Delta
---

Vous devez vous rendre sur l'interface de configuration de votre Freebox Delta.
Cliquez ensuite sur VMs.
![delta1](../images/delta1.png)

Etape 2 : Paramétrer les différentes options 
---

Cliquez sur "Ajouter une VM"
![delta2](../images/delta2.png)

Configurez les caractéristiques.
Nous vous recommandons de mettre 2 CPUs et le maximum en RAM.
![delta3](../images/delta3.png)

Configurez l'utilisateur et le mot de passe:
![delta4](../images/delta4.png)

Etape 3 : Installation en cours
---

Patientez pendant le téléchargement de l'image
![delta5](../images/delta5.png)

Etape 4 : Connectez-vous à votre Jeedom
---

Vous pouvez vous connecter grâce à l'adresse indiquée sur la page:
![delta6](../images/delta6.png)

Pensez à affecter le port USB de la Delta à la VM si vous souhaitez utiliser une antenne.

l'adresse ip de votre Jeedom sur la Freebox Delta est ecrite en haut, sous son nom.

les login et mot de passe par défaut sont admin/admin. 

Pour la suite, vous pouvez suivre la documentation [Premier pas avec
Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index.html)

VM
==

Si vous voulez découvrir Jeedom sans risque, vous pouvez aussi le
virtualiser sur votre PC, voici la démarche à suivre. Vous ne prenez
aucun risque dans une VM, l’intégrité de votre Pc est protégé :

Etape 1 : Téléchargement et installation de VMware Player 
---

Vous devez télécharger le logicel Virtual Box
[ICI](http://download.virtualbox.org/virtualbox/5.1.28/VirtualBox-5.1.28-117968-Win.exe)

Etape 2 : Téléchargement d’une image Debian strecht - netinstall 
---

Téléchargez une image minimaliste debian 9 Stretch
[Ici](https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/debian-9.3.0-amd64-netinst.iso)

Téléchargez le pack d’extensions, et installez-le.
[ICI](http://download.virtualbox.org/virtualbox/5.1.28/Oracle_VM_VirtualBox_Extension_Pack-5.1.28.vbox-extpack)

Etape 3 : Configuration de l’environnement de la VM 
---

Cliquez sur nouvelle et renseignez les champs comme ci dessous :

![VirtualBox1](../images/VirtualBox1.PNG)

-   Cliquez sur suivant, adapter la taille de la mémoire par rapport à
    votre système (1024 sont suffisants)

-   Cliquez sur suivant, créer un disque virtuel maintenant

-   Cliquez sur Créer, choisissez VDI

-   Cliquez sur suivant, dynamiquement alloué

-   Cliquez sur suivant, Choisissez une taille pour l’espace
    (4Go suffisent)

-   Cliquez sur créer

Etape 4 : Lancement de la VM 
---

-   Cliquez sur configuration

-   Sélectionnez stockage

-   Ajoutez un lecteur optique

-   Choisissez un disque

![VirtualBox2](../images/VirtualBox2.PNG)

-   Indiquez l’image précédemment téléchargée

-   Sélectionnez ensuite réseau et choisissez "accès par pont" dans le mode
    d’accès réseau.

![VirtualBox3](../images/VirtualBox3.PNG)

-   Cliquez sur OK \*Cliquez sur démarrer

Etape 5 : Installation de debian 9 
---

C’est du classique …​

![VirtualBox4](../images/VirtualBox4.PNG)

-   Choisissez Graphical install

-   Installez la debian de préférence sans interface graphique
    car inutile. Le nom d’utilisateur n’a aucune importance. Dans la
    plupart des écrans, il suffit de valider le choix par défaut. Vous
    pouvez laissez des champs vides, ce n’est pas bloquant.

-   Pour la sélection des logiciels :

![VirtualBox5](../images/VirtualBox5.PNG)

-   Pour Grub, pas d’inquiétude, le secteur de démarrage est celui de la
    VM, pas celui de votre PC. Aucun risque de casser quoi que ce soit.

Etape 6 : Installation de jeedom 
---

-   Lancez votre VM

-   Identifiez-vous avec l’utilisateur et le mot de passe choisis
    pendant l’installation

-   Passez en root

<!-- -->

    su

-   Saisissez le mot de passe root défini pendant l’installation

-   Récupérez le script jeedom, le rendre exécutable, le lancer

<!-- -->

    wget https://raw.githubusercontent.com/jeedom/core/master/install/install.sh

    chmod +x install.sh

    ./install.sh

-   et laissez faire…​

Etape 7 : Lancement de jeedom 
---

-   Pour connaitre l’adresse Ip Lan de la VM

<!-- -->

    ip -s -c -h a

Votre adresse Ip, type 192.168.0.XX apparait en rouge. Il vous suffit de
la saisir dans votre navigateur.

> **Warning**
>
> Si cela ne fonctionne pas, vous n’avez pas configuré votre carte
> réseau en Pont réseau comme indiquée au départ.

Ensuite, vous pouvez suivre la documentation [Premier pas avec
Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index)

Docker
======

> **Important**
>
> Attention, nous partons ici du principe que vous maîtrisez déjà Docker

Pour découvrir Jeedom, vous pouvez aussi le faire tourner dans un
conteneur Docker :


Etape 1 : Installation de docker 
---

Docker est maintenant disponible sur toutes les distributions récentes.
Pour l’installer sur une distribution

-   à base de rpm

<!-- -->

    $ yum install docker

-   à base de deb

<!-- -->

    $ apt-get update
    $ apt-get install docker
    $ apt-get install docker.io

Etape 2 : Installation d’une image mysql 
---

> **Note**
>
> Vous pouvez aussi installer mysql directement sur la machine hôte,
> dans ce cas, il faut sauter cette étape.

J’utilise [celle-ci](https://hub.docker.com/_/mysql/). Pour l’installer
:

    docker pull mysql:latest

Puis la lancer :

    sudo docker run --name jeedom-mysql -v /opt/jeedom/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=your-mysql-password -d mysql:latest

Avec :

-   jeedom-mysql : le nom du conteneur mysql

-   /opt/jeedom/mysql : le dossier de l’hote ou l’on doit stoker les
    données de MySql

-   your-mysql-password : le mot de passe root de l’instance MySql

Etape 3 : Installation d’une image Jeedom 
---

Installation de l’image :

    docker pull jeedom/jeedom

Puis lancez la :

    sudo docker run --name jeedom-server --link jeedom-mysql:mysql --privileged -v /your/jeedom/path:/var/www/html -e ROOT_PASSWORD=your-root-password -p 9080:80 -p 9022:22 jeedom/jeedom

Avec :

-   jeedom-server : nom du Docker jeedom voulu

-   /your/jeedom/path : répertoire où les données de Jeedom sont mises
    sur l’hôte

-   your-root-password : mot de passe root pour accéder à Jeedom en SSH

Il vous faut ensuite installer Jeedom en allant sur : IP\_DOCKER:9080 et
entrer les informations de connexion vers mysql :

![install other](../images/install_other.PNG)

Pour la suite, vous pouvez suivre la documentation [Premier pas avec
Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index)

> **Important**
>
> Pour le nom de l’hote MySql, il faut mettre jeedom-mysql

Synology
========

Vous trouverez ici la documentation pas à pas pour installer Jeedom sur un
Synology (DSM 5.2 minimum).

Etape 1 : Installation de Docker 
================================

Allez sur le centre des paquets :

![install synology 1](../images/install_synology_1.PNG)

Cliquez sur tous, puis installez le paquet Docker

![install synology 2](../images/install_synology_2.PNG)

Attendez jusqu’à ce que l’installation soit finie :

![install synology 3](../images/install_synology_3.PNG)

> **Important**
>
> Pour avoir accès au paquet Docker, il faut absolument avoir DSM 5.2 et
> un NAS compatible

Etape 2 : Récupération et installation des images Jeedom 
========================================================

Il faut Docker pour faire tourner Jeedom, le premier un Docker Mysql qui
contiendra la base de données et un 2ème qui contient Jeedom

Lancez l’application Docker :

![install synology 4](../images/install_synology_4.PNG)

MYSQL 
-----

Cliquez sur "Registre" :

![install synology 5](../images/install_synology_5.PNG)

Dans le champ de recherche tapez "mysql", selectionnez mysql et cliquez
sur télécharger :

![install synology 15](../images/install_synology_15.PNG)

Validez ensuite la demande de version, le mieux étant de prendre la
version latest :

![install synology 14](../images/install_synology_14.PNG)

Cliquez ensuite sur image, ici vous pouvez suivre l’avancement du
téléchargement (peut prendre plusieurs dizaines de minutes) :

![install synology 16](../images/install_synology_16.PNG)

Une fois terminé, cliquez sur l’image puis lancer :

![install synology 17](../images/install_synology_17.PNG)

Donnez un nom à votre mysql ainsi qu’un port local redirigé vers le port
3306 du conteneur, puis faites suivant :

![install synology 18](../images/install_synology_18.PNG)

Faites suivant :

![install synology 19](../images/install_synology_19.PNG)

Cliquez sur "Paramètres avancés" :

![install synology 34](../images/install_synology_34.PNG)

Puis sur "Ajouter un dossier", et là, mettez le dossier voulu côté
Synology (c’est dans ce dossier qu’il y aura tous les fichiers de la
base de données) et /var/lib/mysql côté conteneur (attention à bien
décocher "Lecture seule")

![install synology 32](../images/install_synology_32.PNG)

Cliquez sur "Environnement" puis "Ajoutez une variable" et mettant dans
"Variable" : "MYSQL\_ROOT\_PASSWORD" et dans valeur mettez le mot de
passe de BDD voulu (il servira plus tard). Puis validez :

![install synology 33](../images/install_synology_33.PNG)

Cochez "Exécuter ce conteneur lorsque l’assistant a terminé" puis
cliquez sur "Appliquer".

Jeedom 
------

Cliquez sur "Registre" :

![install synology 5](../images/install_synology_5.PNG)

Dans le champ de recherche, tapez "jeedom", sélectionnez jeedom/jeedom
et cliquez sur télécharger :

![install synology 20](../images/install_synology_20.PNG)

Validez ensuite la demande de version, le mieux étant de prendre la
dernière.

Cliquez ensuite sur image, ici vous pouvez suivre l’avancement du
téléchargement (peut prendre plusieurs dizaines de minutes) :

![install synology 21](../images/install_synology_21.PNG)

Une fois terminé, cliquez sur l’image puis lancez :

![install synology 22](../images/install_synology_22.PNG)

Donnez un nom à votre jeedom ainsi qu’un port local redirigé vers le
port 80 (ici 9080) et un vers le 22 (ici 9022) du conteneur, puis faites
suivant :

![install synology 23](../images/install_synology_23.PNG)

Faites suivant :

![install synology 24](../images/install_synology_24.PNG)

Cliquez sur "Paramètres avancés"

![install synology 25](../images/install_synology_25.PNG)

Puis sur "Ajouter un dossier"

![install synology 26](../images/install_synology_26.PNG)

Choisissez un dossier sur votre Synology (c’est dans ce dossier qu’il y
aura tous les fichiers jeedom), attention à bien décocher "Lecture
seule"

![install synology 27](../images/install_synology_27.PNG)

Dans chemin d’accès, mettez /var/www/html puis cliquez sur
"Environnement" :

![install synology 28](../images/install_synology_28.PNG)

Cochez "Exécuter le conteneur à l’aide de privilèges élevés" puis
validez le tout :

![install synology 29](../images/install_synology_29.PNG)

Cochez "Exécuter ce conteneur lorsque l’assistant a terminé" puis
cliquez sur "Appliquer".

> **Paramètre de configuration avancé**
>
> Il existe 3 paramètres optionnel de configuration, ces paramètres doivent etre passé en variable d'environement
> - APACHE_PORT : permet de changer le port par défaut (80) d'écoute du serveur web
> - SSH_PORT : permet de changer le port par défaut (22) d'écoute du ssh
> - MODE_HOST : indique que le résaux est en mode host

> **IMPORTANT**
>
> Certain plugin on besoin d'avoir le broadcast du réseaux (type plugin Xioami), pour cela il faut ABSOLUMENT passer en le réseaux en mode host (possible uniquement lors de la création), changer le port d'écoute par defaut du serveur web et ssh par des ports non utilisé (type 9080 pour le serveur web et 9022 pour le ssh), et mettre la variable MODE_HOST à 1

Etape 3 : Configuration de Jeedom 
---

Il vous faut maintenant installer Jeedom, c’est très simple, allez sur
IP\_NAS:9080

![install synology 31](../images/install_synology_31.PNG)

Remplissez les champs en fonction de votre configuration (configuration
du Docker mysql installé précédemment) et validez.

> **Important**
>
> L’addresse IP de la BDD est l’addresse IP du NAS, le port est celui
> redirigé du Docker Mysql, le mot de passe est celui mis dans le Docker
> Mysql. Le nom d’utilisateur est root et le nom de la base celui que
> vous voulez (conseillé Jeedom)

![install synology 30](../images/install_synology_30.PNG)

> **Tip**
>
> Si vous voulez un accès SSH, il vous faut dans les ports rediriger un
> port local vers le port 22 du conteneur, les identifiants SSH sont
> root/jeedom. Vous pouvez changer le mot de passe en initialisant la
> variable d’environement ROOT\_PASSWORD à la valeur du mot de passe
> voulu.

Ensuite, vous pouvez suivre la documentation [Premier pas avec
Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index)

Autres
======

Vous trouverez ici la documentation pour installer Jeedom sur la plupart
des systèmes linux (testée et approuvée sur la distribution Debian)

> **Important**
>
> Debian 9 (Stretch) est la distribution officiellement supportée pour
> la version 3.1.7 de Jeedom (mais Jessie reste parfaitement
> fonctionnelle). Si vous ne maîtrisez pas un minimum les environnements
> Linux, nous vous conseillons de partir sur une image officielle (OVF)
> ou l’utilisation d’une Mini+ ou Smart (disponible prochainement).

> **Important**
>
> Le script d’installation peut être dangereux, car il part du principe
> que votre système est vierge. Si ce n’est pas le cas merci de lire le
> script et de faire une installation à la main.

Connectez-vous en SSH à votre système et faites :

    wget https://raw.githubusercontent.com/jeedom/core/master/install/install.sh
    chmod +x install.sh
    ./install.sh

Il vous suffit ensuite d’aller sur IP\_MACHINE\_JEEDOM à partir de votre
navigateur Internet.

> **Note**
>
> Les identifiants par défaut sont admin/admin

> **Note**
>
> Les arguments suivants sont utilisables : -w = dossier webserver -z =
> installation dependances z-wave -m = mot de passe root mysql désiré

    ./install.sh -w /var/www/html -z -m Jeedom

Ensuite, vous pouvez suivre la documentation [Premier pas avec
Jeedom](https://jeedom.github.io/documentation/premiers-pas/fr_FR/index).
