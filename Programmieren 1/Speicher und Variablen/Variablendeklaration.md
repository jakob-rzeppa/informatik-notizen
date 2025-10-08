# Variablendeklaration

```java
// Type Identifier
int x;

// Type Identifier, Identifier, ...
int x, y;

// Type Identifier = Expression
int x = 1 + 1;

// Type Identifier = Expression, Identifier = Expression, ...
int x = 2, y = 1;
```

## Identifier

Bestehen aus 

- Unicode Buchstaben  
- digitalen Ziffern  
- Währungssymbolen  
- Verbindungszeichen (Bsp.: Bindestrich “-”)
- dürfen theoretisch beliebig lang sein

Einschränkungen 

- Beginnen mit einem Buchstaben, Währungssymbol oder  
Verbindungszeichen, d.h. insb. nicht mit einer Ziffer  
- enthalten keine Leerzeichen  
- Identifier sind case-sensitive (Unterscheidung Groß-/  
Kleinschreibung)  
- und sind keine reservierten Schlüsselwörter (class, main, for,...