---
title: "Konfiguration"
type: docs
weight: 2
bookCollapseSection: false
---
# Konfiguration

Für jede Störmeldeliste muss ein eigenes **zyklisches Skript** angelegt werden, mit einer **Standby Zeit** von **0 Sekunden**. Mit der `delayedAlerts` Funktion können Störmeldungen in einem zyklischen Skript ausggelöst werden:

## delayedAlerts(list, tag [, settings [, callback]])
Erzeugt eine neue Störmeldeliste mit der Nummer `list`. Alle Objekte, welchen der Tag `tag` zugeordnet ist, werden in der Störmeldeliste angezeigt. Aktuell werden nur boolsche Datenpunkte unterstützt bzw. alle Werte, werden in einen Boolean konvertiert. Standardmäßig gilt eine Störmeldung als "**ausgelöst**", wenn diese den Wert `true` besitzt. Der Auslösewert / Trigger-Wert kann entweder [global](/alertmanager/konfiguration-schreiben/), für die gesamte Störmeldeliste geändert werden, oder über die `settings` Tabelle für jeden einzelnen Datenpunkt.  

### List
Listennummer, mit welcher auf die Störmeldeliste zugegriffen werden kann.

### Tag
Alle Objekte, welchen der Tag zugeordnet ist, werden in der Störmeldeliste angezeigt.

### Settings
Lua Tabelle, mit welcher das Verhalten jeden einzelnen Datenpunktes angepasst werden kann.  
Der Schlüssel jeden einzelnen Tabelleneintrags gibt die Adresse des Objektes an (z.B. **1/1/1**).  
Als Wert wird jeweils eine Lua Tabelle mit folgenden Werten erwartet. **Jeder Wert ist optional.**
* `delayoff`  
Zeit in Sekunden, wie lange das Objekt dem Trigger-Wert entsprechen muss, bis die Störmeldung ausgelöst wird.
* `delayon`  
Zeit in Sekunden, wie lange das Objekt nicht dem Trigger-Wert entsprechen muss, bis die Störmeldung zurückgesetzt wird.
* `message`  
Text, welcher als Störmeldetext angezeigt wird, wird der Wert `message` nicht angegeben, wird standardmäßig der Objektname des Objektes verwendet.
* `trigger`  
Trigger-Wert, bei welchem die Störmeldung, als "*ausgelöst*" angezeigt wird. Wird der Wert `trigger` nicht angegeben, wird der Default Trigger-Wert verwendet. Dieser ist standardmäßig `true`, kann aber auch für die gesamte Störmeldeliste geändert werden.

### Callback
Lua Funktion, welche aufgerufen wird, wenn eine Störmeldung ausgelöst wurde. Der Funktion werden alle aktuellen Werte der Störmeldung übergeben, um nach dem Auslösen weiter Aktionen ausführen zu können.

## Beispiel
```lua
require('applibs.alertmanager.functions')

list = 1
tag = 'sm'
settings = {}

callback = function (msg)
  log(msg)
end

settings['33/1/1'] = {delayoff = 3, message="My Message", trigger = false}

delayedAlerts(list, tag, settings, callback)
```