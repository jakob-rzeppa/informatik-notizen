# Zahlensysteme

## Binäre Zahlen (positiv)

Der Wert jeder Stelle $s$ wird durch $2^{s-1}$ berechnet.

### Aufschreiben

Nullen vor der letzten Eins (größere Stellen) müssen angegeben werden, wenn nach einer bestimmt großen Zahl gefragt wird.

> $(42)_{10}$ als 8-Bit Zahl: (00101010). Die Null am Anfang muss angegeben werden.

>$(42)_{10}$ als Binärzahl: (101010). Die Null am Anfang muss nicht angegeben werden.

### Anzahl der Kombinationen

Die Anzahl der Kombinationen ist immer der Wert der Stelle des nächst höheren Bits.

Bei 4 Bits:
Wert der höchsten Stelle: $2^3$
=> Anzahl der Kombinationen: $2^4 = 16$

### höchst darstellbare Zahl

Die höchst darstellbare Zahl ist immer die Anzahl der Kombinationen (der Wert der Stelle des nächst höheren Bits) minus 1 (wegen 0).

Bei 4 Bits:
Wert der höchsten Stelle: $2^3$
=> Anzahl der Kombinationen: $2^4 = 16$
=> höchst darstellbare Zahl: $2^4 - 1 = 15$

### Binärzahl zu Dezimalzahl

Jede Stelle muss mit dem Wert der Stelle multipliziert werden.

### Dezimalzahl zu Binärzahl

Um eine Dezimalzahl zu einer Binärzahl umzurechnen kann man die Zahl durch zwei dividieren. Den Rest schreibt man auf und mit dem Ergebnis wiederholt man das dividieren, bis das Ergebnis Null ist. Dann schreibt man den Rest *von unten nach oben* auf.

$$
\begin{align}
42 : 2 = 21 \text{ Rest } 0\\
21 : 2 = 10 \text{ Rest } 1\\
10 : 2 = 5 \text{ Rest } 0\\
5 : 2 = 2 \text{ Rest } 1\\
2 : 2 = 1 \text{ Rest } 0\\
1 : 2 = 0 \text{ Rest } 1\\

\Rightarrow 101010
\end{align}
$$

> Das gleiche Verfahren lässt sich auch für andere Zahlendarstellungen anwenden: bei Oktalzahlen mit 8 dividieren, bei Hexadezimal mit 16.

### Binärzahl zu Hexadezimalzahl

1. In Viererblöcke aufteilen.
2. Hexadezimalzahl für jeden Block bestimmen.
3. Ergebnis zusammensetzen

Wandeln Sie die Binärzahl `1101011100` in Hexadezimal um:

$$
(00)11|0101|1100
$$

$$
(3)_{16} | (5)_{16} | (C)_{16}
$$

$$
(35C)_{16}
$$
