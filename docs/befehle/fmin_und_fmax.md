## fMin und fMax
Die Befehle `fMin` und `fMax` sind besonders nützlich, wenn man eine Funktion in einem Sachkontext untersucht. Dabei ist wichtig, dass diese beiden Befehle in der Regel numerische Näherungen liefern. Die Ergebnisse müssen also mathematisch eingeordnet und überprüft werden. 

Immer dann, wenn mit Hilfe der Ableitungsfunktion und einer Randwertbetrachtung rechnerisch Funktionsmaxima und Funktionsminima herausgefunden werden sollen, sind `fMin` und `fMax` **nicht** geeignet. Wenn aber kein rechnerischer Nachweis verlangt wird, kann man hierfür auch die Funktionen `fMin` und `fMax` benutzen.

## Wofür benutzt man fMin und fMax?

Mit `fMin` bestimmt man näherungsweise die Stelle, an der eine Funktion in einem angegebenen Bereich einen kleinsten Wert annimmt. Mit `fMax` bestimmt man entsprechend näherungsweise die Stelle, an der eine Funktion in einem angegebenen Bereich einen größten Wert annimmt. Dabei untersucht der TI-Nspire nicht automatisch die gesamte Funktion, sondern nur den Bereich, den du selbst angibst. Mathematisch ist dieser Bereich das Intervall, auf dem du die Funktion betrachtest. Deshalb ist es sehr wichtig, sinnvolle Grenzen zu wählen.

Wenn zum Beispiel die Funktion $f(x)=x^2-4x+5$ untersucht werden soll, kann man mit `fMin` herausfinden, an welcher Stelle der Graph im gewählten Intervall seinen tiefsten Punkt hat. 

## Grundform der Befehle

Die allgemeine Eingabe lautet:

``fMin(Funktion, Variable, untere Grenze, obere Grenze)``
``fMax(Funktion, Variable, untere Grenze, obere Grenze)``

Die einzelnen Bestandteile bedeuten:

- ``Funktion``: Hier steht der Funktionsterm oder der Name einer bereits definierten Funktion.
- ``Variable``: Hier gibst du an, nach welcher Variablen gesucht werden soll. In der Schule ist das meistens `x`.
- ``untere Grenze``: Das ist der Rand des Intervalls.
- ``obere Grenze``: Das ist der rechte Rand des Intervalls.

Ein vollständiger Befehl kann also zum Beispiel so aussehen:

<img src="..\..\img\minmax1.png" alt="fMax"/>

Der TI-Nspire sucht dann im Intervall von `-10` bis `10` nach einem Minimum der Funktion.

<img src="..\..\img\minmax2.png" alt="fMax"/>

## Funktion definieren

Es ist oft übersichtlicher, eine Funktion zuerst zu definieren.

<img src="..\..\img\minmax3.png" alt="fMax"/>

Bei längeren Aufgaben kann man so schnell Minima und Maxima bestimmen.

## Wichtig: fMin und fMax liefern zunächst nur den x-Wert

Ein häufiger Fehler besteht darin, das Ergebnis von `fMin` oder `fMax` direkt als Minimum oder Maximum zu interpretieren. Der Befehl liefert zunächst die Stelle, also den x-Wert. Wenn du den y-Wert beziehungsweise Funktionswert brauchst, musst du diesen x-Wert zusätzlich in die Funktion einsetzen. 

<img src="..\..\img\minmax4.png" alt="fMax"/>

In unserem Beispiel liegt das Minimum der Funktion $f(x)=x^2-4x+5$ im Intervall $[-10;10]$ bei $x=2$. Das Minimum hat den y-Wert $f(2)=1$

## Das Intervall richtig wählen und lokale vs. globale Extremstellen

In der Analysis unterscheidet man lokale und globale Extremstellen. Eine lokale Extremstelle ist ein Hoch- oder Tiefpunkt in der näheren Umgebung. Eine globale Extremstelle ist der größte oder kleinste Wert im gesamten betrachteten Bereich. Die Befehle `fMin` und `fMax` untersuchen immer das angegebene Intervall und geben die globale Extremstelle an. Weitere Extremstellen werden ignoriert! Deshalb musst du anschließend überlegen, ob das Ergebnis tatsächlich zur Fragestellung passt.

Wenn die Aufgabe zum Beispiel lautet:

> Bestimme den maximalen Gewinn im Zeitraum von 0 bis 12 Monaten.

Dann ist das Intervall `0` bis `12` durch den Sachzusammenhang vorgegeben. Ein Maximum außerhalb dieses Intervalls wäre für die Aufgabe nicht relevant.

## Typische Fehler

- Ein häufiger Fehler ist ein zu kleines oder falsches Intervall. Wenn das Intervall nicht zur Aufgabe passt, kann der TI-Nspire kein sinnvolles Ergebnis liefern.
- Ein weiterer Fehler besteht darin, den x-Wert mit dem Funktionswert zu verwechseln. `fMin` und `fMax` liefern zunächst die Stelle, nicht den y-Wert.
- Außerdem sollte man beachten, dass der TI-Nspire numerisch arbeitet. Ergebnisse können gerundet sein. Bei exakten mathematischen Untersuchungen, besonders in Klausuren, muss oft zusätzlich mit Ableitungen argumentiert werden.

## Checkliste für fMin und fMax

Bevor du dein Ergebnis aufschreibst, prüfe:

- Habe ich die Funktion richtig eingegeben?
- Habe ich die richtige Variable angegeben?
- Passt das Intervall zur Aufgabe?
- Suche ich ein Minimum oder ein Maximum?
- Habe ich den Funktionswert zusätzlich berechnet?
- Habe ich Randwerte beachtet, falls ein globales Extremum gesucht ist?
- Habe ich das Ergebnis im Sachzusammenhang interpretiert?