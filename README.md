# DYBoard_Feeder

# Projet d'électonique 2022/2023

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

* V1 : 
* V2 : 

## A faire :

- Mise en forme des répertoirs 
- Notice d'assemblage et d'utilisation
- Utiliser les outils de configuration de SiliconLabs
- Ajouter des photos
