# Normalform von boolischen Ausdrücken

Die Normalform ermöglicht eine genormte Darstellung jeglicher bollischer Ausdrücke.

## Konjunktive Normalform (KNF)

Die konjunktive Normalform ist eine AND-Verknüpfung von Maxtermen.

1. Für jede Konfiguration von Inputs, die *Null* ergibt, muss ein [Maxterm](Maxterme.md) erstellt werden. Maxterme werden erstellt, indem die Variablen durch eine OR-Vernküpfung kombiniert werden, während die Terme, die *Eins sind negiert* werden.
2. Diese Maxterme werden mit einer *AND-Verknüpfung* kombiniert.

<!-- TODO möglicherweise negation des ergebnisses -->

| A | B | C | E | Maxterm |
| --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 0 | $A \lor B \lor C$ |
| 0 | 0 | 1 | 1 | |
| 0 | 1 | 0 | 0 | $A \lor \overline{B} \lor C$ |
| 0 | 1 | 1 | 1 | |
| 1 | 0 | 0 | 1 | |
| 1 | 0 | 1 | 1 | |
| 1 | 1 | 0 | 1 | |
| 1 | 1 | 1 | 0 | $\overline{A} \lor \overline{B} \lor \overline{C}$ |

$\Rightarrow \text{KNF} = (A \lor B \lor C) \land (A \lor \overline{B} \lor C) \land (\overline{A} \lor \overline{B} \lor \overline{C})$

> Tipp: In der Klausur die Maxterme benennen

## Disjunktive Normalform (DNF)

Die disjunktive Normalform ist eine OR-Verknüpfung von Mintermen.

1. Für jede Konfiguration von Inputs, die *Eins* ergibt, muss ein [Minterm](Minterme.md) erstellt werden. Minterme werden erstellt, indem die Variablen durch eine AND-Vernküpfung kombiniert werden, während die Terme, die *Null sind negiert* werden.
2. Diese Minterme werden mit einer *OR-Verknüpfung* kombiniert.

| A | B | C | E | Minterm |
| --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 1 | $\overline{A} \land \overline{B} \land \overline{C}$ |
| 0 | 0 | 1 | 0 | |
| 0 | 1 | 0 | 1 | $\overline{A} \land B \land \overline{C}$ |
| 0 | 1 | 1 | 0 | |
| 1 | 0 | 0 | 0 | |
| 1 | 0 | 1 | 0 | |
| 1 | 1 | 0 | 0 | |
| 1 | 1 | 1 | 1 | $A \land B \land C$ |

$\Rightarrow \text{DNF} = (\overline{A} \land \overline{B} \land \overline{C}) \lor (\overline{A} \land B \land \overline{C}) \lor (A \land B \land C)$

> Tipp: In der Klausur die Minterme benennen