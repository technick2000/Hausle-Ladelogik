# Hausle-Ladelogik
Ladeelektronik zum Schutz des Akkus

## Problem: 
Ein Solarpanel lädt eine 12V Batterie auf. Das Solarpanel kann jedoch nicht erkennen ob die Batterie voll ist und Versucht so immer weiter zu laden.

## Lösungsidee:
Man misst beim Laden den Ladestrom. Sobald dieser weit genug sinkt wird die Verbindung zwischen Batterie und Solarpanel getrennt. Sobald Die Verbindung getrennt wurde kann die Spannung der Batterie gemessen werden. Sollte diese unter einen bestimmten Wert fallen kann die Verbindung zum Solarpanel wieder hergestellt werden.

## Umsetzung:

- Mikrocontrollern zum Messen sowie Steuern(Waveshare RP2040-Zero)
- 1Ohm 100W widerstände zum Messen des Ladestroms
- Diverse kleine Widerstände zum verkleinern der Spannung damit der Mikrocontroller sie messen kann.
- Kleines Display zum Anzeigen des Ladestroms oder der Batteriespannung. (ssd1306 i2c 0.96" OLED)

