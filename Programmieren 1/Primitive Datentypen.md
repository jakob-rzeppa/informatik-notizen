# Primitive Datentypen

## int

Q: Was passiert, wenn eine Zahl über den maximalen Wert eines Integers geht?
A: Es wird auf die kleinstmögliche Zahl übergesprungen und weiter gemacht.
<!--ID: 1758956803435-->

## float

Manchmal können komische Dinge mit den letzten Nachkommastellen eines Floats passieren.

```Java
float hundertGramm = 0.1f;
float klio = hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm + hundertGramm;

System.out.println(kilo);
// => 1.0000001
```