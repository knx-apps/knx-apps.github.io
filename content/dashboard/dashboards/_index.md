---
title: "Dashboards"
type: docs
weight: 2
bookCollapseSection: false
---

# Dashboards

## Dashboard hinzufügen
1. Um ein Dashboard zu erstellen, gehen Sie zum Dashboard-Bereich und klicken Sie unten links auf die Schaltfläche „Dashboard hinzufügen“ (![1](../1.png)).

{{< image src="add-dashboard.png" alt="Dashboard hinzufügen" title="Dashboard hinzufügen" >}}

2. Geben Sie im Dialogfeld einen Namen für das Dashboard ein, das Sie erstellen möchten (![1](../1.png)), und klicken Sie auf die Schaltfläche **Dashboard hinzufügen** (![2](../2.png)).

{{< image src="add-new-dashboard.png" alt="Dashboard hinzufügen" title="Dashboard hinzufügen" >}}

## Dashboard verwalten

{{< image src="dashboard-buttons.png" alt="Dashboard Buttons" title="Dashboard Buttons" >}}

### ![1](../1.png) bearbeiten
Klicken Sie hier, um das Dashboard zu bearbeiten. Weitere Informationen finden Sie im Abschnitt **Dashboard bearbeiten**.

### ![2](../2.png) duplizieren
Klicken Sie hier, um das Dashboard zu duplizieren. Dem Namen des duplizierten Dashboards wird "**(Kopie)**" hinzugefügt.

### ![3](../3.png) exportieren
Klicken Sie hier, um das Dashboard zu exportieren. Ihr Browser wird versuchen, eine Datei mit dem Inhalt des Dashboards herunterzuladen.

### ![4](../4.png) ansehen
Klicken Sie hier, um das Dashboard in Ihrem Browser anzuzeigen.

### ![5](../5.png) importieren
Klicken Sie hier, um ein zuvor exportiertes Dashboard erneut zu importieren. Dem Namen des importierten Dashboards wird "**(Import)**" hinzugefügt.

## Dashboard bearbeiten
Hier können Sie alle Einstellungen für ein Dashboard sowie die Anordnung und Größe der einzelnen Widgets konfigurieren.

{{< image src="dashboard-description.png" alt="Beschreibung Dashboard" title="Beschreibung Dashboard" >}}

### ![1](../1.png) Widgets bearbeiten
Klicken Sie hier, um die Dashboard-Widgets zu bearbeiten.

### ![2](../2.png) Name des Dashboards
Hier können Sie den Namen des Dashboards anzeigen und ändern.

### ![3](../3.png) Parameter des Dashboards
Alle Parameter des Dashboards werden hier angezeigt. Standardmäßig werden nur einige grundlegende Parameter angezeigt. Die vollständigen Parameter sind erst verfügbar, wenn die Dashboard-Widgets erstellt wurden.

### ![4](../4.png) Dashboard speichern
Klicken Sie hier, um alle Dashboard-Einstellungen zu speichern.

#### Widgets bearbeiten
Zunächst müssen Sie dem Dashboard neue Widgets hinzufügen. Ziehen Sie dazu das grüne Widget von der linken Seite in den hellgrauen Bereich auf der rechten Seite des Bildschirms.

{{< image src="add-widget.png" alt="Widget hinzufügen" title="Widget hinzufügen" >}}

Jedes Widget kann per Drag & Drop verschoben und so positioniert werden, dass es optimal zum Layout des Dashboards passt. Die Größe des Widgets kann ebenfalls angepasst werden, indem Sie die rechte untere Ecke des Widgets ziehen.

{{< image src="resize-widget.png" alt="Widget größe ändern" title="Widget größe ändern" >}}

Um ein Widget zu löschen, ziehen Sie es per Drag & Drop auf das rote Lösch-Widget auf der linken Seite des Bildschirms.

{{< image src="delete-widget.png" alt="Widget löschen" title="Widget löschen" >}}

Sobald alle Widgets hinzugefügt und positioniert wurden, können sie durch Klicken auf die Schaltfläche "**Widgets speichern**" gespeichert werden.

{{< image src="save-widgets.png" alt="Widget speichern" title="Widget speichern" >}}

#### Dashboard Parameter
Sobald die Widgets erstellt wurden, stehen zusätzliche Parameter zur Verfügung.

{{< image src="dashboard-parameters.png" alt="Dashboard Parameter" title="Dashboard Parameter" >}}

##### ![1](../1.png) Grundlegende Parameter

###### **Title section**
Hier kann HTML-Code eingegeben werden, der oberhalb des Dashboards als Titel angezeigt wird.  
`<h1 style="font-weight: bold; padding-left: 10px; margin: 0px; margin-top: 50px; color: #000000">Energy Dashboard</h1>`

###### **Responsive**
Ohne responsives Design werden das Dashboard oder einzelne Widgets einfach "zusammengeschoben", wenn der Bildschirm kleiner als das Dashboard ist. Wenn der responsive Parameter aktiviert ist, werden die Widgets untereinander angeordnet, anstatt zusammengeschoben zu werden.

{{< image src="responsive.png" alt="Responsive" title="Responsive" >}}

###### **Column width**
Legt die minimale Spaltenbreite und damit auch die minimale Breite eines Widgets fest.

###### **Max column**
Hier kann die maximale Anzahl der Spalten im Dashboard reduziert werden (mögliche Werte sind 1 bis 12). Ein Dashboard kann aus maximal 12 Spalten bestehen.  

In unserem Beispiel-Dashboard haben wir ein großes Widget mit einer Spaltenbreite von 6 und mehrere kleinere Widgets mit einer Spaltenbreite von jeweils 3.  

Das bedeutet, dass theoretisch eine Zeile das „große Widget” mit einer Spaltenbreite von 6 und zwei „kleine Widgets” mit einer Spaltenbreite von 3 aufnehmen könnte (6 + 3 + 3 = 12).  

Dies würde jedoch bedeuten, dass das Dashboard auf großen Bildschirmen wie folgt angezeigt würde.

{{< image src="responsive-12-cols.png" alt="Responsive 12 Spalten" title="Responsive 12 Spalten" >}}

Wenn der Wert für "**Max column**" in unserem Beispiel nun von 12 auf 11 reduziert wurde, können entweder das Widget mit einer Spaltenbreite von 6 und ein Widget mit einer Spaltenbreite von 3 in einer Zeile angezeigt werden, oder drei Widgets mit einer Spaltenbreite von 3, da jedes weitere Widget die maximale Anzahl von 11 überschreiten würde. Bei einer Einstellung von "**Max column**" auf 11 wird das Dashboard also wie folgt angezeigt.

{{< image src="dashboard.png" alt="Dashboard" title="Dashboard" >}}

###### **Appearance**

Wenn "**Default settings**" ausgewählt ist, werden die globalen Designeinstellungen von der Seite "**Settings**" angewendet. Wenn "**Custom settings**" ausgewählt ist, wird das Erscheinungsbild dieses Dashboards überschrieben. Eine detaillierte Beschreibung der einzelnen Parameter finden Sie in der Beschreibung der globalen Parameter auf der Seite [Settings](/dashboard/settings/).

##### ![2](../2.png) Widget Übersicht
Zeigt die aktuelle Widget-Struktur des Dashboards an. Jedem Widget wird eine eindeutige **Widget-ID** zugewiesen. Die **Widget-ID** kann im nächsten Schritt verwendet werden, um den Inhalt festzulegen, der im Widget angezeigt werden soll.

##### ![3](../3.png) Inhalt Zuweisung einzelner Widgets
Für jedes Widget können Sie wählen, ob Sie ein [**Chart**](/dashboard/charts/), [**Gauge**](/dashboard/gauges/), [**Energyflow**](/dashboard/energyflows/) oder eine **URL** als Inhalt anzeigen möchten. Wenn im ersten Auswahlfeld Chart, Gauge oder Energyflow ausgewählt ist, kann das entsprechende Element im zweiten Auswahlfeld ausgewählt werden.

{{< image src="select-content.png" alt="Inhalt auswählen" title="Inhalt auswählen" >}}

Wenn **URL** als Inhaltstyp ausgewählt ist, wird anstelle eines zweiten Auswahlfeldes die folgende Oberfläche angezeigt. In das Textfeld (![1](../1.png)) kann eine beliebige URL eingegeben werden, um den Inhalt einer anderen Seite, z. B. eine Visualisierungsseite von Wiser for KNX, im Dashboard anzuzeigen. Sie können weitere URLs hinzufügen, indem Sie auf den grünen + Button (![2](../2.png)) klicken. Wenn Sie die Option "**Show navigation button**" (![3](../3.png)) aktivieren, werden im Dashboard zwei Schaltflächen mit Pfeilen nach links und rechts angezeigt, mit denen Sie durch die verschiedenen Seiten navigieren können. Sie können eine URL löschen, indem Sie auf den Papierkorb Button (![4](../4.png)) klicken.

{{< image src="select-content-url.png" alt="Inhalt URL auswählen" title="Inhalt URL auswählen" >}}

Sobald alle Parameter konfiguriert sind, kann das Dashboard durch Klicken auf die Schaltfläche "**Dashboard speichern**" gespeichert werden.

## Dashboard löschen
Wechseln Sie in den Bearbeitungsmodus, klicken Sie auf den **roten Löschen Button** und bestätigen Sie mit **Ja**.

{{< image src="delete-dashboard.png" alt="Dashboard löschen" title="Dashboard löschen" >}}