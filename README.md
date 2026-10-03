# context-embedded

Contexte réutilisable pour apprendre et réaliser des projets en systèmes embarqués.

Objectifs :
- apprendre progressivement l'embarqué avec des projets concrets ;
- garder le code simple, testable et lisible ;
- distinguer clairement électronique, firmware, communications et outillage ;
- réutiliser les contextes spécialisés comme `context-github`, `context-python` ou `context-bash` lorsque nécessaire.

## Structure

```text
context-embedded/
├── AGENTS.md
├── README.md
├── DECISIONS.md
├── docs/
│   ├── learning.md
│   ├── roadmap.md
│   ├── progress.md
│   ├── theory.md
│   ├── conventions.md
│   ├── architecture.md
│   ├── protocols.md
│   ├── hardware-safety.md
│   ├── testing.md
│   └── debugging.md
├── cheatsheets/
│   └── embedded.md
├── projects/
│   └── README.md
└── checklists/
    └── project-completion.md
```

## Deux modes

### Mode apprentissage
Théorie courte → une action pratique → tentative → correction → progression.

### Mode outil
Produire directement une solution embarquée exploitable, expliquer les choix importants et fournir les vérifications utiles.

## Périmètre

Le contexte couvre notamment :
- Arduino et compatible Arduino Core ;
- ESP32 ;
- micro:bit ;
- Raspberry Pi lorsqu'il interagit avec du matériel ;
- GPIO, PWM, ADC ;
- UART, I2C et SPI ;
- capteurs et actionneurs ;
- architecture firmware ;
- consommation et alimentation basse tension ;
- diagnostic matériel/logiciel ;
- tests et validation.

## Contextes complémentaires

- Git/GitHub → `context-github`
- Python → `context-python`
- Bash/Linux tooling → `context-bash`
- sécurité spécialisée → futur `context-security`

Le routeur pourra charger plusieurs contextes pour un même projet.

## Principes

KISS, YAGNI et DRY. Commencer par faire fonctionner le chemin nominal, puis ajouter validation, gestion d'erreur et structure uniquement quand elles apportent une valeur réelle.
