# Fließpunkt-Darstellung

Eine Fließpunkt-Darstellung in Binärcode besteht aus:

- Vorzeichen ($s \in \{0,1\}$)
- Mantisse ($m \in \{\mathbb{R}  | 1 \leq m < 2\}$) => Wert der Zahl mit nur einer Stelle vor dem Komma, im Speicher sind nur die Zahlen nach dem Komma, da vor dem Komma immer null steht
- Exponent ($e \in \mathbb{N}$) => Verschiebung des Kommas (nur positiv)
- Basis ($b = (10)_2 = (2)_{10}$)

$$
(-1)^s \cdot m \cdot b^e
$$

> Bei einer Fließpunkt-Darstellung kann es sein, dass manche Zahlen nicht genau dargestellt werden können und daher es kleine Fehler geben (wie 10,0000005f, wenn 10,0f gewünscht ist).

## Typen in Java

### Float

Genauigkeit von ca. 7 Dezimalstellen

### Double

Genauigkeit von ca. 15 Dezimalstellen

## Berechnung

### Von Dezimal zu Float

$$
\begin{align}
(2,75)_{10} = (2\cdot1 + 1 \cdot 0 + \frac{1}{2} \cdot 1 + \frac{1}{4} \cdot 1)_{10}\\
\Rightarrow (10,11)_2\\
10,11 = 0,1011 \cdot 10^{10} = (-1)^0 \cdot 0,1011 \cdot 10^{10}\\
\\
\Rightarrow m = 1011; e = 10; s = 0
\end{align}
$$

### Von Float zu Dezimal

$$
\begin{align}
(-1)^0 \cdot 0,1011 \cdot 10^{10} = 0,1011 \cdot 10^{10} = 10,11\\
\Rightarrow (2 \cdot 1 + 1 \cdot 0 + \frac{1}{2} \cdot 1 + \frac{1}{4} \cdot 1)_{10}\\
\Rightarrow (2,75)_{10}
\end{align}
$$