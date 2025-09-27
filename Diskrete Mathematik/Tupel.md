# Tupel

Q: Was ist ein Tupel?
A: Ein Tupel ist eine Art von [[Kollektionen|Kollektion]], wo die Reihenfolge und ob die Komponenten mehrfach vorkommen relevant ist.
<!--ID: 1758976670717-->

Q: Bezeichnung der Objekte eines Tupels
A: Die Objekte eines Tupels werden *Komponenten* genannt.
<!--ID: 1758976773442-->

## Definition (In diesem Kurs)

Tupel werden in diesem Kurs durch eckige Klammern gekennzeichnet.

Das Tupel $[D,e,f,i,n,i,t,i,o,n]$ ist das beste Modell für die Kollektion der Buchstaben des Wortes Definition, da Mehrfachnennungen und Reihenfolge relevant sind.

$$
[1,2,3] \neq [2,1,3]
$$

Darin unterscheiden sie sich von [[Mengen]], bei welchen die Reihenfolge und Mehrfachnennungen irrelevant sind:

$$
\{1,2,3\} = \{2,1,3\}
$$

$$
\{1,2,3\} = \{1,2,3,3\}
$$

Deshalb ist eine Menge kein gutes Modell für die Kollektion der Buchstaben des Wortes Definition:

$$
\{D,e,f,i,n,i,t,i,o,n\} = \{e,f,i,n,t,i,D,o,n,i\}
$$

$$
\{D,e,f,i,n,i,t,i,o,n\} = \{D,e,f,i,n,t,o\} \text{ (Mehrfachnennungen nicht relevant)}
$$


## Benennung von Tupel

Tupel werden nach der Anzahl der Komponenten benannt: 2-Tupel, 3-Tupel etc.