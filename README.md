# LED-Cube

8x8x8 LED Cube für Arduino Uno Rev3

[![MIT License](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/fuchsalex/Smart-Mirror/blob/master/LICENSE)


## Beschreibung
Ein LED Cube ist eine kubische Anordnung von LEDs. Die Größenordnungen liegen bei 3x3x3 bis über 10x10x10. 
Die Fertigung ist sehr Zeitaufwendig, da die Anschlüsse jeder LED in Form gebracht werden müssen. Desweiteren müssen die Lötarbeiten präzise durchgeführt werden, damit am Schluss der Cube gerade steht.

Die Ansteuerung der 512 LEDs erfolgt über den Arduino.

Die Kathoden werden über ein Darlington-Array auf Masse geschalten.

Die Anoden werden über 8 Schieberegister, die durch Kaskadierung miteinander verbunden sind, auf Vcc geschaltet.

Ein Demo vom fertigen Cube kann [:warning:in Arbeit...] betrachtet werden.

## Dokumentation

:warning: Inhalt in Arbeit...


## Simulation
Der Schaltungsaufbau inklusive Arduino Uno ist in Proteus simuliert. 
Die Simulation ist auf 3 Seiten aufgeteilt:
- [Sheet 1] Platinenaufbau
- [Sheet 2] Analyse der Steuerleitungen
- [Sheet 3] Ansteuerung der 512 LEDs


[Simulation](https://github.com/fuchsalex/LED-Cube/tree/master/Simulation)

## Funktionstest
Um die Funktionalität der einzelnen LEDs zu überprüfen wird das [Testprogramm](https://github.com/fuchsalex/LED-Cube/blob/master/Sourcecode/LED_CUBE_Testprogramm.ino) in den Microcontroller geladen.
Dabei wird jede LED für kurze Dauer beschalten. Sollte hier eine LED nicht leuchten, so liegt entweder ein Fehler in der Platine vor oder die Leuchtdiode ist defekt.

## Programmcode
Ist der Cube auf funktionsfähigkeit geprüft, so kann der [Programmcode](https://github.com/fuchsalex/LED-Cube/blob/master/Sourcecode/LED_CUBE_source.ino) in den Microcontroller geladen werden.

### Autor
![Alexander Fuchs](https://github.com/fuchsalex)

### Lizenz
MIT

### Info
Die Anfertigung eines eigenen LED Cube wurde inspiriert von [ChrisB](http://ledcubeblog.blogspot.co.at/).
