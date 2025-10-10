# Ausdrücke (Expressions)

Ausdrücke bestehen aus einem Operator und einem oder mehreren Operanten.

> Beispiel: Operator: +, Operanten x / y ⇒ Ausdruck: x + y

Die Anzahl der Operanten ist die *Stelligkeit* des Ausdrucks. Die meisten Ausdrücke in Java sind ein- oder zweistellig. Der einzige dreistellige Ausdruck ist der "Ternary Operator" (Fragezeichen Operant)

Alle Ausdrücke geben einen spezifischen Rückgabewert und Typ zurück. Wenn die Operanten eines Ausdrucks unterschiedlich sind, muss ein [Typecast](../Speicher%20und%20Variablen/Typecasts.md) verwendet werden. Der Rückgabewert ist generell vom *Typ, der am meisten Daten darstellen kann* (Long vor Integer, Double vor Float etc.).

Ausdrücke haben eine [Ausdrucksreihenfolge](Ausdrucksreihenfolge.md).

## Side-Effects von Ausdrücken

Ausdrücke können [Side-Effects](../Funktionen/Side-Effects.md) haben - also den Zustand eines der Operanten verändern.