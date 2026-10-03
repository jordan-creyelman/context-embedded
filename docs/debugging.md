# Debugging Embedded

Ordre de diagnostic conseillé :

1. alimentation ;
2. masse ;
3. câblage ;
4. brochage configuré ;
5. firmware réellement flashé ;
6. logs série ;
7. périphérique détecté ;
8. valeurs reçues ;
9. logique applicative.

## Principe

Changer une seule variable à la fois.

## I2C

Si le capteur ne répond pas :
- vérifier VCC/GND ;
- vérifier SDA/SCL ;
- scanner les adresses ;
- vérifier la tension logique ;
- vérifier les pull-ups.

## Firmware

Réduire le problème à un test minimal avant de modifier l'architecture complète.

Diagnostic → hypothèse → test minimal → correction minimale → vérification.
