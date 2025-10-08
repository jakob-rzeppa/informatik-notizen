# Typecasts

Wenn ein anderer Datentyp benötigt ist, als bei einer Variable vorhanden kann ein Typecast durchgeführt werden. D. h. eine Variable wird von einem Typen in einen anderen überführt.

Dabei gibt es *explizite* und *implizierte* Typecasts.

## Implizierte Typecasts (Widening)

Java kann, wenn keine Daten verloren gehen impliziert Typecasten - also z. B. wenn man ein Integer zu einem Long überführt. Dabei muss der Entwickler nichts weiter beachten.

|Von Typ|Zu Typ möglich (implizit)|
|---|---|
|`byte`|`short`, `int`, `long`, `float`, `double`|
|`short`|`int`, `long`, `float`, `double`|
|`char`|`int`, `long`, `float`, `double`|
|`int`|`long`, `float`, `double`|
|`long`|`float`, `double`|
|`float`|`double`|
|`double`|_(kein impliziter Cast möglich)_|
|`boolean`|_(keine Konvertierung zu/von anderen Typen möglich)_|

## Explizite Typecasts (Narrowing)

Wenn ein Type von Java nicht direkt überführt werden kann, muss das explizit gefordert werden.

```java
double d = 2.5;

int i = (int) d;
// i = 2
```