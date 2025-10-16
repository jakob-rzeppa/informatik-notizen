# Karnaugh-Vietch-Diagramme (KV-Diagramme)

KV-Diagramme werden für die übersichtliche Darstellung von boolschen Funktionen verwendet.

Ziel: Umwandlung einer disjunktiven Normalform in einen minimalen distinktiven logischen Ausdruck

> In der Prüfung werden KV-Diagramme für 4 Bits verwendet

## Übertragung von Wahrheitstafeln in KV-Diagramme

> In der Klausur wird wohl das Diagramm mit Zahlen vorgegeben => Jede Zeile der Tabelle in das entsprechende Fach eintragen. Falls tabelle nicht geordnet den Binärwert der Input-Bits nehmen (wenn Diagramm richtig gezeichnet).

Geordnetes Diagramm:

| A | B | y |
| --- | --- | --- |
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

Das Diagramm lässt sich auch selber herleiten. Jede kombination von Bits kann als 1er Block verstanden werden. Erstellt man jetzt ein KV-Diagramm (welche Variable wo ist in dem Fall egal) kann man jeden dieser 1er Blöcke in das Diagramm eintragen.

> Es ist einfacher entweder alle Einsen onder Nullen einzuragen und dann den Rest aufzufüllen.

## Vereinfachen mit dem KV-Diagramm

Bei dem Vereinfachen mit dem KV-Diagramm erstellt man (wenn alles richtig ist) die [Minimalform](Minimalform.md).

> Nur wenn alle großen Blöcke gefunden werden kann es sich um die minimalste Form handeln! Größere Blöcke sind immer kleineren vorzuziehen.

Von großen Blöcken zu kleinen gehen:

1. Ist ein 16er Block vorhanden?
2. Ist ein 8er Block vorhanden?
3. Ist ein 4er Block vorhanden?
4. Ist ein 2er Block vorhanden?
5. Ist ein 1er Block vorhanden?

Die entsprechenden Blöcke markieren und dann zu einer Formel zusammenfassen.

> Tipp: Für die Klausur Farben benutzen (außer Rot)