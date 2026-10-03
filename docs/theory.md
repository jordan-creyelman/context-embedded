# Théorie Embedded — référence courte

## Électricité

Tension : différence de potentiel, en volts (V).

Courant : débit de charge électrique, en ampères (A).

Puissance :

```text
P = U × I
```

Loi d'Ohm :

```text
U = R × I
```

## GPIO

Une broche numérique peut généralement être configurée comme entrée ou sortie.

Ne jamais connecter une tension supérieure à celle tolérée par le GPIO.

## Pull-up / pull-down

Une entrée laissée flottante peut produire des valeurs instables.

Une résistance de pull-up force un état par défaut HIGH.
Une résistance de pull-down force un état par défaut LOW.

## PWM

Le PWM commute rapidement une sortie. Le duty cycle représente la proportion du temps passé à l'état actif.

## ADC

Un ADC convertit une tension analogique en valeur numérique. La résolution dépend du microcontrôleur et de sa configuration.

## UART

Communication série point à point, typiquement TX/RX + GND.

Les paramètres des deux côtés doivent être compatibles, notamment le baud rate.

## I2C

Bus utilisant généralement :
- SDA : données ;
- SCL : horloge.

Plusieurs périphériques peuvent partager le bus grâce à leurs adresses.

## SPI

Bus généralement composé de :
- SCK ;
- MOSI ;
- MISO ;
- CS par périphérique.

SPI est souvent plus rapide qu'I2C mais utilise davantage de lignes.

## Boucle non bloquante

Un firmware réactif évite de bloquer longtemps la boucle principale.

Préférer une logique basée sur le temps écoulé ou des états lorsqu'il faut gérer plusieurs comportements simultanément.
