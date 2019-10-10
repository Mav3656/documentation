Hardware
========

Hardware | Zustand | Bemerkungen
--- | --- | ---
Jeedomboard             | Stabil                  |
Hummingboard            | Stabil                  |
Odroid C2               | Stabil                  |                          
Smart                   | Stabil                  |                          
RPI1                    | Stabil                  |                          
RPI2                    | nicht offiziell/Stabil     |                          
RPI3                    | nicht offiziell/Stabil     | Achtung, wenn Sie eine Razberry verwenden, funktioniert das WLAN/Bluetooth nicht.
64 Bits                 | Stabil                  |                          
32 Bits                 | Nicht unterstützt            |                          
Vmware                  | Stabil                  | Keine Unterstützung für VMware, nur für Jeedom. Achtung, VmWare 6.5 erfordert die Installation eines VMWare-Patches für die Unterstützung von Zwave.

Images
======

Vous pouvez retrouver toutes les images Jeedom
[ici](https://images.jeedom.com/),
puis dans le dossier Images

> **Notiz**
>
> Ein Netinstall-Image wird nach dem ersten Start die neueste stabile 
> Version von Jeedom installieren, dieser Start dauert etwas länger und Sie
> müssen auf das Internet zugreifen können. Sie können den Fortschritt
> verfolgen, indem Sie die IP-Adresse Ihres Jeedom in Ihrem Browser
> eingeben.

| Abbilder         | Hardware       | Zustand           | SSH Zugriff      | Bemerkungen      |
|----------------|----------------|----------------|----------------|----------------|
| Jeedomboard    | Jeedomboard und | Beta           | root/Mjeedom96 |                |
| netinstall     | hummingboard   |                |                |                |
| Jeedomboard    | Jeedomboard und | Stabil         | root/Mjeedom96 |                |
|                | Hummingboard   |                |                |                |
| Docker         |                | Beta           | root/Mjeedom96 |                |


Alle anderen zuvor herunterladbaren Bilder werden nicht länger gepflegt,
es ist besser, die manuelle Installation von Jeedom
[Doc](https://github.com/jeedom/documentation/blob/master/installation/fr_FR/other.asciidoc)
nach der Installation einer Linux-Distribution zu durchlaufen, die Ihrer
Hardware entspricht : Debian (vm, pc,…​), Raspbian Lite (Raspberry pi),
Armbian (Ordoid,…​), …​

Logiciel
========

> **Wichtig**
>
> Jeedom unterstützt nur Debian Jessie (stabil) und Stretch (stabil). Eine
> andere Version (Wheezy...) oder Distribution (Ubuntu...) wird von Jeedom
> nicht unterstützt.


| Name                     | Zustand                    | Bemerkungen                |
|-------------------------|-------------------------|--------------------------|
| PHP 5.5 oder weniger        | Nicht unterstützt            |                          |
| PHP 5.6                 | Stabil                  |                          |
| PHP 7.X                 | Stabil                  |                          |
| Mysql 5.5/5.6           | Stabil                  |                          |
| Mysql 5.7               | Beta                    |                          |
| MariaBD                 | Stable                  |                          |

Andere
=====

Clef USB/Module d’extension
---------------------------

ENOCEAN Controller :

-   USB-Stick EnOcean USB300
-   USB-Stick EnOcean USB310 (Empfohlen)

RFXCOM  Schnittstelle :

-   RFXtrx433 USB
-   RFXtrx433E USB (Empfohlen)

EDISIO Gateway :

-   Edisio Dongle (Empfohlen)

LED-Anzeige :

-   blink(1) mk2 (Empfohlen)

GSM Dongle :

-   HUAWEI E220 (Empfohlen)
-   Alcatel one touch X220L
-   HSDPA 7.2MBPS 3G Wireless

Z-Wave Controller :

-   SIGMA DESIGNS Z-Wave Controller Plus USB
-   Z-WAVE.ME - Mini Controller USB Z-Wave Plus UZB1
-   AEON LABS Z-Wave Controller Aeon Labs Z-Stick S2
-   AEON LABS - USB Controller Z-Wave Plus Z-Stick GEN5 (Empfohlen)


Contrôleur Zigbee :

- [Phoscon Conbee I/II](http://bit.ly/2n4VyWc)

Modules Zwave
-------------

Vous trouverez la liste
[ici](https://jeedom.github.io/documentation/zwave/fr_FR/equipement.compatible)

Modules EnOcean
---------------

Vous trouverez la liste
[ici](https://jeedom.github.io/documentation/enocean/fr_FR/equipement.compatible)

Modules Edisio
--------------

Vous trouverez la liste
[ici](https://jeedom.github.io/documentation/edisio/fr_FR/equipement.compatible)

Modules RFXcom
--------------

Vous trouverez la liste
[ici](https://jeedom.github.io/documentation/rfxcom/fr_FR/equipement.compatible)

Caméras
-------

Vous trouverez la liste
[ici](https://jeedom.github.io/documentation/camera/fr_FR/equipement.compatible)

Plateforme matérielle recommandée
---------------------------------

L’équipe jeedom vous recommande (en fonction de votre budget) :

-   Jeedom Smart (tout est préinstallé, vous n’avez rien à faire)

-   Odroid C2 (meilleur rapport performance/prix)

-   Intel Nuc gen6 (des performances extrêmes, voir la catégorie tuto
    pour le choix dans les differents modèles et l’installation)
