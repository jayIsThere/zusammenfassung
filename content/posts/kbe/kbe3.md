+++
title = 'Vorlesung 3: komponentenbasiertes Software-Engineering'
date = 2025-04-17T18:13:15+02:00
categories = ['KBE']
tags = ['komponente', 'schnittstelle']
draft = false
+++

### 🧩 Grundprinzipien der KBSE

- **Unabhängige Komponenten**
 – Austauschbar, Schnittstellen-basiert

- **Komponentenstandards**
 – Einheitliche Schnittstellendefinition

- **Middleware-Unterstützung**
 – Kommunikation, Ressourcen, Sicherheit

- **Wiederverwendung im Prozess**
 – Schon bei Planung und Entwicklung

---------------------------------------

### ⚠️ Herausforderungen im KBSE

|**Thema**|**Problemstellung**|
|------|---|
|**Vertrauenswürdigkeit**|Blackbox-Komponenten erschweren Verständnis|
|**Komponentenzertifizierung**|Wer haftet bei Fehlern? Rechtlich unklar|
|**Emergente Eigenschaften**|Unvorhersehbares Verhalten bei Integration|
|**Anforderungskompromisse**|Passende Komponente ≠ perfekte Erfüllung aller Anforderungen|

---------------------------------------

### 🎯 Zentrale Entwurfsprinzipien

- **Unabhängigkeit** der Komponenten
- **Stabile, klar definierte Schnittstellen**
- **Standardisierte Infrastruktur** mit Basisdiensten

---------------------------------------

### 🧩 Komponenten als Dienstanbieter

- Kapseln Funktionalität → Zugriff nur über Schnittstelle
- **Lokalisation & Sprache irrelevant**

|**Vorteil**|**Erklärung**|
|------|---|
|**Unabhängigkeit**|Austauschbar ohne Einfluss auf andere Komponenten|
|**Schnittstellenbasiert**|Kein interner Zugriff nötig|

---------------------------------------

### 🔍 Komponenten vs. Objekte

| **Merkmal**                | **Komponente**                     | **Objekt**                          |
|------------------------|--------------------------------|---------------------------------|
| **Deployment**          | Direkt ausführbar | Bestandteil eines Programms |
| **Typdefinition**       | Instanz mit eigener Struktur               | Objekt auf Basis einer Klasse     |
| **Transparenz**         | Blackbox, nur API sichtbar   | Intern oft sichtbar               |
| **Sprachabhängigkeit**  | Sprachunabhängig (.NET, WSDL)               | Sprachgebunden (z. B. Java) |
| **Standardisierung**    | Muss Modell folgen  | Frei definierbar                |

---------------------------------------

### 🧩 Komponentenschnittstellen

|**Schnittstellentyp**|**Beschreibung**|
|------|---|
|**Provided Interface**|API der Komponente: was sie bietet|
|**Required Interface**|Externe Dienste, die die Komponente benötigt|

---------------------------------------

### 📐 UML-Notation für Komponenten

🧱 **Komponente**  
- Rechteck mit zwei kleinen Rechtecken (≙ Stecker & Buchse)
- Darstellung der:
    - Realisierungsklassen
    - Provided/Required-Interfaces

---------------------------------------

### 💡 Schnittstellenspezifikation in Komponentenmodellen

|**Modell**|**Beschreibungssprache**|
|------|---|
|**SOAP Webservices**|API der Komponente: was sie bietet|
|**Java CDI**|Annotationen & Interfaces|
|**.NET Framework**|CIL (Common Intermediate Language)|

**Beispiele für Schnittstellen-Nutzung**: URI, JNDI (z. B. in Java EE)

---------------------------------------

### 🧩 Grundelemente eines Komponentenmodells

| **Element**              | **Beschreibung**                                                        |
|----------------------|---------------------------------------------------------------------|
| **Schnittstellen**    | Bereitgestellte & benötigte Dienste – definieren, **was** eine Komponente kann/braucht|
| **Nutzung**           | Verwendung globaler Bezeichner wie **URI**, **JNDI** zur Identifikation und Verknüpfung           |
| **Bereitstellung & Verpackung** | Konfigurationsoptionen, Dokumentation, Metadaten – z. B. als **JAR** oder **DLL**           |
| **Komposition**       | Wie Komponenten **zusammengesetzt** und integriert werden                               |
| **Anpassung**         | Konfigurierbarkeit für unterschiedliche Einsatzszenarien                         |
| **Evolution**         | Regeln für Austausch, **Versionskontrolle** und Updates                                          |
| **Dokumentation & Namenskonvention** | Einheitliche Strukturen für bessere **Übersicht & Wartung**                      |

---------------------------------------

### ⚙️ Bereitstellung & Anpassung

- Komponenten liefern Infrastruktur mit
- Konfigurierbar über Parameter
- Beispiel: **Maven** – **.jar** + Doku + Metadaten

---------------------------------------

### 🛠️ Middleware-Dienste im Komponentenmodell

**Plattformdienste**
- Kommunikation
- Ressourcen- & Transaktionsverwaltung
- Sicherheit, Nebenläufigkeit, Persistenz

**Hilfsdienste**
- Z. B. Authentifizierung, Logging
- Entlasten Entwickler, verhindern Inkompatibilitäten

---------------------------------------

### 🧃 Container als Laufzeitumgebung

|**Aspekt**|**Beschreibung**|
|------|---|
|**Container**|Bereitstellung der Middleware-Dienste|
|**Beispiel**|**EJB-Container** (komplex), **Spring Framework** (leichtgewichtig)|
|**Proxy-Prinzip**|Kommunikation erfolgt **indirekt** – über Vermittlerobjekte ("Proxy")|

🔎 **Was ist ein Proxy?**
→ Ein Proxy ist eine Stellvertreter-Komponente, die Anfragen entgegennimmt und an die eigentliche Komponente weiterleitet – z. B. für Logging, Security oder Transparenz.


