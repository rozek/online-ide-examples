Dieses Repository enthält eine Reihe von Java-Beispielen zur Verwendung in der [Online-IDE](https://github.com/martin-pabst/Online-IDE) von [Martin Pabst](https://github.com/martin-pabst).

Zwar wurden die Beispiele primär für den Kurs "Grundlagen der Informatik" an der [Hochschule für Technik](https://www.hft-stuttgart.de/) in Stuttgart entwickelt, vermutlich können sie aber genauso gut auch in anderen Lehrveranstaltungen eingesetzt werden.

**Falls Sie gerade die README-Datei aus diesem Repository lesen, wechseln Sie bitte auf die zugehörige [GitHub Page](https://rozek.github.io/online-ide-examples/), um die Online-IDE in Aktion zu sehen und damit zu arbeiten.**

> Nota bene: dieser Beitrag befindet sich gerade in Arbeit und wird vermutlich nicht vor Ende des lfd. Semesters fertiggestellt werden

### Zusätzliche Hinweise ###

Eine Beschreibung der von der "Online-IDE" bereitgestellten System-Klassen und -Schnittstellen finden Sie unter [https://www.online-ide.de/api_documentation.html](https://www.online-ide.de/api_documentation.html)

### ASCII-Tabelle ###

Das folgende Beispiel erstellt eine kleine "ASCII-Tabelle", bestehend aus den druckbaren (Unicode-)Zeichen mit den Codes 0...255

<iframe src="ASCII-Tabelle.html" style="width:800px; height:400px; overflow:hidden"></iframe>

### Newton-Verfahren ###

Das [Newton-Verfahren](https://de.wikipedia.org/wiki/Newtonverfahren) ermöglicht die (näherungsweise) Bestimmung von Nullstellen nicht-linearer Gleichungen (die mathematischen Voraussetzungen für die Anwendbarkeit des Newton-Verfahrens sollen hier nicht erläutert werden)

![](https://upload.wikimedia.org/wikipedia/commons/c/c9/Newtonsches_N%C3%A4herungsverfahren.png)<br>(Quelle: Sebastian Queißer auf Wikipedia, Lizenz: [Creative Commons Attribution-Share Alike 3.0 Unported](https://creativecommons.org/licenses/by-sa/3.0/deed.en))

Aus dem Diagramm lässt sich leicht ablesen:

![](https://www.rozek.de/GDI/GDI-02/Newton-I.png)

oder

![](https://www.rozek.de/GDI/GDI-02/Newton-II.png)

Die Approximationsanweisung lautet somit:

![](https://www.rozek.de/GDI/GDI-02/Newton-III.png)

Das folgende Java-Beispiel berechnet die genäherte Lösung für die Gleichung

x<sup>2</sup>-4 = 0

<iframe src="Newton-Verfahren.html" style="width:800px; height:400px; overflow:hidden"></iframe>

### Monte-Carlo-Verfahren ###

Das Monte-Carlo-Verfahren ermöglicht die Lösung bestimmter mathematischer und physikalischer Probleme mittels stochastischer Methoden - zum Beispiel die Bestimmung der Kreiszahl π.

![](https://www.rozek.de/GDI/GDI-02/MonteCarlo-Illustration.png)

* Quadratfläche: ![](https://www.rozek.de/GDI/GDI-02/Monte-Carlo-I.png)
* Kreisfläche: ![](https://www.rozek.de/GDI/GDI-02/Monte-Carlo-II.png)
* Flächenverhältnis: ![](https://www.rozek.de/GDI/GDI-02/Monte-Carlo-III.png)

Bei gleichmäßiger Verteilung der Testpunkte ("Nadelstiche") entspricht das Verhältnis der Punkte in zwei Flächen dem Verhältnis der Flächeninhalte.

Man muss also nur zählen, wieviele Nadelstiche im Quadrat und wieviele im Kreis liegen.

Das folgende Beispiel zeigt eine mögliche Implementierung:

<iframe src="Monte-Carlo-Verfahren.html" style="width:800px; height:400px; overflow:hidden"></iframe>

### Sukzessive Approximation ###

Die sukzessive Approximation (lateinisch für: schrittweise Annäherung) ist ein Iterationsverfahren zur Annäherung an einen gesuchten (Funktions-)Wert, welches unter bestimmten Voraussetzungen sehr schnell zu einem sehr genauen Ergebnis führt.

Wird das Verfahren zur Berechnung eines Funktionswertes verwendet, sollten folgende Voraussetzungen erfüllt sein:

* die Funktion selbst sollte schwierig,
* die Umkehrfunktion jedoch einfach zu berechnen sein,
* außerdem muss die Funktion streng monoton verlaufen.

Die Vorgehensweise entspricht dem bekannten Witz "wie fängt ein Mathematiker eine Fliege in einem Raum?". Die Antwort: "er halbiert den Raum und prüft, in welcher Hälfte sich die Fliege befindet. Anschließend wiederholt er das Verfahren für die Hälfte mit der Fliege - so oft, bis der Raum so klein ist, daß sich die Fliege nicht mehr bewegen kann. Damit ist die Fliege gefangen."

#### Berechnung der Quadratwurzel ####

Für die Berechnung der Quadratwurzel sind die oben genannten Bedingungen erfüllt, sofern man sich auf positive oder negative Werte beschränkt.

<iframe src="Quadratwurzel.html" style="width:800px; height:400px; overflow:hidden"></iframe>



#### Berechnung von MAX_SAFE_INTEGER ####

<iframe src="MAX_SAFE_INTEGER.html" style="width:800px; height:400px; overflow:hidden"></iframe>



## Lizenz ##

Dieser Beitrag steht unter [MIT Lizenz](LICENSE.md)
