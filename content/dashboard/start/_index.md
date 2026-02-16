---
title: "Erste Schritte"
type: docs
weight: 1
bookCollapseSection: false
---
# Erste Schritte

## Zusammenfassung
Mit der Energy Dashboard-App können Dashboards zur grafischen Darstellung von Energieflüssen und -verbrauch erstellt werden.
Ein Dashboard besteht aus mehreren Widgets. Jedes Widget enthält Anzeigeinformationen in Form von Diagrammen, Energieflüssen, Messanzeigen oder anderen HTML-Seiten.

Anbei ein Beispiel, wie ein fertiges Dashboard aussehen könnte.

{{< image src="dashboard.png" alt="Dashboard" title="Dashboard" >}}

## Using the Energy Dashboard app

### 1. Klicken Sie auf die Energy Dashboard-App auf dem Startbildschirm des Wiser for KNX / spaceLYnk-Controllers. (![1](../1.png)).
{{< image src="start-dashboard.png" alt="Start Dashboard" title="Start Dashboard" >}}

### 2. Dashboard Übersicht
Alle verfügbaren Dashboards werden auf der Dashboard-Übersichtsseite (![3](../3.png)) angezeigt. Sie können die App auch beenden, indem Sie auf das Schließen-Symbol (![1](../1.png)) in der oberen rechten Ecke klicken.
Über das Zahnrad-Symbol (![2](../2.png)) gelangen Sie zur Konfigurationsoberfläche für die verschiedenen Dashboards. Es wird nur angezeigt, wenn Sie mit dem Administratorkonto angemeldet sind.
Wenn das Zahnrad-Symbol auch mit dem Administratorkonto nicht angezeigt wird, fahren Sie mit Schritt 3 fort. Andernfalls können Sie mit Schritt 4 fortfahren.

{{< image src="start-dashboards.png" alt="Dashboards" title="Dashboards" >}}

### 3. Administrator Zugriff auf das Energie-Dashboard aktivieren
Gehen Sie zu **Configurator** → **Benutzerzugang** → **Einstellungen Benutzerzugriff** → aktivieren Sie "**Aktiviere Passwort für Apps**" → klicken Sie auf "**Speichern**".

{{< image src="admin-access.png" alt="Administrator Zugang" title="Administrator Zugang" >}}

### 4. Bereiche der Energy Dashboard App
{{< image src="dashboard-areas.png" alt="Energy Dashboard App Bereiche" title="Energy Dashboard App Bereiche" >}}

#### ![1](../1.png) [Dashboards](/dashboard/dashboards/)
Im Bereich **Dashboards** können Sie verschiedene Dashboards erstellen und das Layout der einzelnen Widgets festlegen. Außerdem können Sie hier den Inhalt für jedes einzelne Widget festlegen.

#### ![2](../2.png) [Charts](/dashboard/charts/)
Die verschiedenen Diagramme werden im Abschnitt **Charts** erstellt. Derzeit können Torten, Donut und Balkendiagramme erstellt werden.

#### ![3](../3.png) [Gauges](/dashboard/gauges/)
Einzelne Messelemente können unter **Gauges** erstellt werden. Ein Messgerät ist ein Zeigerinstrument, das einen Wert in einem Halbkreis anzeigt.

#### ![4](../4.png) [Energyflows](/dashboard/energyflows/)
Energieflüsse können verwendet werden, um die Energieverteilung in Gebäuden grafisch darzustellen. Unter **Energyflows** kann eine animierte Grafik erstellt werden, die den aktuellen Energiefluss im Gebäude anzeigt.

#### ![5](../5.png) [Settings](/dashboard/settings/)
Globale Designeinstellungen für alle Dashboards können im Bereich **Settings** definiert werden. Darüber hinaus kann das Erscheinungsbild der Dashboards mit benutzerdefiniertem JavaScript- und CSS-Code weiter angepasst werden.

#### ![6](../6.png) Close button
Verwenden Sie die Schaltfläche **Schließen**, um zur Übersicht aller erstellten Dashboards zurückzukehren.