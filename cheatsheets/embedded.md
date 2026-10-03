# Cheat sheet Embedded

## Loi d'Ohm

```text
U = R × I
I = U / R
R = U / I
```

## Puissance

```text
P = U × I
```

## Bus

| Bus | Signaux principaux | Usage |
| --- | --- | --- |
| UART | TX, RX | série point à point |
| I2C | SDA, SCL | plusieurs petits périphériques |
| SPI | SCK, MOSI, MISO, CS | débit élevé |

## Debug

```text
power → ground → wiring → pin config → protocol → data → application
```

## Rappels

- vérifier les niveaux logiques ;
- nommer les unités ;
- éviter les delays bloquants lorsque plusieurs tâches coexistent ;
- mesurer avant de supposer ;
- ne jamais ignorer une valeur de retour importante.
