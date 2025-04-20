+++
title = 'Vorlesung 2: Wiederverwendung von Software 2'
date = 2025-04-10T18:04:15+02:00
tags = ['Wiederverwendung', 'Framework']
categories = ['KBE']
draft = false
+++

### Wiederverwendungstechniken (laut Sommerville)

1. **Frameworks**
   - **Definition:** Ein Framework ist ein Set von Softwarekomponenten, das eine Architektur für verwandte Anwendungen bereitstellt.
   - **Beispiel:** Ein Web-Framework wie Spring MVC verwendet das Model-View-Controller-Muster.
   - **Eigenschaft:** Bietet generische Funktionalität und wird erweitert, nicht ersetzt.

2. **Inversion of Control (IoC)**
   - **Prinzip:** Die Steuerung liegt beim Framework, nicht bei der Anwendung. Die Anwendung registriert ihre Komponenten, und das Framework ruft sie bei Bedarf auf.
   - **Beispiel:** Callbacks in Web-Frameworks.

3. **Entwurfsmuster**
   - **Beispiel:** Observer, Strategy sind gängige Muster, um wiederkehrende Probleme zu lösen.

4. **Architekturmuster**
   - **Beispiel:** Microservices bieten eine systemweite Lösung für komplexe Anwendungen.

5. **ERP-Systeme**
   - **Definition:** Unternehmensweite Systeme mit konfigurierbaren Modulen.
   - **Vorteil:** Bietet Lösungen für die Verwaltung von Geschäftsdaten und Prozessen.

6. **Komponentenbasierte Entwicklung**
   - **Prinzip:** Systeme werden aus austauschbaren Komponenten aufgebaut.

7. **Modellgetriebene Entwicklung**
   - **Definition:** Software wird aus plattformunabhängigen Modellen erstellt.

8. **Serviceorientierte Systeme**
   - **Prinzip:** Nutzung verteilter Webservices (z. B. REST, SOAP) zur Kommunikation zwischen Komponenten.

9. **Softwareproduktlinien**
   - **Definition:** Produktfamilien mit einer gemeinsamen Codebasis und variablen Komponenten.


### Framework-Klassifizierung (nach Fayad & Schmidt)

- **Systeminfrastruktur-Frameworks:** Z. B. Kommunikation, GUI, Compiler
- **Middleware-Integrations-Frameworks:** Z. B. Jakarta EE, .NET für Komponentenkommunikation
- **Unternehmensanwendungs-Frameworks:** Z. B. spezialisierte Frameworks für Branchen wie Telekommunikation oder Finanzen.


### Wiederverwendung von Anwendungssystemen

- **Softwareproduktlinien:** Gemeinsamer Kern mit anpassbaren Komponenten
- **Konfigurierbare Systeme:** Über Parameter anpassbar (z. B. ERP-Systeme)
- **Integrierte Systeme:** Kombination verschiedener Anwendungen über Schnittstellen


### Vorteile und Herausforderungen

- **Vorteile:** Schnellere Bereitstellung und geringeres Entwicklungsrisiko
- **Herausforderungen:** Anpassung an Unternehmensprozesse, fehlende Expertise, Auswahl des richtigen Systems

---


