# Projets Embedded

Les projets servent la roadmap. Commencer petit puis enrichir.

## 1. LED + bouton

Compétences :
- GPIO ;
- résistance ;
- entrée avec pull-up/pull-down.

Objectif : contrôler une LED avec un bouton sans entrée flottante.

## 2. LED non bloquante

Compétences :
- temps ;
- états ;
- boucle principale.

Objectif : faire clignoter une LED sans bloquer le reste du programme.

## 3. Potentiomètre → PWM

Compétences :
- ADC ;
- mapping ;
- PWM.

Objectif : régler la luminosité d'une LED avec un potentiomètre.

## 4. Capteur I2C

Compétences :
- I2C ;
- détection ;
- erreurs.

Objectif : détecter le périphérique, lire une mesure et gérer son absence.

## 5. Station de mesure

Compétences :
- capteur ;
- affichage ou Serial ;
- états ;
- erreurs ;
- architecture simple.

Objectif : produire une mesure périodique fiable et diagnostiquable.

## 6. Projet ESP32 connecté

Compétences :
- Wi-Fi ;
- configuration ;
- timeout ;
- séparation matériel/réseau.

Objectif : publier une mesure sans bloquer le fonctionnement local si le réseau tombe.

## Définition d'un projet terminé

- besoin clair ;
- schéma/câblage documenté ;
- broches et tensions connues ;
- firmware lisible ;
- erreurs importantes gérées ;
- cas nominal vérifié ;
- une panne pertinente testée ;
- aucun secret versionné.
