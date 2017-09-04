# C und Python Tutorial
## Python
### Overview
[Overview](https://www.tutorialspoint.com/python3/python_overview.htm)


### Environment Setup
```python
#!/usr/bin/python3
print ("Hello, Python!")
```
  * Online Compiler  
  Testen eines Python-Scripts mithilfe eines Online-Compilers.  
  z.B. unter [Python Online Environment](https://www.tutorialspoint.com/execute_python3_online.php)<br><br>
  * Locale Umgebung  
  siehe [Setup](https://www.tutorialspoint.com/python3/python_environment.htm)
    * Installation von Python
    * Die "PATH-Variable" setzen
    * eventuell Python Umgebungsvariablen setzen
    * Python Programme starten
      * Interaktiver Interpreter  
      Eingabe von **python** von der Kommandozeile
      * Python-Script von der Kommandozeile starten  
      Unterschied zwischen "**script.py**" oder "**python script.py**" beachten. Unter Linux auf das **x**-Recht achten.
    * Integrierte Entwicklungsumgebungen (IDEs)  
    z.B. IDLE unter Linux<br><br>


### Basic Syntax
siehe [Syntax](https://www.tutorialspoint.com/python3/python_basic_syntax.htm)
#### Reservierte Wörter
In Python gibt es viele reservierte Wörter wie "and, exec, break, ...", die nicht als Variablennamen oder Klassennamen verwendet werden dürfen.
#### Zeilen und Einrückungen
Python verwendet keine Klammern ((),{}) für Code- und Klassen- und Funktions-Blockstrukturen. Blöcke werden in Python durch Zeileneinrückungen gesteuert.
```python
...
if True:
  print("True")
else:
  print("False")
...
```
#### Multi-Line Statements
Programmzeilen können in Python über meherer Zeilen gehen.
```python
total = item_one + \
        item_two + \
        item_three
```
#### Quotation in Python
#### Kommentare in Python
#### User Input
#### Mehrere Programmzeilen in einer Zeile
#### Gruppierung, Blockstruktur

### Variablen Typen
siehe [Python Variablen](https://www.tutorialspoint.com/python3/python_variable_types.htm)  
Python benötigt keine explizite Deklaration von Variablen. Die Deklaration passiert automatisch sobald ein Wert zugewiesen wird (= ist der Zuweisungsoperator)
```python
counter = 100
miles   = 1000.0
name    = "John"
```

#### Mehrere Zuweisungen
In Python möglich:
```python
a = b = c = 1
a, b, c = 1, 2, "john"
```

#### Standard Datentpen
* Numbers  
```python
var1 = 10
var2 = 11.01
var3 = 6.5+3.14j
```
Python kennt drei verschiedene numerische Typen:
  * int (signed integers)
  * float (floating point real values)
  * complex (complex numbers)<br><br>
* Strings  
Strings in Python sind definiert als eine kontinuierliche Folge von Zeichen. Diese werden durch Anführungszeichen (', ") begrenzt. Teilstrings kann durch den slice-Operator extrahieren. Der Unterschied zu klassischen Arrays in C ist, dass alle Listenelemente verschiedene Datentypen haben können.
```python
str = 'Hello World!'
print(str)
print(str[0])
print(str[2:5])
```
* List  
Listen sind die vielseitigsten Datentypen in Python. Eine Liste enthält Elemente, welche durch Beistriche getrennt werden.
```python
list = ['abcd', 786, 2.23, 'john', 70.2]
tinylist = [123, 'john']
print(list)
print(list[0])
print(str[1:3])
print(list + tinylist)
```
* Tuples  
Tuples sind eine andere Sequenz von Datentypen ähnlich den Listen. Die Elemente werden durch Beistriche getrennt und durch runde Klammern begrenzt. Der Hauptunterschied zwischen Listen und Tuples ist der das Listen geändert werden können, wohingegen Tuples nur read-only sind.
```python
tuple = ('abcd', 786, 2.23, 'john', 70.2)
tinytuple = (123, 'john')
print(tuple)
print(tuple[0])
print(tuple[1:3])
print(tuple + tinytuple)
```
* Dictionary  
Dictionaries sind eine Art von Hash-Table. Sind sind vergleichbar mit assiziative Arrays in PHP und bestehen aus Schlüssel-Wert Paaren. Sie werden in geschwungenen Klammern eingeschlossen.
```python
dict = {}
dict['one'] = "This is one"
dict[2]     = "This is two"
tinydict = {'name': 'john', 'code':6734, 'dept': 'sales'}
print(dict['one'])
print(dict[2])
print(tinydict.keys())
print(tinydict.values())
```

#### Datentypkonvertierungen
Es gibt viele eingebaute Konvertierungsfunktionen in Python.  
z.B. **int(x[,base])** --> Konvertiert x in eine Integerzahl. Base spezifiziert die Basis von x.

### Basisoperatoren
Python unterstützt die folgenden Operatoren:
* Arithmetische Operatoren (+, -, \*, /, %, \*\*, ...)
* Vergleichsoperatoren (==, !=, <, ...)
* Zuweisungsoperatoren (=, +=, \*=, ... )
* Logische Operatoren and, or, not)
* Bit Operatoren (&, |, ^, ~, <<, >>)
* Zugehörigkeit(Membership) Operatoren (in, not in)
* Gleichheits(Identity) Operatoren (is, is not)

#### Operatoren Reihenfolge
Wie in jeder Programmiersprache ist die Reihenfolge der Operatoren zu beachten. Die Reihenfolge kann durch Klammerung beeinflusst werden. Alle non-zero und non-null Werte werden als TRUE interprediert.

### Verzweigungen
Klassische if/else-Struktur, welche auf einer TRUE/FALSE-Entscheidung beruht.
![decision](pic/decision.gif)
* if statements
* if...else statements
* nested if statements

### Schleifen
Normalerweise wird ein Programm Codezeile für Codezeile abgearbeitet. Es gibt aber viele Situationen, wo ein anderer Codeablauf gewünscht wird. Mir Hilfe von Schleifenkontrukten ist es mögliche Codeabschnitte mehrmals zu wiederholen.  
![loops](pic/loops.gif)  
Python unterstützt folgende Schleifenkontrukte:
* while loop
* for loop
* nested loop

#### Schleifen Control Elemente
* break statement
* continue statement
* pass statement

### Numbers
siehe [Numbers](https://www.tutorialspoint.com/python3/python_numbers.htm)

### Strings
siehe [Strings](https://www.tutorialspoint.com/python3/python_strings.htm)

### Lists
siehe [Lists](https://www.tutorialspoint.com/python3/python_lists.htm)

### Tuples
siehe [Tuples](https://www.tutorialspoint.com/python3/python_tuples.htm)

### Dictionary
siehe [Dictionary](https://www.tutorialspoint.com/python3/python_dictionary.htm)

### Funktionen
Funktionen sind Blöcke von Code um eine einmalige Aktion wiederwerwendbar auszuführen. Funktionen ermöglichen eine bessere Wiederverwendbarkeit und Modularität eines Programms.  
Python hat viele built-in-Funktionen (z.B. print, abs, ...), aber man kann auch eigene Funktionen (user-defined functions) definieren.   
siehe [Functions](https://www.tutorialspoint.com/python3/python_functions.htm)

#### Funktion definieren
* eine Funktion beginnt mit dem Schlüsselwort **def** gefolgt vom Funktionsnamen und runden Klammern
* Übergabeparameter werden innerhalb der runden Klammern platziert
* Die erste Zeile kann optional als Dokumentation der Funktion verwendet werden.
* Der Code-Block startet mit einem **:** und ist eingerückt
* Die **return[...]** Zeile beendet die Funktion

Syntax:
```python
def functionname(parameters):
  "function_docstring"
  function_suite
  return [expression]
```

Beispiel:
```python
def printme(str):
  "This prints a passed string into this function"
  print(str)
  return
```

#### Funktionen aufrufen
Der Aufruf der Funktion erfolgt durch Angabe des Funktionsnamens mit der Übergabe der entsprechenden Parameter.
```python
...
printme("Erste Ausgabe")
printme("Zweite Ausgabe")
```

#### Übergabe per Reference versus Value
In Python werden alle Übergabeparameter einer Funktion als Referenz übergeben. Dies bedeutet, falls der Wert eines Übergabeparamters geändert wird, so ändert sich auch der Wert der innerhalb der aufrufenden Funktion.  
siehe Beispiele in  [Functions](https://www.tutorialspoint.com/python3/python_functions.htm)

#### Globale versus lokale Variablen
Variablen welche innerhalb einer Funktion definiert sind haben eine lokale Sicht, wohingegen Variablen die außerhalb einer Funktion definiert sind eine globale Sicht haben. Dies bedeutet, dass auf lokale Variablen nur innerhalb einer Funktion zugegriffen werden kann. Auf globale Variablen kann sowohl innerhalb als auch außerhalb einer Funktion zugegriffen werden.
```python
#!/usr/bin/python3

total = 0
def sum(arg1, arg2):
  total = arg1 + arg2
  print("inside the function local total : ", total)
  return total

sum(10, 20)
print("Outside the function global total : ", total)

Inside the fuction local total : 30
Outside the function global total : 0
```

### Module
Module erlauben den Code logisch zu organisieren. Einfach ausgedrückt ist ein Modul ein File welches aus Python-Code besteht. Ein Modul kann Funktionen, Klassen, Variablen und ausführbaren Code beinhalten.  
siehe [Module](https://www.tutorialspoint.com/python3/python_modules.htm)  
Ein Modul wir also in einem file (z.B. "module1.py") geschrieben und mit dem import-Befehl (import module1) importiert.  
z.B. file mod1.py
```python
def print_func(par):
  print "Hello : ", par
  return
```
wird wie folgt importiert
```python
#!/usr/bin/python3
import mod1

mod1.print_func("Zara")
```

#### from...import
Mit der from Anweisung werden nur spezifische Teile eines Moduls importiert.  
Syntax:
```python
from modname import name1[, name2[, ... nameN]]
```

#### Namespaces and Scopes
Variablennamen gehören zu einem Objekt. Ein Namespace ist ein dictionary von Variablennamen (keys) und deren zugehörigen Objekten (values).
* Ein Python statement kann auf Variablen im lokalen und globalen Namespace zugreifen. Die lokale Variable deckt die globale Variable zu.
* Jede Funktion und Klasse hat seinen eigenen Namespace
* Python definiert jede Variable die einen Wert zugewiesen bekommt als lokal an.
* Um einer globalen Variblen innerhalb einer Funktion einen Wert zuzuweisen, muss sie vorher als global deklariert werden.
* Das global-Statement teilt mit, dass es sich um eine globale Variable handelt. Python beendet damit die Suche innerhalb des lokalen Namespaces.

Der folgende Code erzeugt einen "UnboundLocalError". Durch auskommentieren der Zeile "global Money" kann dieser Fehler behoben werden.
```python
#!usr/bin/python3
Money = 2000
def AddMoney():
  # global Money
  Money = Money + 1

print(Money)
AddMoney()
print(Money)
```

### Date & Time
Python Programme können Datum und Zeit auf verschiedene Arten behandeln. Die Umwandlung zwischen verschiedenen Datumsformaten ist eine übliche Aufgabe eines Computers. Die Python-Module "time" und "calendar" unterstützen bei diesen Aufgaben.  
siehe [Date and Time](https://www.tutorialspoint.com/python3/python_date_time.htm)

#### Tick
Zeitintervalle sind floating-point Zahlen in Sekundeneinheit. Diese werden in Sekunden sein dem 1.1.1970 (12am) gerechnet.  
Das time-Modul stellt entsprechende Funktionen zur Verfügung.
```python
#!usr/bin/python3
import time;

ticks = time.time()
print("Number of ticks since 12:00am, January 1, 1970:", ticks)
```


#### TimeTuple
Viele der time-Funktionen behandeln die Zeit mit einem Tuple von 9 Zahlen.  
```python
#!usr/bin/python3
import time;

print(time.localtime());

time.struct_time(tm_ear = 2016, tm_mon = 2, tm_mday = 15, tm_hour = 9,
  tm_min =29, tm_sec = 2, rm_wday = 0, tm_yday = 46, tm_isdst = 0)
```

#### Formatierte Zeit
Mit der Funktion asctime() kann man die Zeit in eine beliebig formatierte Zeitangabe umwandeln.
```python
#!usr/bin/python3
import time;

localtime = time.asctime(time.localtime(time.time()))
print("Local current time :", localtime)

Local current time : Mon Feb 15 09:34:03 2016
```
Für zusätzliche time- und calendar-Funktionen siehe [Date and Time](https://www.tutorialspoint.com/python3/python_date_time.htm)

### File I/O
#### Printing to the Screen
```python
#!usr/bin/python3
print("Python is really a great language,", "isn't it?")
```

#### Reading Keyboard Input
* python2 - hat 2 eingebaute Funktionen: input() und raw_input()
* python3 - es soll nur mehr die input()-Funktion verwendet werden. Die raw_input()-Funktion ist veraltet.

```python
#!usr/bin/python3
x = input("Give me input: ")
...
```

#### Öffnen und Schließen von files
Syntax:
```python
file object = open(file_name [, access_mode][, buffering])
```
* file_name - der Filename als string des zu öffnenden files
* access_mode - bestimmt des Modus (Rechte - read, write, append) des öffnenden files
* buffering
  * 0 - keine Bufferung
  * 1 - Zeilenweise buffern
  * \>1 - Wert entspricht der Buffergröße
  * <0 - System default Buffergröße

#### File Object Attribute
Nachdem das File geöffnet ist, kann man mehrere Attribute abrufen:
* file.closed
* file.mode
* file.name

```python
#!usr/bin/python3
fo = open("foo.txt", "wb")
print("name of the file: ", fo.name)
print("Closed or not: ", fo.closed)
print("Opening mode: ", fo.mode)
fp.close()
```

#### Reading and Writing Files
* write()  
```python
#!usr/bin/python3
fo = open("foo.txt", "w")
fo.write("Python is a great language.\n")
fp.close()
```
* read()
```python
#!usr/bin/python3
fo = open("foo.txt", "r+")
str = fo.read(10)
print("Read String is: ", str)
fp.close()
```

#### Weitere Filefunktionen
* File Position - tell(), seek(offset[, from])
* Renaming and Deleting Files - über das Python **os**-Modul
* Verzeichnisse in Python - mkdir(), chdir(), getcwd(), rmdir()


### Exceptions
Python stellt 2 sehr wichtige Features zur Behandlung von unerwarteten Fehlern und debugging-Möglichkeiten zur Verfügung.
* Exception Handling
* Assertions

#### Standard Exceptions
siehe [Exceptions](https://www.tutorialspoint.com/python3/python_exceptions.htm)  
Ein Exception ist ein Event, welcher bei der Ausführung eines Programms auftritt und den normalen Programmablauf unterbricht. Wenn ein Python Programm eine exception aufruft, muss diese behandelt werden oder das Programm terminiert und beendet sich.

#### Exception Handling
Die Behandlung von Exceptions wird mit **try** und **except**-Blöcken behandelt.  
Syntax:
```python
try:
  You do our operation here
  .......................
except ExceptionI:
  If there is ExceptionI, then execite this block.
except ExceptionII:
  If there is ExceptionII, then execite this block.
  ................
else:
  If there is no exception, then execite this block.
```

Beispiel:
```python
#!/usr/bin/python3
try:
  fh = open("testfile", "w")
  fh.write("This is may test file fpr exception handling!!")
except IOError:
  print("Erros: can\'t find or read data")
else:
  print("Written content in the file successfully")
  fh.close()
```

### Links
[Holzapfel](http://www.michael-holzapfel.de/)  
[Thomas Güttler](http://www.thomas-guettler.de/vortraege.html)  
[Python Kurs](http://www.python-kurs.eu/python3_kurs.php)  
[Uni Jena](http://www.uni-jena.de/unijenamedia/python-p-10631.pdf)  
[Uni Rostock](http://www.informatik.uni-rostock.de/~nl/files/loi/aufgaben/blatt1)  

---

## C
### Overview
[Overview](https://www.tutorialspoint.com/cprogramming/c_overview.htm)

### Environment Setup
```C
#include <stdio.h>
int main() {
   // my first program in C
   printf("Hello, World! \n");

   return 0;
}
```
  * Online Compiler  
  Falls kein lokaler Compiler installiert wurde, kann man ein C-Programm auch mit einer Online-Umgebung testen.  
  Als Beispiel die Online-Umgebung von TutorialsPoint: [C Online Environment](https://www.tutorialspoint.com/compile_c_online.php)
  ![onlinecompiler](pic/onlinecompiler.gif)
  <br><br>
  Noch eine Online-Umgebung von Codechef: [Codechef Online Environment](https://www.codechef.com/ide)  
  Noch eine Online-Umgebung von ideone: [ideone Online Environment](https://ideone.com/)<br><br>
  * Locale Umgebung  
  siehe [Setup](https://www.tutorialspoint.com/cprogramming/c_environment_setup.htm)
    * Installation eines C-Compilers
    * Auswahl eines entsprechenden Text-Editors
    * eventuell "PATH-Variable" setzen
    * Compilieren (z.B. gcc hello.c)
    * Starten eines compilierten Programms (z.B. ./a.out)
    * Integrierte Entwicklungsumgebungen (IDEs)

### Programm Struktur
Ein C-Programm besteht aus folgenden Teilen:
* Preprocessor Commands
* Functions
* Variables
* Statements & Expressions
* Kommentaren (Comments)

```C
#include <stdio.h>
int main() {
   // my first program in C
   printf("Hello, World! \n");

   return 0;
}
```
* **#include <stdio.h>** ist ein Preprocessor Kommando
* **int main()** ist die Hauptfunktion wo die Programmausführung beginnt
* **// my first ...** ist eine Kommentarzeile. Diese wird beim compilieren ignoriert
* **printf(...)** ist ein Funktionsaufruf, welcher in C vorhanden ist.
* **return 0** ist ein Statement, welches die Hauptfunktion main() beendet.

#### Compilieren und Ausführen eines C-Programms
* Schreiben des Programmcodes mit einem Text-Editor
* Abspeichern als \*.c file (z.B. hello.c)
* Öffne eine Shell oder einen Kommandointerpreter und wechsle in das Verzeichnis wo du das .c file gespeichert hast.
* compiliere das Programm mit "*gcc hello.c*"
* falls keine Fehler auftreten erzeugt der Compiler ein ausführbares file mit dem Namen a.out (x-Rechte unter Linux beachten)
* Starte das Programm mit *a.out* (oder *./a.out*)
* Die Ausgabe "*Hello World*" sollte auf dem Bildschirm erscheinen

```sh
$ gcc hello.c
$ ./a.out
Hello, World!
```

### Basic Syntax
siehe [Basic Syntax](https://www.tutorialspoint.com/cprogramming/c_basic_syntax.htm)

#### Semicolons
Jede Zeile (Statement) in C endet mit einem Semicolon
```C
printf("Hello, World! \n");
return 0;
```

#### Kommentare
* Zeilenweise Kommentare (**// ...**)
* Mehrzeilige Kommentare (**/\* ... \*/**)

#### Identifiers
