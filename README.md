# Fragenkatalog für „Paradigmen der Programmierung“

## Unix

* Beschreiben Sie ein allgemeines Unixsystem.
* Beschreiben Sie die Philosophien von Unix.
* Beschreiben Sie das Prinzip [„alles ist eine Datei.“](https://en.wikipedia.org/wiki/Everything_is_a_file)
  * Warum ist das sinnvoll?
  * Welches Paradigma wird dadurch implementiert?  ([Pipe-Filter-Architektur](https://de.wikipedia.org/wiki/Pipes_und_Filter) bzw. Datenflussparadigma)
* Wo liegen in Unix/Linux die Gerätetreiber? In den Programmen oder im Kernel? (Kernel)
* Wenn man ein neues Gerät an den Computer anschließt, müssen Sie das dann in ihrer Anwendung berücksichtigen? (Nein)
* Wenn ein C-Programm eine Minute läuft, kann man dann sicher sein, dass dann immer noch ein C-Programm läuft? Besonders im Hinblick auf den [`exec`-Systemcall](https://en.wikipedia.org/wiki/Exec_(system_call)).
* Erklären Sie den Unterschied zwischen `fork()` und `exec()`.
* Was passiert genau bei [`fork()` und `exec()`](https://en.wikipedia.org/wiki/Fork%E2%80%93exec)?
* Wenn ein Programm mittels `fork()` ein Kindprogramm erzeugt, ab welchem Punkt findet dann die weitere Ausführung statt? (ab dem Aufruf von `fork()` und nicht von vorne)
* Wie baut man Pipes? Wie funktionieren [Pipes](https://de.wikipedia.org/wiki/Pipe_(Informatik))?
* Was passiert beim Umleiten der Ausgabe eines Programms? Wie genau wird das in einer Shell gemacht?
* Wann werden bei einer Pipe die FD der Kommandos umgelenkt? (zwischen Fork und Exec)
* Warum sind *file descriptors* wichtig?
* Welche Standard-FDs bekommt jeder Prozess? (`stdin`, `stdout`, `stderr`)

## Haskell und Monaden

* Was ist eine Monade? ([siehe z.B. die Typeclassopedia](https://wiki.haskell.org/Typeclassopedia))
* Wofür braucht man Monaden?
* Betrachten wir die IO-Monade aus der Vorlesung: welchen Typ hat diese und wie ist der Bind-Operator (`>>=`) definiert? (auf „Weltzustand“ und „RealWorld“ eingehen)
* Wie funktioniert dann die sequentelle Berechnung/Ausführung von Funktionen?
* Was ist ein Monadentransformer?
* Wie sieht die Typklasse von Monadentransformern aus?
* Wie schafft man es einen Zustand (State) an eine andere Monade ranzubacken?

## Lisp

* Was ist so besonders an Lisp?
* Nennen Sie Unterschiede zwischen Lisp und Haskell.
* Was ist ein Makro in Lisp?
* Wie kann man ein Lisp-Programm mit Lisp verändern?
* Was ist eine [Closure](https://de.wikipedia.org/wiki/Closure_(Funktion))?
* Erklären Sie den Unterschied zwischen einem C- und einem Lisp-Makro.
* Erklären Sie den Unterschied zwischen einer Haskell- und einer Lisp-Closure.
* Was kann man mit Lisp-Closures nicht implementieren? (Nichts, man kann alles implementieren)
