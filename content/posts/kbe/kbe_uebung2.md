+++
title = 'KBE Übung 2'
date = 2025-04-17T18:08:32+02:00
categories = ['KBE Übung']
tags = []
draft = false
+++

Übungsblatt 2
-------------

### Aufgabe 1. Beweggründe für die Entstehung des Komponentenbasierten Software-Engineerings

**Wiederverwendbarkeit**:  
- Softwarekomponenten können wiederverwendet werden, was Entwicklungszeit und Kosten spart.

**Modularität**:  
- Komponenten sind unabhängig, was Wartung und Erweiterung vereinfacht.

**Flexibilität**:  
- Komponenten können ausgetauscht werden, ohne das gesamte System zu ändern.

**Skalierbarkeit**:  
- Komponenten können unabhängig skaliert und optimiert werden.


### Aufgabe 2. Vier Grundlagen des Komponentenbasierten Software-Engineerings

**Unabhängige Komponenten**:  
- Komponenten können ohne Systemänderungen ausgetauscht werden.

**Komponentenstandards**:  
- Einheitliche Schnittstellen und Integrationen sind wichtig.

**Middleware**:  
- Unterstützung für Kommunikation, Ressourcenmanagement, Transaktionen, Sicherheit und Parallelität.

**Komponentenorientierter Entwicklungsprozess**:  
- Komponenten können während der Planung und Entwicklung angepasst und wiederverwendet werden.


### Aufgabe 3. Probleme der Vertrauenswürdigkeit von Komponenten

**Blackbox-Natur**:  
- Quellcode nicht verfügbar, schwierige Transparenz.

**Kein Zugriff auf den Quellcode**:  
- Es ist schwierig, Fehler zu erkennen.

**Unerwartete Seiteneffekte**:  
- Das Zusammenspiel von Komponenten kann unvorhergesehene Probleme verursachen.


### Aufgabe 4. Drei grundlegende Entwurfsprinzipien des Komponentenbasierten Software-Engineerings

**Unabhängigkeit**:  
- Komponenten beeinflussen sich nicht gegenseitig.

**Klar definierte Schnittstellen**:  
- Stabiler API-Austausch möglich.

**Komponenteninfrastruktur mit Standarddiensten**:  
- Weniger Eigenentwicklung notwendig, Fokus auf Integration.


### Aufgabe 5. Eigenschaften von Komponenten (Sommerville)

**Unabhängigkeit**:  
- Komponenten sind autonome Einheiten.

**Modularität**:  
- Komponenten sind isolierte Einheiten, die unabhängig entwickelt werden können.

**Wiederverwendbarkeit**:  
- Komponenten können in verschiedenen Systemen verwendet werden.

**Dienstanbieter**:  
- Komponenten bieten Dienste, ohne dass der Benutzer den internen Zustand kennt.


### Aufgabe 6. Kritische Vorteile der Betrachtung einer Komponente als Dienstanbieter

**Unabhängigkeit**:  
- Komponenten werden über Schnittstellen aufgerufen und sind nicht von der Umgebung abhängig.

**Sprachunabhängigkeit**:  
- Komponenten können in verschiedenen Programmiersprachen implementiert werden.


### Aufgabe 7. Unterschiede zwischen Komponenten und Objekten

| Merkmal              | Komponente                        | Objekt                         |
|----------------------|-----------------------------------|--------------------------------|
| **Deployment**        | Direkt auf Plattform installierbar | Teil eines Programms (kompiliert) |
| **Typdefinition**     | Instanz                           | Basierend auf Klasse (Typ)    |
| **Transparenz**       | Blackbox (nur Schnittstelle sichtbar) | Oft transparenter (mehr Einblick) |
| **Sprachabhängigkeit**| Sprachunabhängig                  | Sprachgebunden (z. B. Java)    |
| **Standardisierung**  | Muss Modell folgen                | Frei definierbar               |


### Aufgabe 8. Unterschiedliche Schnittstellen von Komponenten

**Bereitgestellte Schnittstelle (provided interface)**:  
- Definiert die Dienste, die von der Komponente angeboten werden.

**Benötigte Schnittstelle (required interface)**:  
- Definiert, welche Dienste die Komponente benötigt, ohne zu spezifizieren, wie sie bereitgestellt werden.


### Aufgabe 8. UML-Diagramm

---


### Aufgabe 10. UML-Darstellung der „DataBroker“-Komponente

- Eine Komponente wird durch ein Rechteck dargestellt, das die Schnittstellen und die dazugehörigen „bereitgestellten“ und „benötigten“ Schnittstellen (mit kleinen Rechtecken) enthält.


### Aufgabe 11. Prinzip eines Komponentenmodells

**Prinzip**:  
- Ein Komponentenmodell definiert, wie Komponenten strukturiert, interagieren und konfiguriert werden.

**Beispiele**:  
- SOAP (WSDL), Jakarta Beans (CDI), Microsoft .NET (CIL).


### Aufgabe 12. Drei allgemeine Aspekte der Grundelemente eines Komponentenmodells

**Schnittstellen**:  
- Definiert die bereitgestellten und benötigten Dienste.

**Nutzung**:  
- Globale Bezeichner (z. B. URI, JNDI).

**Bereitstellung & Verpackung**:  
- Konfiguration, Dokumentation und Meta-Informationen.


### Aufgabe 13. Unterschied zwischen Plattform- und Hilfsdiensten einer Middleware

**Plattformdienste**:  
- Grundlegende Funktionen wie Kommunikation, Ressourcenverwaltung, Transaktionen, Persistenz.

**Hilfsdienste**:  
- Ergänzende Dienste wie Authentifizierung, die Inkompatibilitäten verhindern.


### Aufgabe 14. Implementierung eines Komponentenmodells

**Container**:  
- Eine Laufzeitumgebung, die Middleware-Dienste für die Ausführung von Komponenten bereitstellt.


### Aufgabe 15. Aussagen zu Containern und Komponenten

| Aussage                                                         | Ja/Nein |
|-----------------------------------------------------------------|---------|
| Ein Container ist die Hauptkomponente jeder Applikation         | Nein    |
| Eine Komponente kann auf den Transaktionsdienst zugreifen      | Ja      |
| Der Container ermöglicht, dass Komponente A auf die Schnittstelle von B zugreifen kann | Ja      |
| Komponenten sind Hilfsdienste des Containers                    | Nein    |
| Der Container kann auf Komponentenschnittstellen zugreifen      | Nein    |
| Die Adressierung von Komponenten ist ein Hilfsdienst des Containers | Ja      |

---
---
---
#### Übungsblatt 3
-------------

#### Übungsblatt 4
-------------

