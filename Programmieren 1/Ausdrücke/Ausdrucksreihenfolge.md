# Ausdrucksreihenfolge

Alle [[Ausdrücke]] gleicher Priorität werden von *links nach rechts* ausgeführt.

```java
int i = 2;
i = i + (++i)
// i = 5, da ++i als zweites ausgeführt wird

int i = 2;
i = (++i) + i;
// i = 6, da ++i zuerst ausgeführt wird und als Side-Effect i dabei 3 wird
```

*Klammern haben die höchste Priorität* und ermöglichen Ausführungen, die von den Reihenfolgen durch Operatorenränge abweichen.

## Ränge

### 1

Q: Welche Operatoren haben den Rang 1?
A: Alle Operatoren mit einer Stelligkeit von 1 (u. a. increment, typecast, unäres Minus (Negation einer Zahl))
<!--ID: 1759938912322-->

### 2 

Q: Welche Operatoren haben den Rang 2?
A: Mal, Geteilt, Modulo
<!--ID: 1759938962462-->

### 3

Q: Welche Operatoren haben den Rang 3?
A: Addition und String-Konkatenation
<!--ID: 1759938989289-->

### Rest

Q: Reihenfolge der Operatoren vom Rang > 3
A: Bitweise Verschiebung, Vergleiche, Logik, Ternary, Zuweisungen
<!--ID: 1759939142963-->
