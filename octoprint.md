# GCODE Scripts

## Vor dem Start eines Druckjobs
```gcode
M42 S200; Switch Light ON
````
Befehle, die du hier platzierst, werden vor Zeilen aus deinen Druckdateien gesendet.
## Nach Vollendung eines Druckjobs
```Gcode
G28; home all axis
M42 S0; Switch Light OFF
```
 Befehle, die du hier platzierst, werden nach Zeilen aus deinen Druckdateien gesendet.
## Nach dem Abbruch eines Druckjobs
```Gcode
M84; disable motors


;disable all heaters
{% snippet 'disable_hotends' %}
{% snippet 'disable_bed' %}
;disable fan
M106 S0

````
Befehle, die du hier platzierst, werden nach Zeilen aus deinen Druckdateien gesendet. Falls du jemals das Default-Abbruch-Skript benötigen solltest, mit dem OctoPrint ausgeliefert wird, so kannst du es hier finden.
## Nach dem Pausieren eines Druckjobs
 ```Gcode 
 ```
 Befehle, die du hier platzierst, werden nach Zeilen aus deinen Druckdateien gesendet.

## Vor dem Fortsetzen eines Druckjobs

```Gcode
```
Befehle, die du hier platzierst, werden vor Zeilen aus deinen Druckdateien gesendet.
## Vor Toolwechsel
```Gcode
```
Befehle, die du hier platzierst, werden vor Werkzeugwechselbefehlen Tn gesendet.
## Nach Toolwechsel
```Gcode
```
 Befehle, die du hier platzierst, werden nach Werkzeugwechselbefehlen Tn gesendet.
## Nach Verbindung mit dem Drucker
```Gcode
```
## Bevor die Verbindung zum Drucker geschlossen wird
```Gcode
```
 Das wird nur ausgeführt wenn die Verbindung aktiv geschlossen wird. Falls die Verbindung zum Drucker plötzlich verloren geht wird nichts gesendet.