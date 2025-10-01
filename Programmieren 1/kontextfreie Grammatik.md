# kontextfreie Grammatik

Grammatik beschreibt, wie eine Sprache aufgebaut werden darf. Über sie wird eine [[Sprache]] erschaffen.

## Bestandteile der Grammatik

Eine Grammatik besteht aus

- einer Menge von *Nichtterminalsymbolen*
- einer Menge von *Terminalsymbolen*
- einer Menge von *Produktionen* (Regeln der Sprache)
- einem *Startsymbol* (Startpunkt)

### Nichtterminalsymbole

sind Hilfskonstrukte im Erzeugungsprozess und verschwinden schließlich.

Über die Nichtterminalsymbole wird die Struktur der Grammatik beschrieben.

> Beispiel "Verb" als Nichtterminalsymbol, welches durch Verben wie "springen" oder "laufen" ersetzt werden darf.

### Terminalsymbole

erscheinen im endgültigen (=terminalen) Text der Sprache (hier: Java-Programm).

> Beispiel "springen" oder "laufen", welche das Nichtterminalsymbol "Verb" ersetzen.

### Produktion (Regeln)

Die Regeln (Produktionen) können *unabhängig vom Kontext* verwendet werden, da es sich um eine *kontextfreie Grammatik* handelt.

In diesem Fall ist die einzige Regel, dass ein Nichtterminalsymbol durch eine beliebige Anzahl von Terminal- und Nichtterminalsymbolen ersetzt werden darf.

## Was bedeutet das jetzt genau?

Im Folgenden wird durch das Ersetzen von Nichtterminalsymbolen durch andere Nichtterminalsymbole oder Terminale ein Satz gebildet.

```
// Das Startsymbol ist das Nichtterminalsymbol Satz

// Das Nichtterminalsymbol Satz wird durch die Nichtterminalsymbole Subjekt und Prädikat ersetzt.
Satz := Subjekt Prädikat

// Die Nichtterminalsymbol Subjekt wird durch die Nichtterminalsymbole Artikel und Substantiv ersetzt.
Subjekt := Artikel Substantiv

// Für Artikel, Substantiv und Prädikat werden durch Terminalsymbole ersetzt.
Artikel := die
Substantiv := Giraffe
Prädikat := schläft

// Alles wird zusammengefasst
Satz = die Giraffe schläft

// Da der Satz nur noch aus Nichtterminalsymbolen besteht, kann er nicht weiter verändert werden.
```