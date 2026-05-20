
# Ableitungsfunktion mit dem TI-Nspire

Die Ableitung ist eines der zentralen Werkzeuge der Analysis. Mit ihr kannst du unter anderem:

- Steigungen von Funktionen bestimmen
- Extremstellen berechnen
- Monotonie untersuchen
- reale Probleme modellieren

## Grundidee der Ableitung

Die Ableitung einer Funktion beschreibt die Steigung des Graphen an jeder Stelle.

Für eine Funktion $f(x)$ ist die Ableitung $f'(x)$ eine neue Funktion, die jeder x-Stelle die Steigung zuordnet.
Beispiel:

$$
f(x)=x^2
$$

$$
f'(x)=2x
$$

## Ableitungbefehl

Die grundlegende Syntax lautet:

$$\frac{d}{d \text{Variable}}(\text{Funktion})$$

- ``Funktion``: Hier steht der Funktionsterm oder der Name einer bereits definierten Funktion.
- ``Variable``: Hier gibst du an, nach welcher Variablen abgeleitet werden soll. In der Schule ist das meistens `x`.

Beispiel:

<img src="..\..\img\ableitung1.png" alt="Ableitung"/>

Den Befehl für die Ableitung kann man im CAS entweder über 

``Menü -> Mathematische Operatoren -> Analysis -> 1. Ableitung``

einfügen oder direkt über die Tastatur der APP:

<img src="..\..\img\ableitung3.png" alt="Ableitung"/>
## Ableitungsfunktion 

Meistens möchte man die Ableitungsfunktion weiter untersuchen oder mit dieser rechnen. Daher ist es oft sinnvoll die Ableitungsfunktion für den weiteren gebrauch zu definieren. Grundsätzlich funktioniert das genauso wie das normale Definieren einer Funktion. Siehe dazu auch [Funktion Definieren](funktion_definieren.md).

Am Dreikönigsgymnasium haben wir uns darauf geeinigt, dass Ableitungsfunktionen im CAS, wenn die Funktion ``f(x)`` heißt,  mit ``fs(x)`` bezeichnet werden. Die zweite Ableitung würde dann entsprechend ``fss(x)`` heißen. In manchen Sachkontexten kann es aber auch sinnvoll sein die in den Aufgaben verwendeten Namen zu verwenden. So werden zurückgelegte Strecken oft mit ``s(t)``und deren Ableitung, welche in diesen Sachkontexten die Geschwindigkeit der Bewegen ist, mit ``v(t)``bezeichnet. 

Hier ein paar Beispiele dazu:

<img src="..\..\img\ableitung2.png" alt="Ableitung"/>
