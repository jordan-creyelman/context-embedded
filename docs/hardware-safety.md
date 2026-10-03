# Sécurité matérielle

## Avant d'alimenter

Vérifier :
- tension d'alimentation ;
- polarité ;
- brochage ;
- masse ;
- consommation attendue ;
- tension logique des GPIO.

## GPIO

Un GPIO n'est pas une alimentation de puissance.

Ne pas piloter directement :
- moteur ;
- relais de puissance ;
- ruban LED ;
- charge inductive importante.

Utiliser un driver adapté.

## Court-circuit

Avant de mettre sous tension un montage nouveau :
- inspection visuelle ;
- continuité si nécessaire ;
- alimentation limitée en courant lorsqu'elle est disponible.

## Batterie

Respecter le type de cellule, la tension maximale, le courant de charge et le circuit de protection requis.

## Limite du contexte

Les exercices restent en basse tension. Les travaux sur le secteur nécessitent des procédures, équipements et compétences spécifiques et ne font pas partie des exercices de base.
