# Vereinfachen von Ausdrücken

| $A$ | $B$ | $C$ | $A \lor \neg B$ | $A \land \neg C$ | $(A \lor \neg B) \lor (A \land \neg C)$ |
|:-:|:-:|:-:|:-------:|:---:|:-----:|:-------------:|
| 0 | 0 | 0 |    1 |   0   |       1       |
| 0 | 0 | 1 |    1 |   0   |       1       |
| 0 | 1 | 0 |    0 |   0   |       0       |
| 0 | 1 | 1 |    0 |   0   |       0       |
| 1 | 0 | 0 |    1 |   1   |       1       |
| 1 | 0 | 1 |    1 |   0   |       1       |
| 1 | 1 | 0 |    1 |   1   |       1       |
| 1 | 1 | 1 |    1 |   0   |       1       |

$A \lor \neg B$ und $(A \lor \neg B) \lor (A \land \neg C)$ haben die gleichen Wahrheitswerte. Das bedeutet, dass die [Aussagen](Aussagen.md) identisch sind. Dementsprechend kann $(A \lor \neg B) \lor (A \land \neg C)$ zu $A \lor \neg B$ vereinfacht werden.

$$
((A \lor \neg B) \lor (A \land \neg C)) = (A \lor \neg B)
$$

## gängige Fälle

$$
\neg(\neg A) = A
$$

$$
\neg(A \land B) = (\neg A \lor \neg B)
$$

> Die Negation der Konjunktion von A und B ist gleich der Disjunktion der Negationen von A und B

$$
\neg(A \lor B) = (\neg A \land \neg B)
$$

> Die Negation der Disjunktion von A und B ist gleich der Konjunktion der Negationen von A und B