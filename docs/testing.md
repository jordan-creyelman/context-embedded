# Tests Embedded

Tester ce qui apporte une vraie valeur.

## Minimum

1. compilation ;
2. démarrage ;
3. cas nominal ;
4. une entrée ou condition invalide importante ;
5. périphérique absent lorsque pertinent.

## Test matériel

Observer :
- Serial ;
- LED de statut ;
- multimètre ;
- oscilloscope/analyseur logique lorsqu'il apporte une vraie information.

## Logique pure

Extraire une fonction pure lorsque cela permet de tester facilement une logique métier importante.

Exemple :
- conversion unité ;
- validation de seuil ;
- machine à états ;
- parsing d'une commande.

Ne pas créer une infrastructure de tests complexe pour un prototype trivial.
