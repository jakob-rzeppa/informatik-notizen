# Verzweigungen

```java
if (/* Ausdruck */) {
	// ...
} else if (/* Ausdruck */) {
	// ...
} else {
	// ...
}
```

Wenn der Ausdruck true zurückgibt wird der Block ausgeführt, sonst weitergegangen.

## Vergleich von Fließkommazahlen

Q: Vergleich von Fließkommazahlen
A: Da Fließkommazahlen kleine Abweichungen von der gewünschten Zahl haben können, kann der == Operator nicht verwendet werden. Daher sollte die Differenz der Zahlen genommen werden und geguckt werden, ob diese kleiner als ein bestimmter Wert (wie 0.00000001) ist.
<!--ID: 1760601581562-->

```java
if (Math.abs(d - e) < 1E-8) // ...
```

## Switch-Anweisung

```java
switch (/* Ausdruck */) {
	case /* Konstante */:
		// ...
		break;
	default:
		// ...
		break;
}
```

Wenn "break" nicht verwendet wird, werden nach dem Ausführen des ersten Blocks die Weiteren auch noch überprüft und ggf. ausgeführt.