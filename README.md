# Fragenkatalog für „Paradigmen der Programmierung“

## Unix

* Beschreiben Sie ein allgemeines Unixsystem.
* Beschreiben Sie die Philosophien von Unix.
* Beschreiben Sie das Prinzip „alles ist eine Datei.“
  * Warum ist das sinnvoll?
  * Welches Paradigma wird dadurch implementiert?  (Pipe-Filter-Architektur bzw. Datenflussparadigma)
* Wo liegen in Unix/Linux die Gerätetreiber? In den Programmen oder im Kernel? (Kernel)
* Wenn man ein neues Gerät an den Computer anschließt, müssen Sie das dann in ihrer Anwendung berücksichtigen?
* Wenn ein C-Programm eine Minute läuft, kann man dann sicher sein, dass dann immer noch ein C-Programm läuft? Besonders im Hinblick auf den `exec`-Systemcall.
* Erklären Sie den Unterschied zwischen `fork()` und `exec()`.
* Was passiert genau bei \textt{fork()` und `exec()`?
* Wenn ein Programm mittels `fork()` ein Kindprogramm erzeugt, ab welchem Punkt findet dann die weitere Ausführung statt? (ab dem Aufruf von `fork()` und nicht von vorne)
* Wie baut man Pipes? Wie funktionieren Pipes?
* Was passiert beim Umleiten der Ausgabe eines Programms? Wie genau wird
  das in einer Shell gemacht?
* Warum sind *file descriptors* wichtig?
* Welche Standard-FDs bekommt jeder Prozess? (`stdin`, `stdout`, `stderr`)

## Haskell und Monaden

* Was ist eine Monade?
* Wofür braucht man Monaden?
* Betrachten wir die IO-Monade aus der Vorlesung: welchen Typ hat diese und wie ist der Bind-Operator ($\gge$) definiert? (auf „Weltzustand“ und „RealWorld“ eingehen)
* Wie funktioniert dann die sequentelle Berechnung/Ausführung von Funktionen?
* Was ist ein Monadentransformer?
* Wie sieht die Typklasse von Monadentransformern aus?
* Wie schafft man es einen Zustand (State) an eine andere Monade ranzubacken?

## Lisp

* Was ist so besonders an Lisp?
* Nennen Sie Unterschiede zwischen Lisp und Haskell.
* Was ist ein Makro in Lisp?
* Wie kann man ein Lisp-Programm mit Lisp verändern?
* Was ist eine Closure?
* Erklären Sie den Unterschied zwischen einem C- und einem Lisp-Makro.
* Erklären Sie den Unterschied zwischen einer Haskell- und einer Lisp-Closure.
