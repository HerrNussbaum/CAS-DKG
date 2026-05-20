# Gleichungen lösen: `solve` und `zeros`

Mit der TI-Nspire App gibt es zwei zentrale Befehle, um **Nullstellen und Lösungen von Gleichungen** zu bestimmen:

- `solve` → allgemeines Lösen von Gleichungen  
- `zeros` → Finden von Nullstellen  

`solve` ist dabei der deutlich mächtigere Befehl, weil er allgemein Gleichungen lösen kann, während `zeros` nur Nullstellen von Funktionen berechnen kann. Dennoch ist `zeros` ein nützlicher Befehl, da bei längeren Aufgaben es sich empfiehlt zunächst die Funktion, welche man untersuchen soll, im Taschenrechner zu definieren.

## Der Befehl `solve`

Mit `solve` kannst du **Gleichungen nach einer Variablen auflösen**. Allgemein ist die Syntax hierbei `solve(Gleichung, Variable)`. Hier ein Beispiel:

<img src="..\..\img\solve1.png" alt="solve Beispiel 1"/>

Hier wird die Gleichung $x^2 - 4= 0$ nach der Variable $x$ aufgelöst. Die beiden Lösungen $x_1=-2$ und $x_2 = 2$ der Gleichungen werden direkt rechts angegeben.

`solve` kann nicht nur Gleichungen mit einer Variable lösen. `solve` kann auch Gleichungen in Abhängigkeit von anderen Variablen lösen. Wir nehmen als Beispiel die Gleichung $x^2 - ax + 2= 0$. Dies wollen wir in Abhängigkeit von $a$ lösen.

$$x^2 - ax + 2= 0$$
$$=> x_{1,2} = \frac{a}{2} \pm \sqrt{\frac{a^2}{2^2} - 2}$$
$$=> x_{1} = \frac{a}{2}+ \sqrt{\frac{a^2}{4} - 2}  \quad \lor \quad  x_{2} = \frac{a}{2} - \sqrt{\frac{a^2}{4}- 2} $$
$$=> x_{1} = \frac{a}{2}+ \sqrt{\frac{a^2}{4} - 2}  \quad \lor \quad x_{2} = \frac{a}{2} - \sqrt{\frac{a^2}{4}- 2} $$
$$=> x_{1} = \frac{a + \sqrt{a^2 - 8}}{2}  \quad \lor \quad x_{2} = \frac{a - \sqrt{a^2- 8}}{2}  $$
Wir vergleichen nun mit dem was unser CAS kann:

 <img src="..\..\img\solve2.png" alt="solve Beispiel 2"/>

Wir sehen, dass der CAS zum gleichen Ergebnis kommt, dieses aber ggf. etwas anders aufschreibt.

## Der Befehl `zeros`

Mit `zeros` bestimmst du die **Nullstellen einer Funktion**. Dafür gibst du entweder nur den Funktionsterm oder eine vorher definierte Funktion als erstes Argument an. Im zweiten Argument gibst du die Variable an, von der die Nullstellen bestimmt werden sollen. Hier ein Beispiel, bei dem der Funktionsterm $x^2-4$ angegeben wurde:

<img src="..\..\img\zeros1.png" alt="zeros Beispiel 1"/>

Im folgenden Beispiel wurde vorher die Funktion $f(x)=x^2-4$ mit `f(x):=x^2-4` definiert:

<img src="..\..\img\zeros3.png" alt="solve Beispiel 3"/>

Die Nullstellen werden bei `zeros` als Lösungsmenge angegeben. Dies ist besonders praktisch bei Funktionen, die viele oder sogar unendliche viele Nullstellen haben:

<img src="..\..\img\zeros2.png" alt="solve Beispiel 2"/>

Diese Lösungsmenge muss man folgendermaßen lesen: `n1` bedeutet, dass es eine ganze Zahl ist. Somit hat der Sinus unendliche viele Nullstellen, die ein ganzzahliges Vielfaches von $\pi$ sind.



