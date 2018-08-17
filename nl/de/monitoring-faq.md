---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Überwachung - Häufig gestellte Fragen

<a name="48"></a>
## Ich sehe eine Vielzahl von Überwachungsalert-Tickets. Bedeutet das, dass mein Server inaktiv ist?

Jedes Gerät verfügt über eine kostenlose Ping-Überwachung und einen entsprechenden Benachrichtigungsservice. Dieser Service erstellt automatisch beim Fehlschlagen festgelegter Parameter ein Überwachungsalert-Ticket. Fehlalarme sind bei dem Überwachungsservice möglich und können auf eine Übertragungsbegrenzung durch eine Software-Firewall auf dem Server, eine bestimmte Service- und Anwendungsverfügbarkeit und Serviceunterbrechungen in der Überwachungsinfrastruktur zurückgeführt werden. Überprüfen Sie die Standardeinstellungen, um die Möglichkeit falscher Überwachungsalerts zu verringern. 

<a name="354"></a>
## Kann ich das Überwachungssystem so konfigurieren, dass ein automatischer Warmstart durchgeführt und ein Support-Techniker benachrichtigt wird, falls der Server ausfällt?

Ja. Mit dem Service **Automatischer Warmstart nach Überwachungsfehler** könne Sie das Überwachungssystem so konfigurieren, dass der Server automatisch neu gestartet und ein Ticket für einen Support-Techniker geöffnet wird, wenn ein Überwachungsalert ausgegeben wird. 

<a name="1699"></a>
## Was ist der Unterschied zwischen einer Überwachung mit einem 'langsamen Ping' und einem 'Service-Ping'?

Der Unterschied zwischen einem Service-Ping und einem langsamen Ping ist die Zeitspanne, innerhalb der eine Antwort von einem Gerät erwartet wird. Standardmäßig wird der Service-Ping verwendet, Sie können aber die Einstellung auch so ändern, dass ein langsamer Ping verwendet wird.

* Ein **Service-Ping** setzt alle fünf Minuten einen Ping ab und erwartet innerhalb von einer Sekunde eine Echoantwort. Wenn mehr als ein Ping verpasst wird, wird ein Alert ausgegeben.
* Ein **langsamer Ping** wartet fünf Sekunden auf eine Antwort, was Servern, die für netzfremde Tasks optimiert sind, mehr Zeit bei der Verarbeitung der Anforderung einräumt. 


<a name="1000"></a>
## Sehen Techniker, wenn ein Überwachungsticket geöffnet wird und mich auf das Problem aufmerksam macht, dieses Ticket und reagieren darauf?

Mit dem einfachen Ping-Service werden Support-Techniker nicht über Ausfälle informiert. Diese Tickets werden geöffnet, wenn das Überwachungssystem einen Alert ausgibt, und es werden nur die Benutzer benachrichtigt, die Sie in der Überwachungsanzeige angeben. Techniker werden nur dann benachrichtigt, wenn Sie ein neues Ticket mit dem Hinweis öffnen, dass der Server nicht antwortet.

