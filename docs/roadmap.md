# Roadmap Embedded

| Étape | Notions | Projet court | Critère |
| --- | --- | --- | --- |
| 1 | tension, courant, GND, GPIO | LED contrôlée | expliquer HIGH/LOW et la masse |
| 2 | entrée numérique, pull-up/pull-down | bouton + LED | lire un bouton sans entrée flottante |
| 3 | millis/time, états | LED non bloquante | éviter un délai bloquant inutile |
| 4 | PWM | variation LED | expliquer duty cycle |
| 5 | ADC | potentiomètre/capteur analogique | lire et convertir une mesure |
| 6 | UART/Serial | console de diagnostic | produire des logs utiles |
| 7 | I2C | lire un capteur | expliquer adresse + SDA/SCL |
| 8 | SPI | périphérique SPI | distinguer MOSI/MISO/SCK/CS |
| 9 | fonctions + modules | structurer un firmware | responsabilités claires |
| 10 | erreurs + timeouts | périphérique absent | ne pas bloquer le système |
| 11 | consommation + alimentation | mesurer une charge | raisonner en V/A/W |
| 12 | stockage ou réseau | configuration simple | gérer les erreurs aux frontières |
| 13 | projet complet | capteur + actionneur + interface | tester nominal + erreurs |

## Règle

Reprendre depuis la première compétence non Validated compatible avec les prérequis.

Un seul exercice ou objectif pratique à la fois.
