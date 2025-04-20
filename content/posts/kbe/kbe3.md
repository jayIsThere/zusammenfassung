+++
title = 'Vorlesung 3: komponentenbasiertes Software-Engineering'
date = 2025-04-17T18:13:15+02:00
categories = ['KBE']
tags = ['komponente', 'schnittstelle']
draft = false
+++

### Grundprinzipien des komponentenbasierten Software-Engineerings ### 

**Unabhängige Komponenten**  
- Vollständig konfigurierbar über ihre Schnittstellen  
- Schnittstelle klar getrennt von der Implementierung  
- Austauschbar ohne Änderung am System

**Komponentenstandards**  
- Einheitliche Schnittstellendefinition & Integration  
- Umsetzung über Komponentenmodelle, z. B.:
    - Schnittstellenbeschreibung
    - Kommunikationsweise zwischen Komponenten

**Middleware**  
- Serverseitige Unterstützung für:
    - Kommunikation verteilter Komponenten
    - Ressourcenmanagement
    - Transaktionsverwaltung, Sicherheit, Parallelität

**Komponentenorientierter Entwicklungsprozess**  
- Anforderungen an vorhandene Komponenten anpassbar  
- Wiederverwendung während Planung & Entwicklung


### ⚠️ Probleme & Herausforderungen im KBSE ### 

**Vertrauenswürdigkeit der Komponenten**  
- Blackbox-Natur erschwert Vertrauen  
- Kein Quellcode = wenig Transparenz

**Komponentenzertifizierung**  
- Wer zahlt, wer haftet?  
- Keine klare Verantwortung, rechtlich unsicher

**Vorhersage emergenter Eigenschaften**  
- Integration ≠ Summe der Einzelteile  
- Unerwartete Seiteneffekte durch Zusammenspiel

**Anforderungskompromisse**  
- Reale Anforderungen vs. Verfügbarkeit  
- Notwendigkeit strukturierter Analysemethoden


### 🧩 Zentrale Entwurfsprinzipien im KBSE ### 

**Unabhängigkeit**  
- Komponenten beeinflussen sich nicht gegenseitig

**Klar definierte Schnittstellen**  
- Austauschbar bei stabiler API

**Komponenteninfrastruktur mit Standarddiensten**  
- Weniger Neuentwicklung nötig  
- Fokus auf Integration statt Eigenentwicklung


### Komponenten als Dienstanbieter ### 

- Komponenten stellen Dienste bereit und kapseln deren Implementierung.
- Aufgerufen vom System, ohne zu wissen:
    - Wo sie ausgeführt werden
    - In welcher Sprache sie geschrieben sind

**Vorteile**  
- Unabhängig & ausführbar über ihre Schnittstelle
- Schnittstellenbasiert → kein Zugriff auf internen Zustand nötig


.... (Tabelle fehlt)


###  🔍 Komponenten vs. Objekte ### 

| Merkmal                | Komponente                     | Objekt                          |
|------------------------|--------------------------------|---------------------------------|
| **Deployment**          | Direkt auf Plattform installierbar | Teil eines Programms (kompiliert) |
| **Typdefinition**       | Ist eine Instanz               | Basierend auf Klasse (Typ)     |
| **Transparenz**         | Blackbox, Schnittstelle-only   | Oft transparenter               |
| **Sprachabhängigkeit**  | Sprachunabhängig               | Sprachgebunden (z. B. nur Java) |
| **Standardisierung**    | Muss Komponentenmodell folgen  | Frei definierbar                |


Sprachabhängigkeit : Java ist eher sprachabhängig aber .NET(Microsoft) ist universell.

### 🧩 Komponentenschnittstellen ### 

**Stellt bereit (provided interface)**  
- API der Komponente – was sie bietet

**Benötigt (required interface)**  
- Welche Dienste sie selbst braucht, um korrekt zu funktionieren  
- Definiert nicht, wie diese bereitgestellt werden


### 🎯 Visualisierung in UML (kompakt) ### 

🧱 **Komponente**  
- Wird mit Rechteck + 2 kleinen Rechtecken dargestellt
- Enthält:
    - Realisierungsklassen
    - "Stellt bereit"- und "Benötigt"-Schnittstellen (sichtbar an Port-Notationen)


### Schnittstellenspezifikation in Komponentenmodellen ### 

- Komponenten werden über ihre Schnittstellen definiert
- Das Komponentenmodell regelt:
    - Wie Schnittstellen aufgebaut sind
    - In welcher Sprache sie beschrieben werden

**Beispiele**  
- SOAP Webservices → WSDL (XML)
- Jakarta Beans / CDI → Java
- Microsoft .NET → CIL


### 🧩 Grundelemente eines Komponentenmodells ### 

| Element              | Beschreibung                                                        |
|----------------------|---------------------------------------------------------------------|
| **Schnittstellen**    | Bereitgestellte + benötigte Dienste                                  |
| **Nutzung**           | Globale Bezeichner/Handles (z. B. URI, JNDI)                         |
| **Bereitstellung & Verpackung** | inkl. Konfigurationsoptionen, Doku, Meta-Infos           |
| **Komposition**       | Wie Komponenten zusammengebaut werden                                |
| **Anpassung**         | Konfigurierbar für konkrete Einsatzszenarien                         |
| **Evolution**         | Austausch- und Update-Regeln                                          |
| **Dokumentation & Namenskonvention** | Strukturierter Zugriff & Übersicht                      |

**Metadatenzugriff**  
- z. B. via Reflection (Java)

Beispiel für Schnittstellen : WSDL für SOAP, CDI-Beans für Java, CIL für .NET
URI, JNDI?



### ⚙️ Bereitstellung & Anpassung ### 

- Komponenten sind unabhängig lauffähig
- Müssen komplett mit benötigter Infrastruktur geliefert werden
- Doku & Austauschregeln sind Teil des Modells
- Unterstützung für Konfigurierbarkeit & Wiederverwendbarkeit


Beispiel: MAVEN

jar file mit free pdf?


### 🛠️ Middleware-Dienste im Komponentenmodell ### 

**Zwei Kategorien:**  
1. **Plattformdienste**  
    (grundlegend für verteilte Kommunikation)
    - Komponentenkommunikation
    - Ressourcenverwaltung
    - Adressierung
    - Ausnahmebehandlung
    - Transaktionsverwaltung
    - Informationssicherheit
    - Persistenz
    - Nebenläufigkeit

2. **Hilfsdienste**  
    (ergänzend, z. B. Authentifizierung)
    - Entlasten die Entwicklung, verhindern Inkompatibilitäten

### 🧃 Container als Laufzeitumgebung ### 

- **Container** = Laufzeitumgebung mit Middleware-Diensten
- Besteht aus:
    - Dienstimplementierungen
    - Definitionen für Schnittstellenintegration

**Effekt:**  
- Komponente nutzt Containerdienste über bereitgestellte Schnittstelle  
- Kommunikation mit anderen Komponenten läuft indirekt über Proxys

**Beispiel:**  
- EJB-Container (mächtig, komplex)
- Spring Framework (leichtgewichtig, effizienter)

Was ist Proxy? Unter den Proxys verbogen 

