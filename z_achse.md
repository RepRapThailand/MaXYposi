![GitHub Logo](http://www.heise.de/make/icons/make_logo.png)

Maker Media GmbH und c't, Heise Zeitschriften Verlag

***

# MaXYposi

### Plan und Stückliste Z-Achse

Für die Ausführung der Z-Achse gibt es mehrere Alternativen: Die einfachste, aber auch teuerste ist eine komplett mit Motor fertig aufgebaute Igus-Linearführung, die man sich [online konfigurieren kann](http://www.igus.de/wpck/7357/DryLin_E_Overview).

Preiswerter wird es, wenn man einen eigenen (billigen) Schrittmotor verwendet und ihn selbst an die manuelle Igus-Linearführung SLW-1040 anpasst. Diese bestellt man sich je nach Bedarf mit 50 bis 100 mm Hub. 

Der Motor-Adapter besteht aus einem 74 mm langen Alu-Rechteckprofil 40 x 60 mm, das nach Plan "igus-portal_Z-Achse_Maße.pdf" gebohrt wird. Im Prinzip wäre auch ein 40x40-Profil geeignet, dann wird es für die Befestigungsschrauben des Motors aber schon etwas eng.

- 1 Linearschlitten SLW-1040, komplett mit Endplatten und Gewindespindel TR10x2
- 1 Aluminium-Rechteckprofil 40x40 bis 40x60 mm, 74 mm lang, Wandstärke 2 mm
- 1 Wellenkupplung flexibel, 5mm/10mm (ebay/Amazon)
- 1 Wellenhalter SH20 (für Befestigung von Proxon-Motoren)
- 1 Schrittmotor NEMA 17 mit 5-mm-Welle, 1,25A bis 2,5A Strangstrom (d.h. gleiche Ausführung wie X/Y-Achse)

![Picture](https://github.com/heise/MaXYposi/blob/master/z_01.JPG)

Ein Alu-Rechteckprofil 40 x 40 mm (Bild) oder 40 x 60 mm wird auf 74 mm abgelängt und nach Plan "igus-portal_Z-Achse_Maße.pdf" gebohrt. Die Bohrung für die Motorwelle sollte mittig sitzen.

![Picture](https://github.com/heise/MaXYposi/blob/master/z_02.JPG)

Damit der Motor bündig passt, muss das mittlere Loch mit einem Stufenbohrer auf 22 mm aufgeweitet werden. Der Motor wird mit vier M3-Innensechskantschrauben (M3 x 8) befestigt. Wer keinen so großen Stufenbohrer besitzt, kann auch ein paar Unterlegscheiben als Abstandshalter zwischen Motor und Alu-Profil einfügen.

![Picture](https://github.com/heise/MaXYposi/blob/master/z_04.JPG)

Es erleichtert die Montage, wenn man die Befestigungslöcher auf beiden Seiten 
bohrt; dann kann man mit einem Sechskantschlüssel die innenliegenden Schrauben 
erreichen. Hier haben wir die Wellenkupplung 5/10 mm bereits auf die Motorwelle 
aufgesetzt.

![Picture](https://github.com/heise/MaXYposi/blob/master/z_06.JPG)

Die Igus-Adapterplatte wird mit zwei M5-Schrauben am Motorträger befestigt. Das 
ist einfacher, als zwei kurze M6-Schrauben für die vorhandenen Gewinde 
hineinzufummeln - der Bauraum im 40er-Profil ist ja begrenzt. 

Die fertige Z-Achse wird mit einem stabilen Alu-Winkel am MaXYposi-X-Schlitten 
befestigt. Es is empfehlenswert, die Konstruktion am oberen Ende noch mit einer 
Querstrebe abzustützen.

Abschließend muss man noch die Anzahl der Schritte pro Millimeter in den GRBL-
Defaults eintragen. Die TR10-Spindel der SLW-1040-Linearführung hat eine Steigung von 2 mm, bei Viertelschritt-Betrieb der Schrittmotor-Endstufe ist also (4*200)/2 = 400 für den Parameter $102 einzutragen.

### Z-Achse aus China

![Picture](https://github.com/heise/MaXYposi/blob/master/z_china_k.JPG)

Die deutlich bequemere und billigere Variante ist eine kleine Z-Achse aus 
chinesischer Fertigung, die wir vor kurzem entdeckten und die jetzt von 
verschiedenen Händlern auf ebay angeboten wird (Bild). Ein passender 
Schrittmotor ist bereits montiert. Einschließlich Versand kostet sie um 50 Euro. 
Hierfür benötigen Sie nur stabile Befestigungswinkel und zur Aufnahme des 
Spindelmotors einen Halter für 20-mm-Stahlwellen (diverse CNC-Shops).

Die Konstruktion erscheint uns ausreichend stabil, das Chassis besteht aus 3 mm starkem Edelstahl. Auf kleine Ungenauigkeiten hinsichtlich der Maßhaltigkeit und Rechtwinkligkeit muss man hierbei hinwegsehen.


