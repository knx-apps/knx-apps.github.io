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

## Beispiel
Das Nachfolgende Beispiel setzt den Standard Trigger-Wert auf `false`, somit werden alle Meldungen, welche einen Werte Wechsel, von `true` nach `false` haben, als **ausgelöst** angezeigt.
```lua
require('applibs.alertmanager.functions')

list = 1
config = {
  ["defaulttriggervalue"] = false
}

setConfig(list, config)
```