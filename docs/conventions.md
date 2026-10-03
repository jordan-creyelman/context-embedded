# Conventions Embedded

## Nommage

Utiliser des noms explicites en anglais.

```cpp
constexpr uint8_t STATUS_LED_PIN = 2;
constexpr unsigned long SENSOR_INTERVAL_MS = 1000;
```

Toujours inclure l'unité dans le nom lorsque cela évite une ambiguïté.

## Fonctions

Une fonction = une responsabilité utile.

```cpp
void updateStatusLed();
bool readTemperature(float& temperatureC);
```

## Constantes

Éviter les nombres magiques. Centraliser les broches, délais, seuils et paramètres de protocole.

## Erreurs

Ne pas ignorer silencieusement un échec de capteur, de bus, de stockage ou de réseau.

Les logs doivent permettre de comprendre :
- ce qui a échoué ;
- à quel endroit ;
- avec quelle valeur ou quel état pertinent.

## Boucle principale

Garder `loop()` lisible.

Exemple :

```cpp
void loop() {
  updateInputs();
  updateApplication();
  updateOutputs();
}
```

Ne pas imposer cette structure à un programme trivial.

## Interruptions

Une ISR doit être courte. Éviter les opérations lentes, allocations, logs complexes ou logique métier lourde dans une interruption.

## Dépendances

Ajouter une bibliothèque uniquement si elle évite une complexité réelle ou fournit une implémentation fiable difficile à reproduire correctement.
