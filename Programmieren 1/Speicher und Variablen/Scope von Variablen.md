# Scope von Variablen

Variablen, die in einem Block definiert werden, sind, nur in diesem Aufrufbar.

> Für lokale Variablen wird zur Laufzeit Speicherplatz auf dem Stack vorgesehen, sobald die Ausführung des Blocks beginnt, in dem sie deklariert sind. Wenn die Lebensdauer einer Variable endet, wird der Speicher im [Stack](Stack.md) wieder freigegeben.

Dopplungen bei Variable-Identifier sind nur erlaubt, wenn die andere Variable von dem Punkt der Deklaration der neuen nicht erreichbar ist.