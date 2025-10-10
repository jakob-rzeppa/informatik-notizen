# Objekte

> "Ein Objekt ist die Instanz der Klasse"

Objekte werden im [Heap](Heap.md) gespeichert und deren Referenzvariable im [Stack](Stack.md).

## Encapsulation / Kapselung

Q: Was ist Encapsulation / Kapselung?
A: Daten und Verhalten werden zu einer Einheit zusammengefasst. Dabei wird klasseneigene Logik von der "Außenwelt" abgeschnitten und nur über eine Schnittstelle erreichbar gemacht.
<!--ID: 1758959238140-->

## Inheritance / Vererbung

Attribute und Methoden können an Sub-Klassen vererbt werden.

## Polymorphie

Q: Was ist Polymorphie?
A: Wenn eine Methode eines Objektes aufgerufen wird, wird erst dann bestimmt, welche genau verwendet wird. Demnach kann eine Methode mehrdeutig sein. Wird über Vererbung genutzt. 
<!--ID: 1758959238145-->

Mit Polymorphie können Objekte unterschiedlicher Klassen in ein Array zusammengefasst werden, wo auf die Parent-Klasse verwiesen ist. Demnach kann ein Array Car mit den Objekten Audi, VW etc. gefüllt werden.

```Java
Car[] cars = new Car[2];

// Golf und Audi erben von Car
cars[0] = new Golf();
cars[1] = new Audi();

for (int i = 0; i < cars.length; i++) {
	// Methoden, die in Car deklariert sind können verwendet werden.
	cars[i].drive();
}
```
