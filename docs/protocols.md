# Protocoles embarqués

## UART

Bon pour :
- console ;
- GPS ;
- modules série ;
- diagnostic.

Vérifier TX ↔ RX, GND commun et niveaux logiques.

## I2C

Bon pour :
- capteurs ;
- RTC ;
- petits écrans.

Vérifier :
- adresse ;
- pull-ups ;
- tension logique ;
- longueur/qualité du bus.

## SPI

Bon pour :
- écrans ;
- cartes SD ;
- ADC/DAC rapides ;
- périphériques nécessitant davantage de débit.

Chaque périphérique utilise généralement son propre CS.

## Choix rapide

- simplicité + plusieurs petits capteurs → I2C ;
- débit plus élevé → SPI ;
- point à point / debug → UART.

Choisir selon le besoin réel, pas selon la sophistication du protocole.
