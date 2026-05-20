# Integrale und Stammfunktionen

Integrale gehören zu den zentralen Werkzeugen der Analysis. Während die Ableitung Änderungsraten und Steigungen beschreibt, werden Integrale häufig verwendet, um Bestände, Flächeninhalte, Gesamtänderungen oder aufsummierte Größen zu bestimmen. Das CAS kann Integrale und Stammfunktionen sehr leicht berechnen.

## Was ist eine Stammfunktion?

Eine Stammfunktion ist eine Funktion, deren Ableitung wieder die ursprüngliche Funktion ergibt.

Wenn gilt:

$$
F'(x)=f(x)
$$

dann nennt man \(F\) eine Stammfunktion von \(f\).

Beispiel:

$$
f(x)=2x
$$

Eine passende Stammfunktion ist:

$$
F(x)=x^2
$$

denn:

$$
F'(x)=2x
$$

Da beim Ableiten konstante Summanden verschwinden, gibt es nicht nur eine Stammfunktion, sondern unendlich viele.

Auch

$$
F(x)=x^2+5
$$

ist eine Stammfunktion von \(f(x)=2x\), denn auch hier gilt:

$$
F'(x)=2x
$$

Deshalb schreibt man beim unbestimmten Integral:

$$
\int 2x\,dx=x^2+C
$$

Das \(C\) steht für eine beliebige Konstante.

## Unbestimmtes Integral

Ein unbestimmtes Integral liefert eine Stammfunktion.

Die allgemeine Eingabe lautet:

$$∫Funktion  \quad d \quad Variable$$

Das Integralzeichen (inkusive Platzhalter um die Funktion und die Variable einzufügen) findet man unter 
``Menü -> Mathematische Operatoren -> Analysis -> Integral``

Alternativ kann man dies auch einfach über die Tastatur der App einfügen:

<img src="..\..\img\integral1.png" alt="Integral"/>

Hierzu schauen wir uns beispielsweise die Funktion $f(x) = x^2 $ an

<img src="..\..\img\integral2.png" alt="Integral"/>

<img src="..\..\img\integral3.png" alt="Integral"/>

Je nach Einstellung und Version wird die Integrationskonstante \(C\) nicht automatisch ergänzt. Mathematisch musst du sie beim unbestimmten Integral aber mitdenken.

Vollständig lautet die Stammfunktion also:

$$
F(x)=\frac{1}{3}x^3+C
$$

## Bestimmtes Integral

Ein bestimmtes Integral beschreibt die orientierte Fläche zwischen dem Graphen einer Funktion und der x-Achse in einem festgelegten Intervall $[a;b]$.

Man schreibt:

$$
\int_a^b f(x)\,dx
$$

Dabei ist:

- \(a\) die untere Grenze
- \(b\) die obere Grenze
- \(f(x)\) die Funktion
- \(dx\) die Integrationsvariable

Liegt der Graph oberhalb der x-Achse, zählt die Fläche positiv. Liegt der Graph unterhalb der x-Achse, zählt die Fläche negativ.

Das Integralzeichen (inkusive Platzhalter um die Grenzen, die Funktion und die Variable einzufügen) findet man unter 
``Menü -> Mathematische Operatoren -> Analysis -> Integral``

Alternativ kann man dies auch einfach über die Tastatur der App einfügen:

<img src="..\..\img\integral1.png" alt="Integral"/>

## Bestimmtes Integral berechnen

Die allgemeine Eingabe lautet:

$$
\int_{untere Grenze}^{obere Grenze} Funktion \quad \,d \quad Variable
$$

Wir schauen uns wieder als Beispiel $f(x)=x^2$ an. Gesucht ist:

$$
\int_0^3 x^2\,dx
$$

Dies kann man einfach mit dem CAS bestimmen:

<img src="..\..\img\integral4.png" alt="Integral"/>

Das bedeutet: Die orientierte Fläche zwischen dem Graphen von \(f(x)=x^2\) und der x-Achse im Intervall \([0;3]\) beträgt 9 Flächeneinheiten.

## Bestimmtes Integral mit definierter Funktion

Auch bei Integralen ist es oft sinnvoll, die Funktion zuerst zu definieren:

<img src="..\..\img\integral5.png" alt="Integral"/>

Diese Schreibweise ist übersichtlicher, wenn du dieselbe Funktion mehrfach verwenden möchtest.

## Checkliste

Prüfe vor dem Abschreiben deines Ergebnisses:

- Habe ich die Funktion richtig eingegeben?
- Habe ich die richtige Integrationsvariable verwendet?
- Sind die Grenzen korrekt?
- Suche ich eine Stammfunktion oder ein bestimmtes Integral?
- Muss ich eine Konstante \(C\) ergänzen?

