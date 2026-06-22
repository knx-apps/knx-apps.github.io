---
title: "Erste Schritte"
type: docs
weight: 1
bookCollapseSection: false
---
# Erste Schritte

## Zusammenfassung
Mit der Alertmanager App können Störmeldungen in einer Liste dargestellt werden. Die zuletzt ausgelöste Meldung, wird in der Liste ganz oben angezeigt. Ausgelöste Meldungen werden mit einem blinkenden {{< badge style="danger" value="roten" >}} Hintergrund dargestellt, über einen Button "Quittieren" kann die Störmeldung **quittiert** werden und der Hintergrund wird {{< badge style="warning" value="orange" >}} dargestellt. Eine quittierte Störmeldung, wird solange in der Liste angezeigt, bis diese behoben wurde und sich der Wert des KNX Datenpunktes ändert.  
Wenn eine ausgelöste Meldung von selbst wieder zurückgesetzt wird, so wird diese in der Liste mit einem {{< badge style="success" value="grünen" >}} Hintergrund dargestellt. Mit einem Klick auf den quittieren Button verschwindet die Meldung dann aus der Störmeldeliste.

Anbei ein Beispiel, wie eine fertige Störmeldeliste aussehen könnte.

{{< image src="list.gif" alt="Dashboard" title="List" >}}

## Verwendung der Alertmanager app

### 1. Klicken Sie auf die Alermanager App auf dem Startbildschirm des Wiser for KNX / spaceLYnk-Controllers. (![1](../1.png)).
{{< image src="start-alertmanager.png" alt="Start Dashboard" title="Start Alertmanager" >}}

Standardmäßig wird die Störmeldeliste mit der `ID = 1` aufgerufen, wenn auf das App Icon geklickt wird. Soll eine andere Störmeldeliste aufgerufen werden, so muss die URL mit dem Parameter `list` aufgerufen werden. `http://<ip>/apps/data/alertmanager/?list=2`

### 2. Grundkonfiguration
Für jede Störmeldeliste muss ein eigenes **zyklisches Skript** angelegt werden, mit einer **Standby Zeit** von **0 Sekunden**. Jede Störmeldeliste bekommt eine eigene ID `1`, sowie einen Tag `sm`. Alle Objekte, welchen dieser Tag zugeordnet ist, werden in der Störmeldeliste angezeigt.  
Alle Konfigurationsmöglichkeiten sind im Abschnitt [Konfiguration](/alertmanager/konfiguration/) zu finden.

```lua
require('applibs.alertmanager.functions')

list = 1
tag = 'sm'

delayedAlerts(list, tag)
```