# Side-Effects

Side-Effects bezeichnen, dass eine Methode, Ausdruck etc. nicht nur Eingabe und Ausgabe hat, sondern Daten außerhalb direkt verändert oder sich auf diese bezieht.

```java
class Main {
	static int i = 0;
	
	static void increment(int value) {
		// Side-Effect
		i += value;
	}
	
	public static void main(String[] args) {
		Main.increment(5);
	}
}
```

Methoden, die keine Side-Effects besitzen werden als reine Funktionen (pure functions) bezeichnet.