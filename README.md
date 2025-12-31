# Minitel1B_Hard
Minitel Library for Arduino (with HardwareSerial)

This is a fork of the original [iodeo](https://github.com/iodeo/Minitel1B_Hard) library made compatible with platform.io registry.

## Connection
* n.c. means **not connected**

| DIN pin | Board | Minitel |
|---------|-------|---------|
| 1       | RX    | TX      |
| 2       | GND   | GND     |
| 3       | TX    | DX      |
| 4       | n.c.  | n.c.    |
| 5       | n.c.  | n.c     |

The TX output on the Minitel side is open-collector, it therefore requires a pull-up resistor R.

I use R = 10 kilohms (a value within the 2.3 to 200 kilohm range indicated in the technical documentation, p.69).

I obtain the +5V through the DIN 5 pin (+8.5V), on which I connect a 5V regulator.

## Documentation:
 * [Technical Specifications](http://543210.free.fr/TV/stum1b.pdf) for Using the Minitel 1B

## Credits
* [iodeo](https://github.com/iodeo) for the original library

## Todo
* Translate everything to English
* Make some adjustement if needed

