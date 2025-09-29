# Boolesche Funktionen (Schaltfunktionen)

Eine boolesche Funktion kann eindeutig durch eine vollständige Wahrheitstafel beschrieben werden.

## Rechengesetze

> In der Klausur kann es sein, dass man Ausdrücke zusammenfassen muss.

||Operator $\land$| Operation $\lor$|
|---|---|---|
|kommutativ|$a \land b = b \land a$|$a \lor b = b \lor a$|
|distributiv|$(a \land b) \lor (a \land c) = a \land (b \lor c)$|$(a \lor b) \land (a \lor c) = a \lor (b \land c)$|
|Identität|$a \land 1 = a$|$a \lor 0 = a$|
|inversion|$a \land \overline{a} = 0$|$a \lor \overline{a} = 1$|

## Wertetabellen erstellen

> In der Klausur kann es sein, dass man eine Wertetabelle von einem Ausdruck oder andersherum bestimmen muss.

Man kann bei einer Wertetabelle auch Zwischenschritte mit eintragen:

$$
y = (a \land b) \lor (a \land \overline{b})
$$

|a|b|$(a \land b)$|$(a \land \overline{b})$|$(a \land b) \lor (a \land \overline{b})$|y|
|---|---|---|---|---|---|
|0|0|0|0|0|0|
|0|1|0|0|0|0|
|1|0|0|1|1|1|
|1|1|1|0|1|1|
