# Tangenten mit dem TI-Nspire

Eine Tangente ist eine Gerade, die den Graphen in einem bestimmten Punkt berührt und dort dieselbe Steigung wie der Graph hat. Sie beschreibt die momentane Änderung an einer Stelle des Graphen.

## Befehl und Syntax

Um eine Tangentengleichung aufzustellen kennst du ein rechnerisches Verfahren, jedoch kann das CAS mit einem einfach Befehl die Tangente an einem Punkt angeben. Dieser Befehl lautet `tagnentLine`

Diesen Befehl findet man unter 

``Menü -> Mathematische Operatoren -> Analysis``

Die Syntax des Befehls lautet  

``tangentLine(Funktion, Variable, Wert``

Alternativ kann man auch  `tangentLine(Funktion, Variable = Wert` verwenden. Man beachte, dass man nur den x-Wert kennen muss um die Tangenten anzulegen.

## Beispiel

Wir betrachten die Funktion $f(x) = x^2$ und wollen eine Tangente an den Punkt $Q(2|4)$ legen. 

<img src="..\..\img\tangente1.png" alt="Tangente"/>

Möchte man mit der Tangentengleichung weiterrechnen, bietet es sich an, dass man diese mit Hilfe des Befehls `tangentLine`definiert. Das funktioniert genauso, wie bei der Ableitungsfunktion oder bei dem Definieren von Funktionen:

<img src="..\..\img\tangente2.png" alt="Tangente"/>
