---
title: "Wertänderungen protokollieren"
type: docs
weight: 4
bookCollapseSection: false
---
# Wertänderungen protokollieren
Mit dem Parameter [`showhistory`](/alertmanager/konfiguration-schreiben/#showhistory) werden alle Wertänderungen der einzelnen Störmeldungen protokolliert und können in der Störmeldeliste über einen zusätzlichen Button (![1](../1.png)) aufgerufen werden.

{{< image src="history-button.png" alt="History Button" title="History Button" >}}

In einem Popup Fenster kann nun jeder Wert mit einem Zeitstempel eingesehen werden. Bei **nicht booleschen** Datenpunkten wird neben dem Trigger Wert, auch nocht der tatsächliche Wert der Störmeldung angezeigt.

{{< image src="history-modal.png" alt="History" title="History" >}}
