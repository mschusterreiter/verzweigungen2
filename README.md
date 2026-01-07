# Übung 3 - Operatoren

**Achtung:** Die beiliegende Main-Klasse beinhaltet die Testfälle für die Aufgaben 1, 2 und 3. 
Wenn Sie vorerst nur eine der drei Aufgaben testen wollen, kommentieren Sie die Testfälle 
der anderen Aufgaben in der Main-Klasse aus.

## 1. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML1.png" alt="Bildbeschreibung" />
</p>

**Spezifikationen:**
- Im Konstruktor müssen statt der Zuweisung die `set`-Methoden aufgerufen werden.
- Die Parameternamen des Konstruktors müssen gleich den Eigenschaftsnamen sein. 
- `print()`: Gibt alle Eigenschaften in der Konsole aus. Folgendermaßen soll die Ausgabe aussehen: 
##############################  
\## Linienbus: true  
\## Anzahl Sitzplätze: 50
\## Firma: Musterbus GmbH 
\## Anzahl Sitzplätze besetzt: 0  
\##############################
- `èinsteigen(int anzahl)`: Es steigen Leute in den Bus ein. Prüfen Sie, ob eine gültige Zahl eingegeben wurde und ob genug Platz im Bus ist. Ist die Zahl gültig und es ist genug Platz im Bus, dann dürfen die Personen einsteigen. Wenn eine der beiden Bedingungen nicht erfüllt ist, darf niemand einsteigen. Geben Sie in beiden Fällen eine Meldung aus. Welche Variable müssen Sie verändern?
- `aussteigen(int anzahl)`: Es wollen Leute aus dem Bus aussteigen. Prüfen Sie, ob eine gültige Zahl eingegeben wurde. Wenn schon, dann dürfen die Personen aussteigen. Wenn nicht, dann darf niemand aussteigen. Geben Sie in beiden Fällen eine Meldung aus.
- `allesAussteigen()`: Endstation! Alle müssen aussteigen.
- `besetzt()`: Gibt zurück, ob der Bus bereits voll ist oder nicht. 

**Hinweis:** Es gibt keine Stehplätze.

## 2. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML2.png" alt="Bildbeschreibung" />
</p>

Es soll das Minimum von zwei, drei und vier Zahlen zurückgegeben werden. Suchen Sie selbst nach einer Lösung ohne Hilfe des Internets und ohne Verwendung der `Math`-Klasse. Wenn Ihnen mehrere Ansätze einfallen, programmieren Sie diese gerne auch.

## 3. Aufgabe


Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML3.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Eigenschaften:**
- `miete` muss größer 0 sein. 
- `anzahlTiere` muss größer 0 sein und kleiner gleich `maxAnzahlTiere`.
- `maxAnzahlTiere` muss größer 0 sein. 
- Wenn die `miete` größer 1000 ist, müssen mindestens 100 Tiere in der Tierhandlung sein. 

Prüfen Sie die Bedingungen an der geeigneten Stelle. Falls eine Bedingung nicht erfüllt ist, setzen Sie den Defaultwert und geben Sie eine Fehlermeldung aus.

**Beschreibung der Methoden:**
- Im Konstruktor müssen statt der Zuweisung die set-Methoden aufgerufen werden.
- Die Parameternamen des Konstruktors müssen gleich den Eigenschaftsnamen sein.
- `printTierhandlung()`: Gibt alle Eigenschaften in der Konsole aus. Wenn die Tierhandlung geöffnet ist, soll nicht true ausgegeben werden, sondern „geöffnet“. Wenn die Tierhandlung geschlossen ist, soll nicht false, sondern „geschlossen“ ausgegeben werden. Folgendermaßen soll die Ausgabe aussehen:
 ##############################  
\## Besitzer: Toni Tierlieb  
\## Anzahl Tiere: 5
\## Maximale Anzahl Tiere: 10
\## Miete: 100.0
\## Offen: Geöffnet  
\##############################
- `tierVerkauf(int anzahl)`: Es sollen `anzahl` Tiere verkauft werden. `anzahl` muss größer 0 sein. Welche Bedingung muss `anzahl` (sinnvollerweise) noch erfüllen? Außerdem darf nur eingekauft werden, wenn die Tierhandlung geöffnet ist. In jedem Fall soll eine entsprechende Meldung ausgegeben werden.
- `mieteErhoehen(int prozent)`: Die Miete soll um `prozent` erhöht werden. `prozent` muss größer 0 sein.
- `voll()`: Gibt zurück, ob die Tierhandlung bereits voll ist oder nicht.
