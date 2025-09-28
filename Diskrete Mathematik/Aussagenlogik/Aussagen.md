# Aussagen

Q: Definition Aussage
A: Eine Aussage ist ein Satz, der *entweder* wahr *oder* falsch ist.
<!--ID: 1759064692642-->

> Beispiel: "Die Erde ist flach."

## Aussageformen

Ist also $x > 0$ eine Aussage?

Nein: $x > 0$ ist nicht *entweder* wahr *oder* falsch. $x > 3$ ist abhängig von $x$ und dementsprechend weder wahr noch falsch. Deshalb ist $x > 0$, ohne $x$ zu kennen, keine Aussage, sondern bloß aussagenartig. 

Wenn $x := 3$ wird $x > 0$ jedoch zu einer Aussage, da es jetzt entweder wahr oder falsch ist - in diesem Fall wahr.

Sätze, die erst dadurch zu Aussagen werden, indem Variablen konkret mit Werten belegt werden, - wie $x > 0$ - werden als *Aussageformen* bezeichnet.

Q: Definition Aussageform
A: Aussageformen sind Sätze oder Ausdrücke, die variable Elemente enthalten und durch Belegung dieser variablen Elemente mit konkreten Werten zu einer Aussage werden. Beispiel: $x > 0$
<!--ID: 1759065819675-->

### Aussageformen als Funktion

Aussageformen kann man sich auch als [[Diskrete Mathematik/Grundlegende Strukturen/Funktionen|Funktion]] vorstellen, die Variablen in Aussagen mit Wahrheitswerten umwandeln:

```setlx
is_greater_than_one := procedure(x) { return x > 1; };

is_greater_than_one(2);
=> True
```

## Aussagen / Aussageformen als Modelle

Aussagen und Aussageformen sind keine Gegenstände der Realität. Sie sind lediglich [[Modellbildung|Modelle]].