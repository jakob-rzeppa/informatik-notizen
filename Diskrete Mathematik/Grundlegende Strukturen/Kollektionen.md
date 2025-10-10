# Kollektionen

Kollektionen sind eine Art von [Modellen](Modellbildung.md). Mit ihnen können mehrere Objekte (andere Modelle) zusammengefasst werden.

## Formen von Kollektionen

Dabei können unterschiedliche Formen von Kollektionen genutzt werden. Diese hängen von zwei Aspekten ab:

- Die Reihenfolge der Objekte
- Mehrfachvorkommen oder kein Mehrfachvorkommen von Objekten

|  | Reihenfolge ist relevant | Reihenfolge ist nicht relevant |
|-:-|-:-|-:-|
| Mehrfachvorkommen ist relevant | [Tupel](Tupel.md) |  |
| Mehrfachvorkommen ist nicht relevant |  | [Mengen](Mengen.md) |

## Genestete Kollektionen

Kollektionen können ineinander genestet werden:

Ein geeignetes Modell für einen Funktionsgraphen ist die [Menge](Mengen.md) von 2-Tupeln. Jedes [Tupel](Tupel.md) beschreibt einen Punkt des Graphen:

$$
[1,2] \Rightarrow x = 1; y = 2
$$

$$
\Rightarrow [1,2] \neq [2,1]
$$

Jetzt wird eine Menge aller Punkte des Graphen erstellt:

$$
\{[1,2],[2,4],[3,6], \dots\}
$$

Dabei wird eine Menge verwendet, da die Reihenfolge und Mehrfachnennungen für den Graphen irrelevant sind. 