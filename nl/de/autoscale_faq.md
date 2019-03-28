---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-16"

keywords:

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# Häufig gestellte Fragen: Auto Scale
{: faqs-auto-scale}

## Unterstützt Auto Scale Skalierungsinstanzen mit Bare-Metal?
{:faq}

Auto Scale unterstützt gegenwärtig keine Bare-Metal-Instanzen für die automatische Skalierung.

## Funktioniert Auto Scale mit Lastausgleichsfunktionen?
{:faq}

Ja, Auto Scale funktioniert derzeit für lokale Lastausgleichsfunktionen und nutzt einen Teil der API der Lastausgleichsfunktion. Weitere Informationen finden Sie in [Lastausgleichsfunktionen für die Skalierung](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#scalelb).

## Welche Beendigungsrichtlinien gibt es im Einzelnen für die automatische Skalierung?
{:faq}

In Auto Scale gibt es die folgenden drei Beendigungsrichtlinien für die Beendigung der automatischen Skalierung: 'Neueste/r/s', 'Älteste/r/s' und 'Nächste/r/s zur nächsten Gebühr'. Diese Richtlinien beschreiben, welche Mitglieder bei der vertikalen Skalierung durch Scale-down entfernt werden sollen. Weitere Informationen finden Sie in [Beendigungsrichtlinie](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#termination).

## Was sind Auto Scale-Richtlinien für die automatische Skalierung?
{:faq}

Eine Richtlinie beinhaltet eine Gruppe von Aktionen und eine Gruppe von Auslösern. Richtlinien bestehen normalerweise aus den folgenden Elementen: Name, Ruhephase, Aktion und Auslöser. Weitere Informationen finden Sie in [Richtlinien](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#policies).

## Was sind Auto Scale-Auslöser für die automatische Skalierung?
{:faq}

Auslöser entsprechen Bedingungen, die erfüllt werden können, jedoch nur, wenn die Gruppe aktiv ist. Es gibt drei Typen von Auslösern: Einmalige Auslöser, wiederkehrende Auslöser und Ressourcennutzungsauslöser. Weitere Informationen finden Sie in [Auslöser](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#triggers).

## Was ist die maximale Anzahl an VSI-Mitgliedern?
{:faq}

Dies ist die Obergrenze für die Anzahl von Mitgliedern, die in einer Gruppe maximal enthalten sein dürfen. Weitere Informationen finden Sie in [Maximale Anzahl von VSI-Mitgliedern](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#max_virtual_member).

## Was ist die Mindestanzahl von VSI-Mitgliedern?
{:faq}

Dies ist die Untergrenze für die Anzahl von Mitgliedern, die mindestens in einer Gruppe enthalten sein müssen. Weitere Informationen finden Sie in [Mindestanzahl von VSI-Mitgliedern](/docs/infrastructure/SLautoscale?topic=slautoscale-auto-scale-terminology#min_virtual_member).

## Was ist ein Auto Scale-Asset?
{:faq}

Ein Asset ist ein festes Mitglied in einer Gruppe, dessen Vorhandensein sich nicht in der Anzahl von Mitglied niederschlägt und das in keiner Weise automatisch gesteuert wird. Das Asset ist vorhanden, um zusätzliche Informationen für die Richtlinienauslöser bereitzustellen. Ein Asset kann zum Beispiel zum CPU-Prozentsatz der gesamten Gruppe beitragen, wenn der CPU-Prozentsatz als Auslöser verwendet wird. Gegenwärtig kann eine Gruppe nur über virtuelle Gast-Assets verfügen, für deren Anzahl es keinen Grenzwert gibt. Darüber hinaus ist eine Gruppe nicht erforderlich.

## Was ist eine Auto Scale-Gruppe für die automatische Skalierung?
{:faq}

Eine Gruppe (Skalierungsgruppe) ist eine regionale und gruppenspezifische Sammlung von Assets, Mitgliedern, Lastausgleichsfunktionen für die Skalierung, VLANs und Richtlinien. Eine Gruppe beinhaltet alle Parameter für die Skalierung, einschließlich den Grenzwerten für die Anzahl von Mitgliedern und den Vorlagen für die Skalierung von VSI-Mitgliedern.

## Was ist ein Auto Scale-Mitglied für die automatische Skalierung?
{:faq}

Ein Mitglied ist eine skalierte Einheit in einer Gruppe. Mitglieder werden basierend auf Richtlinienaktionen automatisch bereitgestellt oder zurückgefordert. Derzeit sind alle Mitglieder VSIs. Eine aktive Gruppe umfasst nie weniger Mitglieder als durch die Untergrenze (Mindestanzahl) oder mehr Mitglieder als durch die Obergrenze (Höchstanzahl) festgelegt. Normalerweise werden Mitglieder zwar durch Aktionen einer Richtlinie hinzugefügt, aber sie können auch manuell von einem Benutzer hinzugefügt werden.
