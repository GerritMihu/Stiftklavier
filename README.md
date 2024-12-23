# Stiftklavier
 
# Dokumentation Stylophon / Stiftklavier

### 1. Platine bestücken

Beim Bestücken einer Platine wird immer so vorgegangen, dass man mit den kleinsten Bauteilen (Kondensatoren, Widerstände und Dioden) anfängt und sich immer weiter bis zu den Größten vorarbeitet

Bei den Widerständen ist zu beachten, dass sie möglichst genau mit den vorgegebenen Werten übereinstimmen. Somit gleichen die Pads einer Tonleiter und es kommen keine großen Sprünge zwischen Tönen vor. Da die meisten Widerstandswerte keine Normwerte sind, müssen mehrere Widerstände parallel bzw. in serie geschaltet (übereinander gelötet) werden.

Beim IC ist wichtig zu beachten, dass dieser richtig gepolt eingelötet wird. Der Pin 1 wird meist gekennzeichnet durch einen Punkt oder einen Strich.

### 2. Drähte vorbereiten

Zunächst werden 4 rote Drähte und 6 schwarze Drähte mit je einem Durchmesser von 0,2mm (gegebenenfalls auch 0,25mm) und einer Länge von 120mm abgeschnitten. Weiters werden ein roter und zwei schwarze Drähte mit einer Länge von 230mm abgelängt. Alle Drähte werden auf beiden Seiten 10mm abisoliert.

### 3. Lautsprecher

An den Lautsprecher wird je ein roter und ein schwarzer Draht mit einer Länge von 230mm angelötet. Es ist dabei egal, wie er gepolt wird, weil dies nur bewirkt, ob sich der Lautsprecher zusammenzieht oder ausdehnt (Wenn mehrere Lautsprecher verwendet werden, muss schon darauf geachtet werden, dass alle gleich gepolt sind. Dies ist aus dem Grund, da sich sonst die Schallwellen überlagern können und kein schöner Ton erzeugt wird.). Zum Anlöten der Drähte am Gehäuse des Lautsprechers wird eine Karosserielötpaste verwendet. Diese beinhaltet ein spezielles Flussmittel, das aggressiver ist und eine bessere Verbindung zum Metall (Eisen) schafft.

### 4. Potenziometer

Es werden ein Potenziometer mit dem Wert von und eines mit benötigt. Anschließend wird je ein schwarzer Draht auf jeden Anschluss des Potis gelötet.

### 5. Anlöten der vorbereiteten Bauteile

Nun werden alle Bauteile, die wir vorher vorbereitet haben (Lautsprecher und Potis), auf die Platine lt. BOM-Datei angelötet.

<u>Als Hinweis:</u>

- Lautsprecher: Der Lautsprecher wird auf der gegenüberliegenden Seite der Taster angelötet.
- Poti : Dies wird gleich neben dem Lautsprecher angelötet, dort wo drei Bohrungen nebeneinander liegen.
- Poti : Das zweite Poti wird bei den übrig gebliebenen drei Bohrungen angelötet.
- Batterieclip: Dieser wird gleich neben den Tastern angelötet, wobei der rote Draht unten ist (in Richtung der großen Kupferflächen).
- Draht des Stiftes: Der Stift wird erst nach dem Einbau der Platine ins Gehäuse angelötet, jedoch muss ein Ende des Drahtes schon angelötet werden. Dazu wird ein langer (23cm) Draht genommen und bei der einzelnen Bohrung bei der Diode angelötet.

### 6. Inbetriebnahme

Wenn alle Bauteile angelötet sind, kann die Platine in Betrieb genommen werden. Vorher muss aber unbedingt noch inspiziert werden, ob auch alle Bauteile richtig angelötet und Bauteile wie der IC richtig gepolt sind. Danach wird eine grobe Kurzschlussüberprüfung durchgeführt, bei dieser wird der Widerstand bei der Versorgung gemessen, ob dieser hoch- oder niederohmig ist. Anschließend wird die Schaltung mit einer vollgeladenen 9V Blockbatterie in Betrieb genommen.

### 7. Gehäuse bauen

Das Gehäuse wird grundsätzlich mit dem 3D-Drucker gedruckt. Da ein Loch für ein Potenziometer fehlt und das Vorhandene zu klein ist, müssen diese neu bzw. nachgebohrt werden.

<img src="bilder/Abbildung1.png" width="50%" text-align: center>

_Abbildung 1_


Der rote Pfeil (Abbildung 1) zeigt auf das Loch für das Potenziometer vorgesehen ist, jedoch muss noch mit einem 5,5mm Bohrer nachgebohrt werden. Von der Mitte dieser Bohrung aus werden 20mm nach rechts abgemessen und dort ebenfalls eine Bohrung von 5,5mm vorgenommen.

Zum Befestigen der Potenziometer werden diese mit Heißkleber von innen angeklebt. Die Kontakte dürfen dabei überklebt werden, jedoch muss darauf geachtet werden, dass der drehbare Teil des Potis nicht festgeklebt wird.

Damit der Stift während er nicht im Gebrauch ist verstaut wird, muss dieses Loch ebenfalls noch mit einem 5mm Bohrer nachgebohrt werden (Abbildung 2).

<img src="bilder/Abbildung2.png" width="50%" text-align: center>


_Abbildung 2_


Um später den Deckel anschrauben zu können, werden rechts und links hinten Muttern „eingeschmolzen“ in das Gehäuse. Dazu werden Einschmelzmuttern oder Einlötmuttern auf die Bohrungen gelegt und so lange mit der Lötspitze erhitzt, bis sie plant mit der Oberkante abschließt Abbildung 3).

<img src="bilder/Abbildung3.png" width="50%" text-align: center>

_Abbildung 3_

### 8. Platine einbauen

Um die Platine ins Gehäuse einzubauen, wird sie von hinten, mit den großen Kupferflächen nach vorne, in das Gehäuse horizontal hineingeschoben. Die 9V-Batterie wird angeschlossen und kann unter die Platine gelegt werden.

### 9. Stift des Stylophons

Hierzu wird ein 10cm lange Stück eines Kupferdrahtes mit einem Querschnitt von vorbereitet (Eine Spitze rund schleifen!). Anschließend werden auf beiden Seiten 15mm abisoliert und auf einem Ende mit viel Lötzinn und einer möglichst großen Lötspitze der vorgesehene Draht (mit einer Länge von 23cm) angelötet. Um die Lötstelle zu sichern, wird anschließend ein Schrumpfschlauch von ca. 4cm mit dem Heißluftföhn geschrumpft.

### 10. Knopf befestigen

Im Betrieb müssen beide Knöpfe gleichzeitig gedrückt werden, um einen Ton zu erzeugen. Dafür muss beim Festschrauben des Deckels vorher der gedruckte Knopf durch das Loch am Deckel gesteckt werden.

### Hinweise für den Betrieb

Es darf nur auf die großen Kupferflächen mit dem Stift gedrückt werden, da sonst die Transistoren oder der IC beschädigt werden können.