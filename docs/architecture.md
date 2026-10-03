# Architecture firmware

Commencer simple.

## Niveau 1 — fichier unique

Adapté à :
- LED ;
- bouton ;
- capteur simple ;
- petit prototype.

## Niveau 2 — responsabilités séparées

Quand le projet grandit :

```text
src/
├── main.cpp
├── sensors.cpp
├── sensors.h
├── actuators.cpp
└── actuators.h
```

`main.cpp` orchestre ; les modules encapsulent les responsabilités matérielles.

## Niveau 3 — domaine + adapters

Seulement pour un projet réellement complexe :

```text
domain/
application/
drivers/
infrastructure/
```

Le domaine ne doit pas dépendre directement du GPIO ou d'une bibliothèque réseau lorsque cette séparation apporte une vraie testabilité.

## Règle

Ne jamais appliquer Clean Architecture mécaniquement à un firmware de 50 lignes.
