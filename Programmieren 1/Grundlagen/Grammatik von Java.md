# Grammatik von Java

Die Grammatik von Java ist eine [kontextfreie Grammatik](kontextfreie%20Grammatik.md).
 
Nichtterminalsymbole von Java:

```
// Nur ein kleiner Teil der Nichtterminalsymbole als Beispiel

Block:
	{ [BlockStatements] }
	
BlockStatements:
	BlockStatement {BlockStatement}
	
BlockStatement:
	Statement
	ClassDeclaration
	...
	
Statement:
	WhileStatement
	...
```

Durch das Ersetzen der Nichtterminalsymbole durch weitere Nichtterminalsymbole (Block -> BlockStatements -> Statement -> WhileStatement etc.) bis am Ende zu den Terminalsymbolen ("while (i < 7) { ... }") entsteht der Java Code bzw. die [Sprache](Sprache.md) Java. Das Startsymbol ist der Block.