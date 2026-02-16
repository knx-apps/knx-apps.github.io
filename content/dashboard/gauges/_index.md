---
title: "Gauges"
type: docs
weight: 4
bookCollapseSection: false
---

# Gauges

## Gauge hinzufügen

1. Um ein Gauge zu erstellen, gehen Sie zum Gauge-Bereich und klicken Sie unten links auf die Schaltfläche "**Add Gauge**" (![1](../1.png)).

{{< image src="add-gauge.png" alt="Gauge hinzufügen" title="Gauge hinzufügen" >}}

2. Geben Sie im Dialogfeld einen Namen für das Gauge ein, das Sie erstellen möchten (![1](../1.png)), und klicken Sie auf die Schaltfläche "**Add Gauge**" (![2](../2.png)).

{{< image src="add-new-gauge.png" alt="Gauge hinzufügen" title="Gauge hinzufügen" >}}

## Gauge verwalten

{{< image src="gauge-buttons.png" alt="Gauge Buttons" title="Gauge Buttons" >}}

### ![1](../1.png) bearbeiten
Klicken Sie hier, um das Gauge zu bearbeiten. Weitere Informationen finden Sie im Abschnitt **Gauge bearbeiten**.

### ![2](../2.png) duplizieren
Klicken Sie hier, um das Gauge zu duplizieren. Dem Namen des duplizierten Gauges wird "**(Kopie)**" hinzugefügt.

### ![3](../3.png) exportieren
Klicken Sie hier, um das Gauge zu exportieren. Ihr Browser wird versuchen, eine Datei mit dem Inhalt des Gauges herunterzuladen.

### ![4](../4.png) ansehen
Klicken Sie hier, um das Gauge in Ihrem Browser anzuzeigen.

### ![5](../5.png) importieren
Klicken Sie hier, um ein zuvor exportiertes Gauge erneut zu importieren. Dem Namen des importierten Gauges wird "**(Import)**" hinzugefügt.

## Gauge bearbeiten

### General
#### Gauge Type
Sie können zwischen zwei Gauge Typen wählen:  
`normal`: Das Gauge beginnt beim Mindestwert.  
`differential`: Das Gauge füllt sich von der Mitte aus.

#### Min
Gibt den Mindestwert an.

#### Max
Gibt den Maximalwert an.

#### Decimals
Anzahl der Stellen nach dem Komma.

#### CSS Padding
Mit der CSS-Eigenschaft `padding` lässt sich die Anzeige besser in ein Widget einpassen, indem der Abstand zum Rand festgelegt wird. Es können zwischen 1 und 4 Werte angegeben werden.

#### Gauge Width Scale
Skalierungsfaktor der Breite des Gauge.

#### Single Color
Das Gauge ist mit einer Farbe gefüllt, um den aktuellen Wert anzuzeigen.

#### Multiple Colors
Das Gauge ändert entweder je nach aktuellem Wert seine Farbe, oder es werden feste Farbbereiche angezeigt, und der aktuelle Wert kann mit Hilfe des Zeigers abgelesen werden.

##### Default Color
Die Standardfarbe wird für alle nicht definierten Wertebereiche angezeigt.

##### Show Sector Colors
Wenn diese Option aktiviert ist, ändert das Gauge seine Farbe nicht in Abhängigkeit vom aktuellen Wert, sondern die definierten Farbbereiche werden als Sektoren auf dem Gauge angezeigt.

##### Values as percentages
Wenn diese Option aktiviert ist, werden die definierten Farbbereiche als Prozentwerte statt als absolute Werte angegeben.

##### From
Gibt den Anfangswert eines zu definierenden Farbbereichs an.

##### To
Gibt den Endwert eines zu definierenden Farbbereichs an.

##### Color
Legt die Farbe des definierten Farbbereichs fest.

#### Backgroundcolor
Legt die Hintergrundfarbe des Gauge fest.

#### Set Backgroundcolor transparent
Durch Auswahl dieser Option wird der Hintergrund des Gauge vollständig transparent.

### Title
#### Text
Der Text, der als Titel über dem Gauge angezeigt werden soll.

#### Color
Die Schriftfarbe des Titels, der über dem Gauge angezeigt wird.

#### Fontweight
Die Schriftstärke des Titels, der über dem Gauge angezeigt wird.

#### Size
Die Schriftgröße des Titels, der über dem Gauge angezeigt wird.

### Value
#### Address
Gibt das Objekt an, das den anzuzeigenden Wert enthält.

#### Color
Schriftfarbe, in der der aktuelle Wert angezeigt werden soll.

#### Size
Schriftgröße, in der der aktuelle Wert angezeigt werden soll.

#### Unit
Die Werteeinheit besteht aus einem frei definierbaren Text, der hinter dem aktuellen Wert angezeigt wird.

### Label
#### Text
Text der Beschriftung, die unter dem aktuellen Wert angezeigt wird.

#### Color
Schriftfarbe der Beschriftung, die unter dem aktuellen Wert angezeigt wird.

#### Size
Schriftgröße der Beschriftung, die unter dem aktuellen Wert angezeigt wird.

### Pointer
#### Show
Wenn diese Option aktiviert ist, wird ein Wertzeiger angezeigt.

#### Color
Farbe des Wertzeigers.

#### Top Length
Oberer Überhang des Wertzeigers.

#### Bottom Length
Bottom overhang of the value pointer.

#### Bottom Width
Unterer Überhang des Wertzeigers.

### Target Line
#### Show
Zeigt eine Ziellinie an.

#### Color
Farbe der Ziellinie.

#### Value
Wert, bei dem die Ziellinie angezeigt wird.

#### Width
Breite der Ziellinie.
\
\
\
Sobald alle Parameter konfiguriert sind, kann das Gauge durch Klicken auf die Schaltfläche "**Save Gauge**" gespeichert werden.

## Gauge löschen
Wechseln Sie in den Bearbeitungsmodus, klicken Sie auf den **roten Löschen Button** und bestätigen Sie mit **Ja**.

{{< image src="delete-gauge.png" alt="Gauge löschen" title="Gauge löschen" >}}