---
title: "Störmeldung quittieren"
type: docs
weight: 3
bookCollapseSection: false
---
# Störmeldung quittieren
Eine Störmeldung, kann über den Button **quittieren** quittiert werden, dies führt dazu, dass diese nicht mehr {{< badge style="danger" value="rot blinkend" >}} angezeigt wird, sondern nur noch mit einem {{< badge style="warning" value="orange" >}} hinterlegten Hintergrund. Alternativ kann eine Störmeldung mit einem **event** Skript mit der Funktion `ackAlert()` quittiert werden.

## ackAlert(list, addr)

* `list`: Nummer der Störmeldeliste
* `addr`: Objekt Adresse (z.B. **1/1/1**)

## Beispiel
```lua
require('applibs.alertmanager.functions')

listnr = 1
ackAlert(listnr, '1/1/1')
```