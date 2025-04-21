+++
title = 'Vorlesung 2: Konzeptionierung von Apps'
date = 2025-04-09T18:30:37+02:00
categories = ['MAD']
tags = []
draft = false
+++

### 🧠 Konzeptentwicklung – Von der Idee zur App

#### 🎯 Zweck & Ziele

|**Aspekt**|**Beschreibung**|
|------|---|
|**Ziel der App**|Was soll die App leisten?|
|**Beispiel**|Eine Fitness-App, die Nutzern hilft, ihre täglichen Schritte zu tracken.|

#### 👥 Zielgruppe

|**Frage**|**Erklärung**|
|------|---|
|**Wer nutzt die App?**|Demografische Merkmale, technisches Niveau, Lebensstil usw.|
|**Beispiel**|Berufspendler, die ihre Fitness im Alltag verbessern wollen|

#### 🌟 Mehrwert / USP

|**Frage**|**Erklärung**|
|------|---|
|**Was unterscheidet die App?**|Wodurch hebt sie sich von bestehenden Lösungen ab?|
|**Beispiel**|Individuelle Fitnesspläne basierend auf täglichem Bewegungslevel|

#### 📈 Marktanalyse

|**Thema**|**Beschreibung**|
|------|---|
|**Konkurrenzanalyse**|Welche Stärken/Schwächen haben z. B. Fitbit, Apple Health, Google Fit?|
|**Alleinstellungsmerkmal**|Definition von Funktionen, die die App einzigartig machen|

#### 🚀 Feature Definition – MVP

|**Begriff**|**Bedeutung**|
|------|---|
|**Minimum Viable Product**|Fokus auf die **wichtigsten Funktionen** zum Start|
|**Beispiel**|**Schrittzähler** + einfache Anzeige des Fortschritts|

#### ⚙️ Technische Rahmenbedingungen

|**Aspekt**|**Beispiel**|
|------|---|
|**Konkurrenzanalyse**|iOS & Android|
|**Alleinstellungsmerkmal**|Swift (iOS), Kotlin (Android), evtl. Flutter|

#### 🎨 App-Design – UI/UX

|**Was wird gestaltet?**|**Beispiel**|
|------|---|
|**Wireframes**|Layout der Screens|
|**Navigation**|Intuitive Benutzerführung|
|**UI-Konzepte**|Klare Buttons, gut strukturierte Navigation|

---------------------------------------

### 👤 Menschzentrierte Gestaltung (ISO 9241-210)

#### 🔍 Nutzungskontext analysieren (PACT)

|**Dimension**|**Fragen**|
|------|---|
|**People**|Wer nutzt die App?|
|**Activities**|Was wollen Nutzer mit der App machen?|
|**Context**|Wann und wo wird die App genutzt?|
|**Technology**|Welche Geräte oder Plattformen werden verwendet?|

📌 **Beispiel**: App soll auch offline funktionieren, da nicht immer Internetzugang besteht.

#### 📋 Anforderungen aus Nutzung ableiten

|**Aspekt**|**Beispiel**|
|------|---|
|**Nutzungsanforderung**|Schrittzählung auch ohne GPS, um Akku zu sparen|

#### ✏️ Gestaltungslösungen entwerfen (Prototyping)

|**Aktivität**|**Beispiel**|
|------|---|
|**Erste Lösungen entwerfen**|Einfacher Klick-Prototyp mit z. B. Figma oder Balsamiq|

#### 🔄 Nutzerbeteiligung bei Evaluierung

|**Methode**|**Beispiel**|
|------|---|
|**Feedback sammeln**|Beta-Tests, Usability-Tests|
|**Iteration**|Prototypen verbessern durch wiederholte Nutzer-Tests|

---------------------------------------

### 👤 Personas

|**Begriff**|**Erklärung**|
|------|---|
|**Fiktive Nutzermodelle**|Typische Nutzer mit Eigenschaften, Bedürfnissen, Zielen|
|**Beispiel**|“Betty, 37 Jahre, Lagerleiterin, technikunsicher, gestresster Alltag”|

🎯 **Ziel**: Design mit Empathie – Entwicklung orientiert sich an echten Bedürfnissen

---------------------------------------

### 📘 Szenarien & Use Cases
#### 🧾 Szenarien

|**Was?**|**Beispiel**|
|------|---|
|**Narrativ (Ist/Soll)**|“Betty möchte nach der Arbeit ihre Schritte sehen.”|

#### 📄 Use Cases

|**Element**|**Beispiel**|
|------|---|
|**Akteur**|Betty|
|**Ziel**|Schritte zählen & Fitnessziel setzen|
|**Ablauf**|App öffnen → Schrittanzahl sehen → Ziel setzen|
|**Alternativen**|Fitnessziel anpassen|
|**Vor-/Nachbedingungen**|App ist geöffnet; Schrittzähler ist aktiv|

---------------------------------------

### 📋 Anforderungen
#### ✅ Funktionale Anforderungen

|**Typ**|**Beispiel**|
|------|---|
|**Funktion**|Login, GPS-Nutzung, Schrittzähler, Benachrichtigungen|

#### ✅ ⚙️ Nicht-funktionale Anforderungen

|**Typ**|**Beispiel**|
|------|---|
|**Performance**|App lädt unter 2 Sekunden|
|**Datenschutz**|DSGVO-konform, keine Weitergabe persönlicher Daten|
|**Kompatibilität**|Kompatibel mit Android 11+ & iOS 15+|

---------------------------------------

### 🧭 Kano-Modell

|**Kategorie**|**Bedeutung & Beispiel**|
|------|---|
|**Basisfaktoren**|Selbstverständlich (z. B. Schrittzähler)|
|**Leistungsfaktoren**|Mehr ist besser (z. B. Fitnessanalysen, Statistikfunktionen)|
|**Begeisterungsfaktoren**|Unerwartet, aber erfreulich (z. B. Motivationsnachrichten mit KI)|

---------------------------------------

### 🧪 Prototyping

#### 🎯 Ziel
**Ideen sichtbar & testbar** machen, bevor Entwicklung beginnt.

#### 📦 Arten von Prototypen

|**Typ**|**Beschreibung**|
|------|---|
|**Low-Fidelity**|Skizzen, Papiermodelle, Wireframes (z. B. mit Figma/Balsamiq)|
|**High-Fidelity**|Realitätsnah, interaktiv, visuell ausgereift|
|**Evolutionär**|Prototyp wächst mit Feedback & Anforderungen (agil)|

#### ⚖️ Tiefe vs. Breite

|**Form**|**Beschreibung**|
|------|---|
|**Horizontaler Prototyp**|Viele Funktionen angedeutet, keine Tiefe|
|**Vertikaler Prototyp**|Wenige Funktionen, dafür komplett durchdacht|
|**Durchstich-Prototyp**|Ein kompletter Pfad als Machbarkeitsnachweis|

#### 🎞️ Weitere Formen
- **Storyboard**: Nutzung wie in einem Comic visualisiert
- **Index Cards**: Jede App-Seite als Karte dargestellt
- **Wireframes**: Layout der Seiten ohne Design

#### 🧪 Testmethoden

|**Methode**|**Ziel**|
|------|---|
|**Nutzerbeobachtung**|Nutzer bei Bedienung beobachten (z. B. Usability-Test)|
|**Feedbackrunden**|Iterativ Meinungen & Verbesserungsvorschläge einholen|
|**Iteration**|Prototyp mehrfach anpassen & verbessern|

