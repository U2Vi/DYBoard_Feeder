# DYBoard_Feeder

# Projet d'électronique 2022/2023

Dans ce réertoir, vous trouverez :
- Fichiers de CAO en électronique sous Altium. 
- Schémas en PDF, notes d'assemblage, de fabrication et tout documents utiles.
- Des photos. 
- Programmes pour les microcontrôleurs des cartes. 

## Contexte 

* Généralités :  
DYBoard est un projet de conception de cartes électroniques modulaires pour la recherche scientifique (et autre). 
Les cartes DYBoard peuvent être connectées entre elles pour créer des systèmes polyvalents et complexes. 
Chaque type de carte à une/des fonction/s spécifique/s. 
Les cartes DYBoard sont conçues pour être compatibles entre elles, ce qui permet de les assembler selon les besoins spécifiques de chaque projet. 
Les cartes DYBoard sont des solutions modulaires pour les personnes qui cherchent à réaliser des projets complexes ayant des besoins en électronique et programmation de microcontrôleurs. 
L'objectif de DYBoard est de pouvoir facilement créer des prototypes personnalisés et modulaires pour la recherche scientifique (ou des projets d'ingénierie).


## Spécifications

* Les cartes "Feeder" sont des interfaces de communication série vers des microcontrôleurs ou d'autres systèmes embarqués.
Elles embarques un UDCC (Universal Device Communication Controller) et communique via une interface UART (Universal Asynchronous Receiver-Transmitter).
Elles sont conçues pour téléverser des programmes sur les séries de microcontrolleurs ESP32 (Mais peuvent trés bien fonctionner pour d'autres µC). 

L'utilisation des broches TXD, RXD, RTS et DTR permettent de mettre les ESP-32 automatiquement en mode téléversement de programme. (TXD > RX / RXD > TX / RS > EN / GPIO0 > GPIO0).

## Exemple(s) d'utilisation : 

* Utilisation de l'IDE arduino (V1 et/ou V2) pour téléverser automatiquement des programmes vers des microcontrolleurs ESP-32 (WROOM-32E / WROOM-32UE / WROOM-32D / S3-WROOM / etc ...)

## Versionement :

* V1 du 04/2022 [4065-V1.0.SD] : 
  - Connectique côté PC : Micro USB type B. 
  - Connectique côté cartes : Connecteur molex type 052207-0633 (pour nappe type 015167-0212). 
  - INTERFACE-FT232RL de FTDI.
  - Selecteur Vout 5V ou 3.3V
  - Sélecteur d'état haut des broches de communication 5V ou 3.3V
  - Voyants RX/TX.
  
 [ OK ] Carte testée et fonctionnelle.
 
* V2 du 12/2022 [2517-V2.0.21.SD] : 
  - Connectique côté PC : USB Type C.  
  - Connectique côté cartes : 
    -> Connecteur molex type 052207-0633 (pour nappe type 015167-0212).
    -> Pads pour assemblage carte à carte (brasure). 
    -> Pads pour assemblage par fils. 
  - INTERFACE-CP2102N-A02-GQFN24R de Silicon Labs.
  - Selecteur Vout 5V ou 3.3V
  - Suppression du sélecteur d'état haut des broches de communication 5V ou 3.3V. Etats haut des E/S fixées à 3.3V.
  - Ajout de protections anti-ESD 
  - Ajout d'une protection par fusible (63V 1A).
  - Pour les voyants RX/TX, nécéssite d'être configuré par le logiciel "Xpress Configurator" de Silicon Labs. 

[ /!\ ] Carte testée, D+ et D- inversés au niveau du connecteur USB-C et composants CMS trop petits pour assemblage manuel, design à refaire (aprés correction, le reste est fonctionnelle).

## A faire :

- Notice d'assemblage et d'utilisation
- Utiliser les outils de configuration de SiliconLabs
- Ajouter des photos
- Ajouter empreinte carte à carte Althium
- Add liens PCBWAY
