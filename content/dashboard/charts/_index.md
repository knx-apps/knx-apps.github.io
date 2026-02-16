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
Here you can select the type of chart. There are currently four different chart types: Donut, Pie, Bar, Horizontal bar

You can switch between donut and pie charts, as well as between bar and horizontal bar charts, at any time without losing the settings you have already made.
If you switch from Donut/Pie to Bar/Bar Horizontal, all data points that have already been assigned will be deleted.

#### Aspect Ratio
This allows you to adjust the aspect ratio of the chart so that the widget fills the dashboard as effectively as possible.

#### CSS Padding
The CSS padding property allows the chart to be better fitted into a widget, specifying the distance to the edge. Between 1 and 4 values can be specified.

#### Cutout (only Donut chart)
Only available for donut charts, this specifies the size of the section in the middle as a percentage. Values between 0.1 and 99 are possible.

#### Backgroundcolor
Specifies the background color of the chart.

#### Set Backgroundcolor transparent
Selecting this option makes the background of the chart completely transparent.

### Dataset
#### Donut / Pie Chart
Only one data set is available for the individual data points.

#### Bar / Bar horinzontal
Several data sets are available, each with multiple data points.
If, for example, a comparison between two time periods (yesterday and today) is to be displayed, a separate data set is used for each time period.

### Datapoint
#### Donut / Pie Chart
##### Datapoint
The value of the KNX data point selected here is used to display it in the diagram.

##### Legend
Labeling of the data point in the legend and the tooltip window.

##### Backgroundcolor
Color as the data point should be displayed in the chart.

##### Border Width
Border width of the data point in the diagram.

##### Bordercolor
Border Color how the data point is displayed in the chart.

#### Bar / Bar horinzontal
##### Datapoint
The value of the KNX data point selected here is used to display it in the diagram.
If "Trend log" is selected as the data point, the value of a trend recording can be displayed in the diagram.

##### Trend log (only available if Trend log is selected as the data point)
Specifies the trend record from which the value is to be displayed.
The trend may only contain absolute counter values, i.e. values that always increase, in order for the calculation to work correctly.

##### Mode (only available if Trend log is selected as the data point)
Specifies the default unit to be used when the chart is first called up.

##### Show data from x days / weeks / months / years (only available if Trend log is selected as the data point)
Specifies the number of values to be displayed depending on the selected mode.

##### Offset (only available if Trend log is selected as the data point)
This value is added to the current date to adjust the start value.
Values in the past can be displayed by entering negative values.

##### Value Multiplier (only available if Trend log is selected as the data point)
The result retrieved from the trend recording is multiplied by this factor in order to adjust the final result (e.g. Wh to kWh).

##### Legend
Each data point in the first data set has a legend, which is displayed below or next to the individual bars. This entry is also used as the title in the tooltip.
If a KNX group address is specified as text, the value of this group address is displayed as text.

##### Label
The first data point of each data set is used in the legend and tooltip to label the individual data sets.

##### Backgroundcolor
Color as the data point should be displayed in the chart.

##### Border Width
Border width of the data point in the diagram.

##### Bordercolor
Border Color how the data point is displayed in the chart.

### Coordinate system (only Bar chart)
#### Stacked axies
This displays the data points of the individual datasets on top of each other instead of side by side.

#### Color X/Y Axis
Specifies the color of the coordinate system.

#### Color Scale Y-Axis
Specifies the color of the Y-axis label.

#### Fontweight
Specifies the font weight of the Y-axis.

#### Size
Specifies the font size of the Y-axis.

#### Show Title Y-Axis
If this option is set, a label can be displayed on the Y-axis.

##### Text
Text to be displayed as the label for the Y-axis.

##### Color
Text color of the Y-axis label.

##### Fontweight
Fontweight of the Y-axis labeling.

##### Size
Font size of the Y-axis label.

#### Color Scale X-Axis
Specifies the color of the X-axis label.

#### Fontweight
Specifies the font weight of the X-axis.

#### Size
Specifies the font size of the X-axis.

#### Show Title X-Axis
If this option is set, a label can be displayed on the X-axis.

##### Text
Text to be displayed as the label for the X-axis.

##### Color
Text color of the X-axis label.

##### Fontweight
Fontweight of the X-axis labeling.

##### Size
Font size of the X-axis label.

### Tooltip
#### Show
By setting this option, a window with the current value is displayed when you click on an element of the diagram.

#### Display all data points of the data set
All data points are displayed one below the other.

#### Display legend value
In addition to the value, the label text is also displayed for better classification.

#### Hide zero values
If a value is 0, the corresponding entry in the legend is also not displayed.

#### Display sum of all data set values
If all values are displayed, this option can also be used to calculate and display the sum of all individual values.

#### Text before sum
A freely definable text can be displayed before the calculated total.

#### Title
##### Color
Text colour of the title in the tooltip.

##### Fontweight
Font weight of the title in the tooltip.

##### Size
Font size of the title in the tooltip.

#### Body
##### Color
Text colour of the body in the tooltip.

##### Fontweight
Font weight of the body in the tooltip.

##### Size
Font size of the body in the tooltip.

#### Footer
##### Color
Text colour of the footer in the tooltip.

##### Fontweight
Font weight of the footer in the tooltip.

##### Size
Font size of the footer in the tooltip.

### Title
#### Show
This option allows a title to be displayed above the chart.

#### Text
The text to be displayed as the title above the diagram.

#### Color
The font colour of the title displayed above the diagram.

#### Fontweight
The font weight of the title displayed above the diagram.

#### Size
The font size of the title displayed above the diagram.

#### Padding Top
Defines the distance above the title to the top edge of the chart.

#### Padding Bottom
Defines the distance below the title to the start of the chart.

### Legend
#### Show
This option allows a legend of the individual diagram elements to be displayed.

#### Position
Specifies on which side of the diagram the legend should be positioned.

#### Color
Font colour of the legend.

#### Fontweight
Font weight of the legend.

#### Size
Font weight of the legend.

### Datalabels
#### Show
This option displays the value of a chart element directly in the element itself.

#### Textcolor
Font colour of the data label text.

#### Fontsize
Font colour of the data label text.

#### Fontweight
Font weight of the data label text.

#### Unit
The value unit consists of a freely defined text that is displayed after the actual value. This unit is also used in the tooltip.

#### Decimal Places
Specifies how many decimal places the value should be displayed with. Also used in the tooltip.

#### Remove values smaller than
If the value is smaller than the value defined here, the data label is not displayed. This means that for small values, where the chart element is very narrow, the data label values can be hidden accordingly.

### Date selection Trend log (only Bar chart)
#### Show
If this option is set, a button is displayed in the chart that can be used to manually adjust the displayed time range.

#### Position
Specifies the position of the button used to make manual time selections.

#### Offset top / bottom
Specifies a distance from the edge of the chart. Depending on the selected position, this can be from the top or bottom edge.

#### Offset right / left
Specifies a distance from the edge of the chart. Depending on the selected position, this can be from the right or left edge.
\
\
\
Sobald alle Parameter konfiguriert sind, kann das Diagramm durch Klicken auf die Schaltfläche "**Save Chart**" gespeichert werden.

## Chart löschen
Wechseln Sie in den Bearbeitungsmodus, klicken Sie auf den **roten Löschen Button** und bestätigen Sie mit **Ja**.

{{< image src="delete-chart.png" alt="Chart löschen" title="Chart löschen" >}}