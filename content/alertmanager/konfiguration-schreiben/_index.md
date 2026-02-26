---
title: "Konfiguration überschreiben"
type: docs
weight: 4
bookCollapseSection: false
---
# Konfiguration überschreiben
Die Konfiguration jeder Störmeldeliste kann mit der Funktion `setConfig()` geändert werden.  
Die Funktion muss nur **einmalig** aufgerufen werden.

## setConfig(list, config)
* `list`: Nummer der Störmeldeliste
* `config`: Lua Tabelle, welche alle Konfigurationsparamter enthält

## Konfigurationsparameter "config" Tabelle
### defaulttriggervalue
Gibt den Standardwert an, bei welchem die Störmeldung als **ausgelöst** angezeigt werden soll. `true` oder `false`. Der Standardwert ist: `true`.

### translation
Hier kann eine Übersetzung der Beschriftung innerhalb der App angegeben werden.  
Folgende Einträge stehen zur Verfügung:

#### headercolumn1
Beschriftung der ersten Spalte, in welcher das Datum und die Uhrzeit zu der die Störmeldung ausgelöst wurde angezeigt wird.

#### headercolumn2
Beschriftung der zweiten Spalte, in welcher die eigentliche Störmeldung angezeigt wird.

#### ackbutton
Beschriftung des quttieren Buttons.

#### title
Beschriftung des Titel des Browserfensters.

#### noalerts
Wenn keine Störmeldungen vorhanden sind, wird diese Meldung angezeigt.

## Beispiel
Das Nachfolgende Beispiel setzt den Standard Trigger-Wert auf `false`, somit werden alle Meldungen, welche einen Werte Wechsel, von `true` nach `false` haben, als **ausgelöst** angezeigt.
```lua
require('applibs.alertmanager.functions')

list = 1
config = {
  ["defaulttriggervalue"] = false,
  ["translation"] = {
                        ["headercolumn1"] = "Zeit",
                        ["headercolumn2"] = "Meldung",
                        ["ackbutton"]     = "Quittieren",
                        ["title"]         = "Störmeldungen",
                        ["noalerts"]      = "Keine Störmeldungen vorhanden",
  }
}

setConfig(list, config)
```