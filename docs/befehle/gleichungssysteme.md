# Gleichungssysteme mit dem TI-Nspire lösen

Diese Anleitung erklärt, wie du Gleichungssysteme mit dem TI-Nspire löst, kontrollierst und interpretierst. Sie richtet sich an Schülerinnen und Schüler der EF, Q1 und Q2 und orientiert sich an den Anforderungen des Kernlehrplans NRW.

Gleichungssysteme treten in vielen Bereichen der Mathematik auf. In der EF begegnen sie häufig bei linearen Funktionen und Schnittpunkten von Geraden. In der Q1 und Q2 werden sie unter anderem verwendet, um Schnittpunkte von Graphen, Parameterwerte, Extrembedingungen oder Modellierungsaufgaben zu bestimmen.

!!! Voraussetzung

    Du solltest wissen, was eine Gleichung ist, wie man Variablen verwendet und wie man einfache Gleichungen nach einer Variablen löst.

## Grundidee

Ein Gleichungssystem besteht aus mehreren Gleichungen, die gleichzeitig erfüllt sein müssen.

Ein einfaches lineares Gleichungssystem ist zum Beispiel:

$$
\begin{aligned}
2x+y&=5 \\
x-y&=1
\end{aligned}
$$

Gesucht sind Werte für \(x\) und \(y\), die beide Gleichungen gleichzeitig wahr machen.

In diesem Beispiel ist die Lösung:

$$
x=2,\quad y=1
$$

Denn:

$$
2\cdot 2+1=5
$$

und:

$$
2-1=1
$$

## Wichtige TI-Nspire-Befehle

Für Gleichungssysteme sind vor allem diese Befehle wichtig:

```text
solve(...)
```

und bei numerischen Lösungen:

```text
nSolve(...)
```

In vielen schulischen Kontexten reicht `solve`, besonders bei linearen Gleichungssystemen und einfachen symbolisch lösbaren Gleichungen.

Außerdem kann man Gleichungssysteme grafisch lösen, indem man die Graphen zeichnet und Schnittpunkte bestimmt.

## Gleichungssysteme mit solve lösen

Die Grundform lautet:

```text
solve({Gleichung1, Gleichung2}, {Variable1, Variable2})
```

Die geschweiften Klammern sind wichtig. Sie zeigen dem TI-Nspire, dass mehrere Gleichungen und mehrere Variablen zusammengehören.

### Beispiel

Gegeben ist:

$$
\begin{aligned}
2x+y&=5 \\
x-y&=1
\end{aligned}
$$

Im TI-Nspire gibst du ein:

```text
solve({2x + y = 5, x - y = 1}, {x, y})
```

Das Ergebnis lautet:

```text
x = 2 and y = 1
```

oder in einer ähnlichen Darstellung:

```text
{x = 2, y = 1}
```

Je nach App-Version und Einstellungen kann die Darstellung leicht abweichen. Inhaltlich bedeutet das: Das Gleichungssystem hat die Lösung \(x=2\), \(y=1\).

## Eingabe Schritt für Schritt

Öffne eine Calculator-Seite.

Gib den Befehl ein:

```text
solve(
```

Dann öffnest du eine geschweifte Klammer für die Gleichungen:

```text
{
```

Trage die erste Gleichung ein:

```text
2x + y = 5
```

Setze ein Komma und trage die zweite Gleichung ein:

```text
x - y = 1
```

Schließe die geschweifte Klammer:

```text
}
```

Setze ein Komma und öffne eine zweite geschweifte Klammer für die Variablen:

```text
{x, y}
```

Der vollständige Ausdruck lautet:

```text
solve({2x + y = 5, x - y = 1}, {x, y})
```

Bestätige mit Enter.

!!! Achtung

    Zwischen den Gleichungen und zwischen den Variablen müssen Kommas stehen. Außerdem müssen die Gleichungen und die Variablen jeweils in geschweiften Klammern stehen.

## Gleichheitszeichen richtig verwenden

Beim Lösen von Gleichungen brauchst du ein echtes Gleichheitszeichen:

```text
=
```

Das ist hier richtig:

```text
2x + y = 5
```

Nicht gemeint ist eine Funktionsdefinition mit `:=`.

Das Zeichen `:=` verwendet man zum Definieren von Funktionen oder Variablen, zum Beispiel:

```text
f(x) := 2x + 1
```

Beim Lösen eines Gleichungssystems geht es aber um Bedingungen, die erfüllt sein sollen. Deshalb verwendet man dort `=`.

## Kontrolle der Lösung

Eine Lösung sollte immer überprüft werden. Setze die Werte in beide Gleichungen ein.

Für \(x=2\) und \(y=1\):

Erste Gleichung:

$$
2x+y=5
$$

$$
2\cdot 2+1=5
$$

$$
5=5
$$

Zweite Gleichung:

$$
x-y=1
$$

$$
2-1=1
$$

$$
1=1
$$

Beide Gleichungen sind erfüllt. Die Lösung ist also korrekt.

## Mehr als zwei Gleichungen

Der TI-Nspire kann auch Gleichungssysteme mit mehr als zwei Variablen lösen.

Beispiel:

$$
\begin{aligned}
x+y+z&=6 \\
2x-y+z&=3 \\
x+2y-z&=2
\end{aligned}
$$

Eingabe:

```text
solve({x + y + z = 6, 2x - y + z = 3, x + 2y - z = 2}, {x, y, z})
```

Der TI-Nspire gibt dann Werte für \(x\), \(y\) und \(z\) aus, sofern das Gleichungssystem eindeutig lösbar ist.

!!! Hinweis

    Bei drei Gleichungen mit drei Variablen ist die Eingabe länger. Achte deshalb besonders sorgfältig auf Klammern, Kommas und Gleichheitszeichen.

## Lineare Gleichungssysteme mit Matrizen

Lineare Gleichungssysteme können auch mit Matrizen gelöst werden. Das ist besonders in der Q1 oder Q2 sinnvoll, wenn Gleichungssysteme systematisch untersucht werden.

Das Gleichungssystem

$$
\begin{aligned}
2x+y&=5 \\
x-y&=1
\end{aligned}
$$

kann als Matrixgleichung geschrieben werden:

$$
A\cdot \vec{x}=\vec{b}
$$

mit:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1
\end{pmatrix}
$$

und:

$$
\vec{b}=
\begin{pmatrix}
5 \\
1
\end{pmatrix}
$$

Dann gilt:

$$
\vec{x}=A^{-1}\cdot \vec{b}
$$

Im TI-Nspire kann man Matrizen eingeben und damit rechnen. Für viele schulische Aufgaben ist der `solve`-Befehl aber übersichtlicher.

## Grafisches Lösen von Gleichungssystemen

Ein Gleichungssystem mit zwei Variablen kann oft grafisch interpretiert werden.

Beispiel:

$$
\begin{aligned}
y&=2x+1 \\
y&=-x+4
\end{aligned}
$$

Jede Gleichung beschreibt eine Gerade. Die Lösung des Gleichungssystems ist der Schnittpunkt der beiden Geraden.

### Vorgehen in Graphs

1. Öffne eine Graphs-Seite.
2. Gib die erste Funktion ein:

```text
f1(x) = 2x + 1
```

3. Gib die zweite Funktion ein:

```text
f2(x) = -x + 4
```

4. Bestimme den Schnittpunkt mit dem Schnittpunkt-Werkzeug.

Typischer Weg:

```text
Werkzeuge → Graph analysieren → Schnittpunkt
```

oder sinngemäß:

```text
Analyse → Schnittpunkt
```

Je nach App-Version kann die Bezeichnung leicht abweichen.

Der TI-Nspire zeigt den Schnittpunkt an. Dieser Punkt ist die Lösung des Gleichungssystems.

## Grafische Lösung rechnerisch kontrollieren

Das Gleichungssystem

$$
\begin{aligned}
y&=2x+1 \\
y&=-x+4
\end{aligned}
$$

kann im Calculator so gelöst werden:

```text
solve({y = 2x + 1, y = -x + 4}, {x, y})
```

Ergebnis:

```text
x = 1 and y = 3
```

Der Schnittpunkt ist also:

$$
S(1|3)
$$

Das bedeutet: Beide Geraden haben bei \(x=1\) denselben y-Wert \(3\).

## Nichtlineare Gleichungssysteme

Gleichungssysteme müssen nicht linear sein. Auch Schnittpunkte zwischen einer Parabel und einer Geraden können als Gleichungssystem beschrieben werden.

Beispiel:

$$
\begin{aligned}
y&=x^2 \\
y&=x+2
\end{aligned}
$$

Im TI-Nspire:

```text
solve({y = x^2, y = x + 2}, {x, y})
```

Der TI-Nspire liefert die Schnittpunkte, sofern sie symbolisch gefunden werden können.

Man kann auch die beiden rechten Seiten gleichsetzen:

```text
solve(x^2 = x + 2, x)
```

Das liefert die x-Werte der Schnittpunkte. Die y-Werte erhältst du durch Einsetzen.

## Wann nSolve sinnvoll ist

Manche Gleichungssysteme lassen sich nicht einfach symbolisch lösen. Dann kann `nSolve` helfen.

`nSolve` liefert eine numerische Näherung. Das ist besonders bei komplizierteren Gleichungen, trigonometrischen Funktionen oder realitätsnahen Modellierungen nützlich.

Beispiel:

```text
nSolve({sin(x) = y, x + y = 1}, {x, y})
```

Je nach Aufgabe muss zusätzlich ein Startwert oder ein Suchbereich angegeben werden. Numerische Lösungen müssen immer besonders sorgfältig interpretiert werden.

!!! Achtung

    `nSolve` liefert Näherungen. Bei mehreren Lösungen findet der TI-Nspire möglicherweise nicht automatisch alle Lösungen.

## Keine Lösung, eine Lösung oder unendlich viele Lösungen

Gleichungssysteme können unterschiedliche Lösungstypen haben.

### Genau eine Lösung

Zwei Geraden schneiden sich in einem Punkt.

Beispiel:

$$
\begin{aligned}
y&=2x+1 \\
y&=-x+4
\end{aligned}
$$

Lösung:

$$
S(1|3)
$$

### Keine Lösung

Zwei Geraden sind parallel und verschieden.

Beispiel:

$$
\begin{aligned}
y&=2x+1 \\
y&=2x-3
\end{aligned}
$$

Diese Geraden haben dieselbe Steigung, aber unterschiedliche y-Achsenabschnitte. Sie schneiden sich nicht.

Im TI-Nspire kann dann eine Ausgabe erscheinen, die sinngemäß bedeutet, dass keine Lösung existiert.

### Unendlich viele Lösungen

Zwei Gleichungen beschreiben dieselbe Gerade.

Beispiel:

$$
\begin{aligned}
y&=2x+1 \\
2y&=4x+2
\end{aligned}
$$

Die zweite Gleichung ist nur eine Umformung der ersten. Deshalb gibt es unendlich viele Lösungen.

Der TI-Nspire kann in solchen Fällen eine allgemeine Lösung oder eine Identität anzeigen.

## Parameter in Gleichungssystemen

In der Q1 und Q2 können Gleichungssysteme auch Parameter enthalten.

Beispiel:

$$
\begin{aligned}
ax+y&=3 \\
x-y&=1
\end{aligned}
$$

Hier ist \(a\) ein Parameter. Man kann untersuchen, für welche Werte von \(a\) das Gleichungssystem eine Lösung besitzt oder wie sich die Lösung in Abhängigkeit von \(a\) verändert.

Eingabe:

```text
solve({a*x + y = 3, x - y = 1}, {x, y})
```

Der TI-Nspire kann dann eine Lösung in Abhängigkeit von \(a\) ausgeben, sofern dies symbolisch möglich ist.

!!! Hinweis

    Wenn Parameter vorkommen, musst du das Ergebnis besonders sorgfältig lesen. Manchmal gelten Lösungen nur unter bestimmten Bedingungen.

## Gleichungssysteme in Sachkontexten

Gleichungssysteme treten häufig in Textaufgaben auf.

Beispiel:

Ein Kino verkauft Erwachsenen- und Schülertickets. Ein Erwachsenenticket kostet 10 €, ein Schülerticket 6 €. Insgesamt wurden 80 Tickets verkauft und 640 € eingenommen.

Setze:

```text
e = Anzahl der Erwachsenentickets
s = Anzahl der Schülertickets
```

Dann gilt:

$$
e+s=80
$$

und:

$$
10e+6s=640
$$

TI-Nspire-Eingabe:

```text
solve({e + s = 80, 10e + 6s = 640}, {e, s})
```

Der TI-Nspire liefert die Anzahl der jeweiligen Tickets.

Wichtig ist anschließend die Interpretation:

```text
Es wurden ... Erwachsenentickets und ... Schülertickets verkauft.
```

Eine Zahl allein ist keine vollständige Antwort.

## Typische Fehler

Ein häufiger Fehler ist das Vergessen der geschweiften Klammern.

Falsch:

```text
solve(2x + y = 5, x - y = 1, x, y)
```

Richtig:

```text
solve({2x + y = 5, x - y = 1}, {x, y})
```

Ein weiterer Fehler ist die Verwechslung von `=` und `:=`.

Falsch im Gleichungssystem:

```text
2x + y := 5
```

Richtig:

```text
2x + y = 5
```

Auch fehlende Multiplikationszeichen können Probleme verursachen. Schreibe bei Unsicherheit lieber:

```text
2*x + y = 5
```

statt:

```text
2x + y = 5
```

Der TI-Nspire versteht zwar häufig die Kurzschreibweise, aber die Schreibweise mit `*` ist eindeutiger.

## Didaktischer Bezug zum Kernlehrplan NRW

In der EF dienen Gleichungssysteme besonders dazu, lineare Zusammenhänge zu untersuchen und Schnittpunkte von Graphen zu bestimmen.

In der Q1 werden Gleichungssysteme unter anderem bei der Analysis verwendet, zum Beispiel bei Schnittpunkten, Extrembedingungen oder beim Bestimmen von Funktionsgleichungen.

In der Q2 treten Gleichungssysteme in komplexeren Modellierungsaufgaben, in analytischer Geometrie und bei Parameteruntersuchungen auf.

Digitale Werkzeuge wie der TI-Nspire unterstützen dabei den Darstellungswechsel:

- Gleichungssystem als Term
- Lösung im Calculator
- Darstellung als Graph
- Interpretation im Sachzusammenhang

## Was gehört zu einer vollständigen Lösung?

Eine vollständige Lösung enthält nicht nur die TI-Nspire-Ausgabe.

Du solltest angeben:

1. welche Variablen verwendet werden,
2. welches Gleichungssystem gelöst wird,
3. welchen TI-Nspire-Befehl du nutzt,
4. welche Lösung der Rechner liefert,
5. was die Lösung im Kontext bedeutet.

Unvollständig wäre:

```text
x = 1, y = 3
```

Besser ist:

```text
Das Gleichungssystem hat die Lösung x = 1 und y = 3. Grafisch bedeutet das, dass sich die beiden Geraden im Punkt S(1|3) schneiden.
```

Bei Sachaufgaben:

```text
Es wurden 40 Erwachsenentickets und 40 Schülertickets verkauft.
```

## Checkliste

Prüfe vor dem Abschreiben deines Ergebnisses:

- Habe ich alle Gleichungen korrekt eingegeben?
- Habe ich echte Gleichheitszeichen verwendet?
- Stehen die Gleichungen in geschweiften Klammern?
- Stehen die gesuchten Variablen in geschweiften Klammern?
- Habe ich die richtige Anzahl an Variablen angegeben?
- Passt die Lösung zu allen Gleichungen?
- Muss ich das Ergebnis grafisch oder im Sachkontext interpretieren?
- Gibt es möglicherweise keine, eine oder unendlich viele Lösungen?

## Kurzzusammenfassung

Ein Gleichungssystem löst du im TI-Nspire mit:

```text
solve({Gleichung1, Gleichung2}, {Variable1, Variable2})
```

Beispiel:

```text
solve({2x + y = 5, x - y = 1}, {x, y})
```

Für grafische Lösungen kannst du die Gleichungen als Funktionen darstellen und den Schnittpunkt bestimmen.

Bei komplizierteren Gleichungssystemen kann `nSolve` helfen, liefert aber nur numerische Näherungen.

Wichtig ist immer: Das Ergebnis muss kontrolliert und im mathematischen oder sachlichen Zusammenhang interpretiert werden.
