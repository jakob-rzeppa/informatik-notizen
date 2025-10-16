# Logische Operatoren

Logische Operatoren verknüpfen [Aussagen](Aussagen.md) miteinander.

Operatoren, die eine Aussage verändern werden unäre Operationen genannt und Operatoren, die zwei Aussagen verknüpfen binäre Operatoren genannt.

Es gibt insgesamt $2^4 = 16$ binäre Operatoren, da es 16 unterschiedliche Kombinationen gibt.

## Negation $\neg$ (!)

Die Negation zweier Aussagen ist nur dann 

| $A$ | $\neg A$ |
| --- | --- |
| $0$ | $1$ |
| $1$ | $0$ |

## Konjunktion $\land$ (&&)

Die Konjunktion zweier Aussagen ist nur dann wahr, wenn beide Aussagen wahr sind.

| $A$ | $B$ | $A \land B$ |
| --- | --- | --- |
| $0$ | $0$ | $0$ |
| $0$ | $1$ | $0$ |
| $1$ | $0$ | $0$ |
| $1$ | $1$ | $1$ |

## Disjunktion $\lor$ (||)

Die Disjunktion zweier Aussagen in nur dann falsch, wenn beide Aussagen falsch sind.

| $A$ | $B$ | $A \lor B$ |
| --- | --- | --- |
| $0$ | $0$ | $0$ |
| $0$ | $1$ | $1$ |
| $1$ | $0$ | $1$ |
| $1$ | $1$ | $1$ |

## Subjunktion $\rightarrow$ (=>)

Die Subjunktion zweier Aussagen in nur dann falsch, wenn die erste Aussage wahr und die zweite falsch ist.

Wenn A nicht wahr ist kann nicht auf B geschlossen werden, daher ist die Aussage immer wahr. Wenn A wahr ist kann auf B geschlossen werden. Dem entsprechend ist die Aussage wahr, wenn auch B wahr ist (=A ist keine Lüge) und falsch wenn B falsch ist (=A ist eine Lüge).
=> Formal sagt uns die Subjunktion, wann Aussage A keine Lüge ist.

| $A$ | $B$ | $A \rightarrow B$ |
| --- | --- | --- |
| $0$ | $0$ | $1$ |
| $0$ | $1$ | $1$ |
| $1$ | $0$ | $0$ |
| $1$ | $1$ | $1$ |

$$
(A \rightarrow B) = (\neg A \lor B)
$$

$$
(A \rightarrow B) = ( \neg B \rightarrow \neg A)
$$

$$
\neg (A \rightarrow B) = (A \land \neg B)
$$

## Bijunktion $\leftrightarrow$ (<==>)

Die Bijunktion zweier Aussagen ist immer wahr, wenn A und B den gleichen Wahrheitswert haben.

| $A$ | $B$ | $A \leftrightarrow B$ |
| --- | --- | --- |
| $0$ | $0$ | $1$ |
| $0$ | $1$ | $0$ |
| $1$ | $0$ | $0$ |
| $1$ | $1$ | $1$ |

$$
(A \leftrightarrow B) = ((A \rightarrow B) \land (B \rightarrow A))
$$

$$
(A \nleftrightarrow B) = \neg (A \leftrightarrow B)
$$

## Alternation $\nleftrightarrow$ (<!=>)

Die Alternation zweier Aussagen ist nur dann wahr, wenn A und B unterschiedliche Wahrheitswerte haben.

| $A$ | $B$ | $A \nleftrightarrow B$ |
| --- | --- | --- |
| $0$ | $0$ | $0$ |
| $0$ | $1$ | $1$ |
| $1$ | $0$ | $1$ |
| $1$ | $1$ | $0$ |

$$
\neg (A \leftrightarrow B) = (A \nleftrightarrow B)
$$