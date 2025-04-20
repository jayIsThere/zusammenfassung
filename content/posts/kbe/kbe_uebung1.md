+++
title = 'KBE Übung 1'
date = 2025-04-10T18:08:29+02:00
categories = ['KBE Übung']
tags = []
draft = false
+++

Übungsblatt 1
-------------

### Aufgabe 1. Grundstrategie des Software-Engineerings

**Ziel der Wiederverwendung**:  
- Wiederverwendung vorhandener Software, statt neue Software von Grund auf zu entwickeln.


### Aufgabe 2. Aspekte, die den Ansatz getrieben haben:

- Geringere Produktions- und Wartungskosten
- Schnellere Auslieferung von Systemen
- Höhere Softwarequalität


### Aufgabe 3. Beispiele für etablierte wiederverwendbare Software:

- Open Source Code (z. B. Apache Commons)
- ERP-Systeme (z. B. SAP)
- Komponentenbibliotheken
- Webservices (z. B. PayPal)


### Aufgabe 4. Größenordnungen von Softwareeinheiten (von groß nach klein):

- Systeme
- Anwendungen
- Softwareproduktlinien
- Komponenten
- Objekte und Funktionen


### Aufgabe 5. Beispiele für jede Größenordnung:

- **System**: Ein ERP-System, z. B. SAP
- **Anwendung**: Ein CRM-System
- **Produktlinie**: Softwarelinie für medizinische Geräte
- **Komponente**: Zahlungsmodul
- **Funktion/Objekt**: Logging-Klasse aus Apache Commons


### Aufgabe 6. Vorteile der Wiederverwendung:

- Geringere Kosten
- Höhere Zuverlässigkeit
- Geringeres Entwicklungsrisiko
- Schnellere Markteinführung
- Effektiver Einsatz von Experten
- Standardkonformität


### Aufgabe 6. Probleme der Wiederverwendung:

- Höhere Wartungskosten
- Mangel an Werkzeugunterstützung
- "Not-invented-here"-Syndrom
- Hoher Aufwand für Bibliotheksverwaltung
- Schwierige Suche und Anpassung von Komponenten


### Aufgabe 7. Planung der Wiederverwendung

**Vier Schlüsselfaktoren:**

- Entwicklungszeitplan
- Erwartete Lebensdauer der Software
- Erfahrung des Entwicklerteams
- Wichtigkeit/Nicht-funktionale Anforderungen


### Aufgabe 8. Schlüsselfaktoren bei .NET und schneller Verfügbarkeit:

- Plattformabhängigkeit (→ .NET-Kompatibilität)
- Geringer Entwicklungsaufwand durch Wiederverwendung fertiger Systeme


### Aufgabe 9-12. Anwendungsframeworks

**Attribute von Frameworks:**

| Attribut | Passt? |
|----------|--------|
| Konfigurierbar | ✅ Ja |
| Generisch | ✅ Ja |
| Call-back | ✅ Ja |
| Unterstützung konkreter Geschäftsaktivitäten | ✅ Ja |
| Inversion of Control | ✅ Ja |
| Inhärent erweiterbar | ✅ Ja |
| Basis sehr ähnlicher Systeme | ✅ Ja |
| Unterstützung für Hardware-Schnittstellen | ❌ Teilweise (meist Software) |
| Immer objektorientiert | ❌ Nein (meist, aber nicht zwingend) |

**Drei Architektur- und Entwurfsmuster, auf denen WAFs basieren:**

- Model-View-Controller (MVC)
- Observer Pattern
- Strategy Pattern (auch Composite Pattern möglich)

**Funktion von WAFs oder Entwicklern:**

| Funktion | WAF | ENT |
|----------|-----|-----|
| Zahlungstransaktion über Kreditkarte durchführen |  | ✅ |
| Verwaltung des Inhalts eines Shop-Warenkorbs | ✅ |  |
| Abfragedaten in einer Tabelle aufbereiten | ✅ |  |
| Am System anmelden und abmelden | ✅ |  |
| Zugriff auf ein Geoinformationsdienst |  | ✅ |
| Bestimmung des aktuellen Standorts über GPS |  | ✅ |
| Asynchrone Aktualisierung durch Auswahl eines Listeneintrags | ✅ |  |
| Geänderte Daten nach dem Speichern sichtbar machen | ✅ |  |
| Ermittlung verschiedener Bahn-Routen |  | ✅ |
| Nutzung einer 3D-Spiele-Engine |  | ✅ |
| Geschäftsdaten persistieren | ✅ |  |

**Unterschied Framework vs. Bibliothek:**

- Bei **Bibliotheken** ruft die Anwendung die Bibliothek auf.
- Bei **Frameworks** ruft das Framework die Anwendung auf.
    - → Inversion of Control (IoC, „Hollywood Principle“: "Don't call us, we'll call you")


### Aufgabe 13-15. Softwareproduktlinien

**Was ist eine Softwareproduktlinie und wann ist sie effizient?**  
- Eine Produktlinie ist ein Satz verwandter Anwendungen mit gemeinsamer Architektur.
- Effizient, wenn viele ähnliche, aber nicht identische Systeme benötigt werden.

**Aufbau des Basissystems:**

- Kernkomponenten (nicht veränderbar)
- Konfigurierbare Komponenten
- Spezielle Anwendungskomponenten

**Voraussetzung bei Nutzung von Frameworks für Produktlinien:**

- Das Framework muss erweiterbar und anpassbar sein, um domänenspezifische Komponenten einzubetten.

### Aufgabe 16-19. Anwendungssysteme

**Welche Aussagen über Anwendungssysteme sind korrekt?**

| Aussage | Ja |
|---------|-----|
| Lassen sich viel schneller zuverlässig bereitstellen | ✅ |
| Sind im Kern sehr gut auf kundenspezifische Bedürfnisse zugeschnitten | ❌ |
| Support-Ratschläge = Verkaufsfokus, nicht Bedarfsermittlung | ✅ |
| Gut zur Abbildung bestehender Geschäftsprozesse geeignet | ✅ |
| Anpassbar ohne Quellcode-Änderung | ✅ |
| Technologie-Updates = Verantwortung des Herstellers | ✅ |
| Für Unternehmen mit ähnlichen Systemanforderungen geeignet | ✅ |

**Zwei Ansätze von Anwendungssystemen:**

- **Konfigurierbare Anwendungssysteme**: Einzelprodukt, Konfiguration
- **Integration von Anwendungssystemen**: Mehrere Systeme, Anpassung durch Integration

**Zuordnung der Aussagen:**

| Aussage | Ansatz |
|---------|--------|
| Schwerpunkt: Systemintegration | 2 |
| Systemanbieter liefert Plattform | 1 |
| Einzelprodukt liefert benötigte Funktionalität | 1 |
| Entwicklung flexibler Lösungen für Kundenprozesse | 2 |
| System basiert auf generischer Lösung und standardisierten Prozessen | 1 |
| Wartung = Verantwortung des Systembesitzers | 2 |

**Beispielsysteme für beide Ansätze:**

- **Konfigurierbares Anwendungssystem**: SAP ERP
- **Integriertes Anwendungssystem**: E-Commerce-System mit ERP- und E-Mail-Anbindung

