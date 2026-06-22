---
title: "Charts"
type: docs
weight: 3
bookCollapseSection: false
---

# Charts

## Chart hinzufügen
1. Um ein Diagramm zu erstellen, gehen Sie zum Chart-Bereich und klicken Sie unten links auf die Schaltfläche "**Add Chart**" (![1](../1.png)).

{{< image src="add-chart.png" alt="Chart hinzufügen" title="Chart hinzufügen" >}}

2. Geben Sie im Dialogfeld einen Namen für das Diagramm ein, das Sie erstellen möchten (![1](../1.png)), und klicken Sie auf die Schaltfläche "**Add Chart**" (![2](../2.png)).

{{< image src="add-new-chart.png" alt="Chart hinzufügen" title="Chart hinzufügen" >}}

## Chart verwalten

{{< image src="chart-buttons.png" alt="Chart Buttons" title="Chart Buttons" >}}

### ![1](../1.png) bearbeiten
Klicken Sie hier, um das Chart zu bearbeiten. Weitere Informationen finden Sie im Abschnitt **Chart bearbeiten**.

### ![2](../2.png) duplizieren
Klicken Sie hier, um das Chart zu duplizieren. Dem Namen des duplizierten Charts wird "**(Kopie)**" hinzugefügt.

### ![3](../3.png) exportieren
Klicken Sie hier, um das Chart zu exportieren. Ihr Browser wird versuchen, eine Datei mit dem Inhalt des Charts herunterzuladen.

### ![4](../4.png) ansehen
Klicken Sie hier, um das Chart in Ihrem Browser anzuzeigen.

### ![5](../5.png) importieren
Klicken Sie hier, um ein zuvor exportiertes Chart erneut zu importieren. Dem Namen des importierten Charts wird "**(Import)**" hinzugefügt.

## Chart bearbeiten

### General
#### Chart Type
Hier können Sie den Diagrammtyp auswählen. Derzeit stehen vier verschiedene Diagrammtypen zur Verfügung:
* `Donut`
* `Torten`
* `Balken`
* `Balken horizontal`

Sie können jederzeit zwischen Donut- und Tortendiagrammen, sowie zwischen Balken- und horizontalen Balkendiagrammen wechseln, ohne dass Ihre bereits vorgenommenen Einstellungen verloren gehen.  
Wenn Sie von Donut/Torten zu Balken/horizontal wechseln, werden alle bereits zugewiesenen Datenpunkte gelöscht.

#### Aspect Ratio
Dadurch können Sie das Seitenverhältnis des Diagramms so anpassen, dass das Diagramm das Widget so effektiv wie möglich ausfüllt.

#### CSS Padding
Mit der CSS-Eigenschaft `padding` lässt sich das Diagramm besser in ein Widget einpassen, indem der Abstand zum Rand festgelegt wird. Es können zwischen 1 und 4 Werte angegeben werden.

#### Cutout (only Donut chart)
Nur für Donut-Diagramme verfügbar. Hiermit wird die Größe des Ausschnitts in der Mitte als Prozentsatz angegeben. Mögliche Werte liegen zwischen 0,1 und 99.

#### Backgroundcolor
Legt die Hintergrundfarbe des Diagramms fest.

#### Set Backgroundcolor transparent
Durch Auswahl dieser Option wird der Hintergrund des Diagramms vollständig transparent.

### Dataset
#### Donut / Pie Chart
Für die einzelnen Datenpunkte steht nur ein Datensatz zur Verfügung.

#### Bar / Bar horinzontal
Es stehen mehrere Datensätze mit jeweils mehreren Datenpunkten zur Verfügung. Wenn beispielsweise ein Vergleich zwischen zwei Zeiträumen (gestern und heute) angezeigt werden soll, wird für jeden Zeitraum ein separater Datensatz verwendet.

### Datapoint
#### Donut / Pie Chart
##### Datapoint
Der Wert des hier ausgewählten KNX-Datenpunkts wird zur Anzeige im Diagramm verwendet.

##### Legend
Beschriftung des Datenpunkts in der Legende und im Tooltip-Fenster.

##### Backgroundcolor
Farbe als Datenpunkt sollte im Diagramm angezeigt werden.

##### Border Width
Randbreite des Datenpunkts im Diagramm.

##### Bordercolor
Rahmenfarbe des Datenpunkt im Diagramm.

#### Bar / Bar horinzontal
##### Datapoint
Der Wert des hier ausgewählten KNX-Datenpunkts wird zur Anzeige im Diagramm verwendet.  
Wenn „Trendprotokoll“ als Datenpunkt ausgewählt ist, kann der Wert einer Trendaufzeichnung im Diagramm angezeigt werden.

##### Trend log (only available if Trend log is selected as the data point)
Gibt den Trenddatensatz an, aus dem der Wert angezeigt werden soll.  
Der Trend darf nur absolute Zählerwerte enthalten, d. h. Werte, die immer ansteigen, damit die Berechnung korrekt funktioniert.

##### Mode (only available if Trend log is selected as the data point)
Legt die Standardeinheit fest, die beim ersten Aufruf des Diagramms verwendet werden soll.

##### Show data from x days / weeks / months / years (only available if Trend log is selected as the data point)
Gibt die Anzahl der anzuzeigenden Werte in Abhängigkeit vom ausgewählten Modus an.

##### Offset (only available if Trend log is selected as the data point)
Dieser Wert wird zum aktuellen Datum addiert, um den Startwert anzupassen.  
Werte in der Vergangenheit können durch Eingabe negativer Werte angezeigt werden.

##### Value Multiplier (only available if Trend log is selected as the data point)
Das aus der Trendaufzeichnung gewonnene Ergebnis wird mit diesem Faktor multipliziert, um das Endergebnis anzupassen (z. B. Wh zu kWh).

##### Legend
Jeder Datenpunkt im ersten Datensatz verfügt über eine Legende, die unterhalb oder neben den einzelnen Balken angezeigt wird. Dieser Eintrag wird auch als Titel im Tooltip verwendet.  
Wenn eine KNX-Gruppenadresse als Text angegeben ist, wird der Wert dieser Gruppenadresse als Text angezeigt.

##### Label
Der erste Datenpunkt jedes Datensatzes wird in der Legende und im Tooltip verwendet, um die einzelnen Datensätze zu beschriften.

##### Backgroundcolor
Farbe wie der Datenpunkt im Diagramm angezeigt werden soll.

##### Border Width
Randbreite des Datenpunkts im Diagramm.

##### Bordercolor
Rahmenfarbe wie der Datenpunkt im Diagramm angezeigt wird.

### Coordinate system (only Bar chart)
#### Stacked axies
Dadurch werden die Datenpunkte der einzelnen Datensätze übereinander statt nebeneinander angezeigt.

#### Color X/Y Axis
Legt die Farbe des Koordinatensystems fest.

#### Color Scale Y-Axis
Legt die Farbe der Beschriftung der Y-Achse fest.

#### Fontweight
Legt die Schriftstärke der Beschriftung der Y-Achse fest.

#### Size
Legt die Schriftgröße der Beschriftung der Y-Achse fest.

#### Show Title Y-Axis
Wenn diese Option aktiviert ist, kann auf der Y-Achse eine Beschriftung angezeigt werden.

##### Text
Text, der als Beschriftung für die Y-Achse angezeigt werden soll.

##### Color
Textfarbe der Beschriftung der Y-Achse.

##### Fontweight
Schriftstärke der Beschriftung der Y-Achse.

##### Size
Schriftgröße der Beschriftung der Y-Achse.

#### Color Scale X-Axis
Legt die Farbe der Beschriftung der X-Achse fest.

#### Fontweight
Legt die Schriftstärke der Beschriftung der X-Achse fest.

#### Size
Legt die Schriftgröße der Beschriftung der X-Achse fest.

#### Show Title X-Axis
Wenn diese Option aktiviert ist, kann auf der X-Achse eine Beschriftung angezeigt werden.

##### Text
Text, der als Beschriftung für die X-Achse angezeigt werden soll.

##### Color
Textfarbe der Beschriftung der X-Achse.

##### Fontweight
Schriftstärke der Beschriftung der X-Achse.

##### Size
Schriftgröße der Beschriftung der X-Achse.

### Tooltip
#### Show
Wenn Sie diese Option aktivieren, wird beim Klicken auf ein Element des Diagramms ein Fenster mit dem aktuellen Wert angezeigt.

#### Display all data points of the data set
Alle Datenpunkte werden untereinander angezeigt.

#### Display legend value
Zusätzlich zum Wert wird zur besseren Zuordnung auch der Legendentext angezeigt.

#### Hide zero values
Wenn ein Wert 0 ist, wird der entsprechende Eintrag in der Legende ebenfalls nicht angezeigt.

#### Display sum of all data set values
Wenn alle Werte angezeigt werden, kann diese Option verwendet werden, um die Summe aller Einzelwerte zu berechnen und anzuzeigen.

#### Text before sum
Vor der berechneten Summe kann ein frei definierbarer Text angezeigt werden.

#### Title
##### Color
Textfarbe des Titels im Tooltip.

##### Fontweight
Schriftstärke des Titels im Tooltip.

##### Size
Schriftgröße des Titels im Tooltip.

#### Body
##### Color
Textfarbe des Body im Tooltip.

##### Fontweight
Schriftstärke des Body im Tooltip.

##### Size
Schriftgröße des Body im Tooltip.

#### Footer
##### Color
Textfarbe der Fußzeile im Tooltip.

##### Fontweight
Schriftstärke der Fußzeile im Tooltip.

##### Size
Schriftgröße der Fußzeile im Tooltip.

### Title
#### Show
Mit dieser Option kann ein Titel über dem Diagramm angezeigt werden.

#### Text
Der Text, der als Titel über dem Diagramm angezeigt werden soll.

#### Color
Die Schriftfarbe des Titels, der über dem Diagramm angezeigt wird.

#### Fontweight
Die Schriftstärke des Titels, der über dem Diagramm angezeigt wird.

#### Size
Die Schriftgröße des Titels, der über dem Diagramm angezeigt wird.

#### Padding Top
Legt den Abstand zwischen dem Titel und dem oberen Rand des Diagramms fest.

#### Padding Bottom
Legt den Abstand unterhalb des Titels bis zum Beginn des Diagramms fest.

### Legend
#### Show
Mit dieser Option kann eine Legende der einzelnen Diagrammelemente angezeigt werden.

#### Position
Gibt an, auf welcher Seite des Diagramms die Legende positioniert werden soll.

#### Color
Schriftfarbe der Legende.

#### Fontweight
Schriftstärke der Legende.

#### Size
Schriftgröße der Legende.

### Datalabels
#### Show
Diese Option zeigt den Wert eines Diagrammelements direkt im Element selbst an.

#### Textcolor
Schriftfarbe der Beschriftung im Diagrammelement.

#### Fontsize
Schriftgröße der Beschriftung im Diagrammelement.

#### Fontweight
Schriftstärke der Beschriftung im Diagrammelement.

#### Unit
Die Werteeinheit besteht aus einem frei definierten Text, der hinter dem aktuellen Wert angezeigt wird. Diese Einheit wird auch im Tooltip verwendet.

#### Decimal Places
Gibt an, mit wie vielen Dezimalstellen der Wert angezeigt werden soll. Wird auch im Tooltip verwendet.

#### Remove values smaller than
Wenn der Wert kleiner als der hier definierte Wert ist, wird die Beschriftung nicht angezeigt. Das bedeutet, dass bei kleinen Werten, bei denen das Diagrammelement sehr schmal ist, die Werte der Beschriftung entsprechend ausgeblendet werden können.

### Date selection Trend log (only Bar chart)
#### Show
Wenn diese Option aktiviert ist, wird im Diagramm ein Button angezeigt, mit der der angezeigte Zeitbereich manuell angepasst werden kann.

#### Position
Gibt die Position des Buttons an, mit dem die manuelle Zeitauswahlen vorgenommen werden kann.

#### Offset top / bottom
Gibt den Abstand vom Rand des Diagramms an. Je nach ausgewählter Position kann dies vom oberen oder unteren Rand sein.

#### Offset right / left
Gibt den Abstand vom Rand des Diagramms an. Je nach ausgewählter Position kann dies vom rechten oder linken Rand sein.
\
\
\
Sobald alle Parameter konfiguriert sind, kann das Diagramm durch Klicken auf den Button "**Save Chart**" gespeichert werden.

## Chart löschen
Wechseln Sie in den Bearbeitungsmodus, klicken Sie auf den **roten Löschen Button** und bestätigen Sie mit **Ja**.

{{< image src="delete-chart.png" alt="Chart löschen" title="Chart löschen" >}}