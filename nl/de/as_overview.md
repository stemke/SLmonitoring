---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-09"

keywords:

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Informationen zu Auto Scale
{: #as-overview}

Auto Scale bietet die Möglichkeit, den Prozess der manuellen Skalierung beim Hinzufügen oder Entfernen virtueller Server zur Unterstützung Ihrer Geschäftsanwendungen zu automatisieren. Die Funktion der automatischen Skalierung kann über die API oder das Steuerportal verwaltet werden und ermöglicht Folgendes:

* Nahtlose und automatische vertikale Skalierung von virtuellen Servern per Scale-up, wenn aufgrund eines Anstiegs der Nachfrage zusätzliche Ressourcen benötigt werden.
* Nahtlose und automatische vertikale Skalierung virtueller Server per Scale-down durch Abbau unnötiger Ressourcen bei sinkender Nachfrage, wodurch Sie Einsparungen erzielen.
* Flexible Skalierungsauslöser, einschließlich belegtem CPU-Prozentsatz, abgehender öffentlicher und privater Bandbreite sowie eingehender öffentlicher und privater Bandbreite.
* Echtzeitnahe Statusaktualisierungen für die Skalierungsaktivität in Gruppen.
    Optionale Integration von virtuellen LANs (VLANs) sowie von lokalen Lastausgleichsfunktionen.

Es gibt zwei gängige Geschäftslösungen, auf die die automatische Skalierung angewendet werden kann - [zeitplanbasierte](/docs/infrastructure/SLautoscale?topic=slautoscale-managing-weekly-traffic-spikes-with-auto-scale-schedule-based-scaling) Skalierung und [ressourcenbasierte](/docs/infrastructure/SLautoscale?topic=slautoscale-managing-traffic-spikes-with-auto-scale-resource-based-scaling) Skalierung. Die zeitplanbasierte Skalierung kann verwendet werden, wenn ein Unternehmen einen Anstieg des Datenverkehrs erwartet, wie z. B. eine Social-Networking-Site, die zeitplangenau zusätzliche Ressourcen erfordert. Die ressourcenbasierte Planung findet statt, um die Markteinführung eines Produkt voranzutreiben oder wenn eine E-Commerce-Site verkaufsfördernde Maßnahmen anwendet und zusätzliche Ressourcen benötigt werden, um die Antwortzeiten aufrechtzuerhalten. Um die automatische Skalierung nutzen zu können, benötigen Sie Folgendes:

* Ein IBM Cloud-Konto.
* Die Berechtigung zur Verwendung von Auto Scale. Die Erteilung der Berechtigung erfolgt durch das Konto des Masterbenutzers, der automatisch die Genehmigung zur Nutzung von Auto Scale erhält.
* Zugriff auf alle virtuellen Server.

Auto Scale verwendet Gruppen, in denen die Richtlinien enthalten sind, die bestimmen, wie Ihre Umgebung erweitert oder verkleinert wird. Diese Richtlinien verwenden Aktionen, um in Übereinstimmung mit Ihren Geschäfts- und Anwendungsanforderungen virtuelle Server hinzuzufügen bzw. zu entfernen.
