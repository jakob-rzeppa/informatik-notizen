# Darstellung von Zahlen

## positive Zahlen

Wie in [[Zahlensysteme]] beschrieben.

| Bytes | Bits | Wertebereich | Datentyp |
| - | - | - | - |
| 1 | 8 | [0;255] | unsigned char |
| 2 | 16 | [0;$2^{16}-1$] | unsigned char |
| 4 | 32 | [0;$2^{32}-1$] | unsigned int |
| 8 | 64 | [0;$2^{64}-1$] | unsigned long |

## Big- und Little-Endian Speicherung

Big- und Little-Endian beschreiben die Reihenfolge, in der Bytes im Speicher abgelegt werden. Also bei einem 32-Bit Integer mit 4 Bytes welcher Byte zuerst liegt.

### Little-Endian

- Das Byte mit der *niedrigsten Wertigkeit* wird *zuerst* gespeichert.
- Das Byte mit der *höchsten Wertigkeit* wird *zuletzt* gespeichert.

Zahl: 3F4E = 16206

| Adresse | Daten |
| --- | --- |
| 1001 | 3F |
| 1000 | 4E |

> höhere Adresse = höherer Wert

### Big-Endian

- Das Byte mit der *höchsten Wertigkeit* wird *zuerst* gespeichert.
- Das Byte mit der *niedrigsten Wertigkeit* wird *zuletzt* gespeichert.

Zahl: 3F4E = 16206

| Adresse | Daten |
| --- | --- |
| 1001 | 4E |
| 1000 | 3F |

> höhere Adresse = kleinerer Wert

> Genutzt von der JVM

## negative Zahlen

### Betrags-Vorzeichendarstellung

Q: Bildung der Betrags-Vorzeichendarstellung
A: Das höchstwertig Bit wird für das Vorzeichen verwendet: 0 = Positiv, 1 = Negativ. Der Rest beschreibt den Betrag.
<!--ID: 1759171198426-->


Wertebereich bei 8-Bits: $[- (2^{7} - 1); 2^{7} - 1]$

|**Dezimal**|0|1|2|3|4|5|6|7|
|---|---|---|---|---|---|---|---|---|
|**Binär**|0000|0001|0010|0011|0100|0101|0110|0111|

|**Dezimal**|0|-1|-2|-3|-4|-5|-6|-7|
|---|---|---|---|---|---|---|---|---|
|**Binär**|1000|1001|1010|1011|1100|1101|1110|1111|

#### Problem

- Die Null wird positiv und negativ dargestellt: "verschwendeter" Platz und *Probleme bei Gleichheitstests*.

### Einerkompliment

Q: Bildung des Einerkompliment
A: Eine negative Zahl wird binär durch das bitweise Kompliment (Umdrehen von 1 und 0) der entsprechenden positiven Zahl dargestellt.
<!--ID: 1759171198429-->


Wertebereich bei 8-Bits: $[- (2^{7} - 1); 2^{7} - 1]$

| **Dezimal** | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|-------------|-----|-----|-----|-----|-----|-----|-----|-----|
| **Binär** | 0000| 0001| 0010| 0011| 0100| 0101| 0110| 0111|

| **Dezimal** | 0 | -1 | -2 | -3 | -4 | -5 | -6 | -7 |
|---|---|-----|-----|-----|-----|-----|-----|---|
| **Binär** | 1111| 1110| 1101| 1100| 1011| 1010| 1001|1000|

#### Problem

- Die Null wird positiv und negativ dargestellt: "verschwendeter" Platz und *Probleme bei Gleichheitstests*.
- Arithmetische Operationen, die das Vorzeichen wechseln müssen gesondert betrachtet werden.

### Zweierkompliment

> Wird normalerweise genutzt.

Q: Bildung des Zweierkompliment
A: Zuerst wird das Einerkompliment gebildet. Die entstehende Binärzahl (als positive Zahl gesehen) wird um eins erhöht.
<!--ID: 1759169795306-->

asymmetrischer  Wertebereich bei 8-Bits: $[- (2^{7}); 2^{7} - 1]$

| **Dezimal** | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|-------------|-----|-----|-----|-----|-----|-----|-----|-----|
| **Binär** | 0000| 0001| 0010| 0011| 0100| 0101| 0110| 0111|

| **Dezimal** | -1 | -2 | -3 | -4 | -5 | -6 | -7 | -8 |
|---|---|-----|-----|-----|-----|-----|-----|-----|
| **Binär** | 1111| 1110| 1101| 1100| 1011| 1010| 1001|1000|

## Addition / Subtraktion

Um Zahlen zu addieren kann man "normal" Schriftlich addieren. Dabei darf man nicht vergessen, dass weitergezogene Werte auch in Binär sein müssen.

Subtraktion ist, wenn das Zweierkompliment verwendet wird, genau wie die Addition, nur dass ein Wert negativ ist.

> Falls man unsicher ist kann man auch immer in Dezimal und zurück umwandeln.