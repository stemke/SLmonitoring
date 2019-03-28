---

copyright:
  years: 2014, 2018
lastupdated: "2018-08-17"

keywords: auto scale, scale out, scale down

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Einführung in die automatische Skalierung
{: #getting-started-with-auto-scaling}

Mit der automatischen Skalierung können Sie den Prozess der manuellen Skalierung beim Hinzufügen oder Entfernen virtueller Server zur Unterstützung Ihrer Geschäftsanwendungen automatisieren.
{:shortdesc}

Hauptmerkmale:

* Nahtloses und automatisches bedarfsgesteuertes Scale-out (horizontale Skalierung) von virtuellen Servern, wenn zusätzliche Ressourcen erforderlich sind
* Nahtloses und automatisches bedarfsgesteuertes Scale-down von virtuellen Servern und Einsparung von Kosten für nicht benötigte Ressourcen
* Flexible Auslöser für die Skalierung: CPU-Prozentsatz, abgehende öffentliche und private Bandbreite, eingehende öffentliche und private Bandbreite
* Statusaktualisierungen in Echtzeit für die Skalierungsaktivität in Gruppen
* Optionale Integration von VLAN und Lastausgleichsfunktion


## Vorbereitende Schritte

Bevor Sie beginnen, überprüfen Sie die folgenden Voraussetzungen.

  1. Informieren Sie sich über die [automatische Skalierung](/docs/infrastructure/SLautoscale?topic=slautoscale-about-auto-scale).
  2. Stellen Sie sicher, dass Sie über die richtigen [Benutzerberechtigungen](/docs/infrastructure/SLautoscale?topic=slautoscale-user-permissions-required-to-use-auto-scale) verfügen.

## Gruppe für die automatische Skalierung erstellen

Überprüfen Sie die Optionen der automatischen Skalierung mit Auto Scale und bestimmen Sie, ob die zeitplanbasierte oder aber die ressourcenbasierte automatische Skalierung für Sie geeignet ist.
<table>
  <tr><th> Optionen der automatischen Skalierung mit Auto Scale</th>
    <th>Beschreibung</th>
  </tr>
  <tr><td>[Zeitplanbasierte automatische Skalierung](/docs/infrastructure/SLautoscale?topic=slautoscale-managing-weekly-traffic-spikes-with-auto-scale-schedule-based-scaling)</td>
    <td>Verwenden Sie die automatische Skalierung, um Richtlinien für zeitbasierte Lastspitzen wie an Wochenenden oder Feiertagen einzurichten.</td>
  </tr>
  <tr><td>[Ressourcenbasierte automatische Skalierung](/docs/infrastructure/SLautoscale?topic=slautoscale-managing-traffic-spikes-with-auto-scale-resource-based-scaling)</td>
    <td>Verwenden Sie die automatische Skalierung, um Richtlinien für zeitpunktunabhängige, unregelmäßige Lastspitzen auf Grundlage der Ressourcennutzung einzurichten.</td>
  </tr>
  </table>
