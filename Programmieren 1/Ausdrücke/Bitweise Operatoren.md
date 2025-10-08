# Bitweise Operatoren

Bitweise Operatoren werden auf die Binäre Darstellung einer Zahl angewand.

## |

Für jede Stelle wird per OR der Output bestimmt.

```java
byte x = 0b1010
byte y = 0b0110
byte r = x | y
// r = 0b1110
```

## &

Für jede Stelle wird per AND der Output bestimmt.

```java
byte x = 0b1010
byte y = 0b0110
byte r = x | y
// r = 0b0010
```

## ^

Für jede Stelle wird per XOR der Output bestimmt.

```java
byte x = 0b1010
byte y = 0b0110
byte r = x | y
// r = 0b1100
```

## <<

Die Bits werden nach *links* verschoben und die neue Stelle *mit einer Null* aufgefüllt. Überstehende Bits werden fallen gelassen.

```java
byte x = 0b10100000
byte r = x << 1
// r = 0b01000000
```

## >>

Die Bits werden nach *rechts* verschoben und die neue Stelle mit *dem derzeitigen Vorzeichen* aufgefüllt. Überstehende Bits werden fallen gelassen.

```java
byte x = 0b00000011
byte r = x >> 1
// r = 0b00000001
```
```java
byte x = 0b11111100
byte r = x >> 1
// r = 0b11111110
```

## >>>

Die Bits werden nach *rechts* verschoben und die neue Stelle mit *einer Null* aufgefüllt. Überstehende Bits werden fallen gelassen.

```java
byte x = 0b00000011
byte r = x >>> 1
// r = 0b00000001
```
```java
byte x = 0b11111100
byte r = x >>> 1
// r = 0b01111110
```