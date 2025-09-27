# Zahlendarstellungen

## Binäre Zahlen

Der Wert jeder Stelle $s$ wird durch $2^{s-1}$ berechnet.

Q: Reihe der Potenzen zur Basis 2
A: $2^0 = 1; 2^1 = 2; 2^2 = 4; 2^3 = 8; 2^4 = 16; 2^5 = 32, 2^6 = 64, 2^7 = 128, 2^8 = 256; 2^9 = 512, 2^{10} = 1024, 2^{11} = 2048, 2^{12} = 4096$
<!--ID: 1758697029624-->

### Anzahl der Kombinationen

Die Anzahl der Kombinationen ist immer der Wert der Stelle des nächst höheren Bits.

Bei 4 Bits:
Höchste Stelle: $2^3$
=> Anzahl der Kombinationen: $2^4 = 16$

### höchst darstellbare Zahl

Die höchst darstellbare Zahl ist immer die Anzahl der Kombinationen (der Wert der Stelle des nächst höheren Bits) minus 1 (wegen 0).

Bei 4 Bits:
Höchste Stelle: $2^3$
=> Anzahl der Kombinationen: $2^4 = 16$
=> höchst darstellbare Zahl: $2^4 - 1 = 15$
