+++
title = 'Vorlesung 1: Einführung in Mobile and Cloud Computing'
date = 2025-04-01T18:22:11+02:00
categories = ['MCC']
tags = []
draft = false
+++

### 🌐 Abgrenzung Festnetz / Mobilnetz / Cloud

|**Netzwerkart**|**Merkmale**|
|------|---|
|**Festnetz**|- Geräte sind **ortsgebunden** und **verkabelt** (z. B. Desktop-PC, Drucker)|
||- Stabil und hohe Bandbreite, aber nicht mobil|
|**Mobilnetz**|- Geräte sind **mobil**, Verbindung über **Funk** (z. B. LTE, WLAN)|
||- Kombiniert feste und mobile Komponenten (z. B. Basisstation + Smartphone)|
|**Cloud**|- Nutzt meist Festnetz, bietet aber **zusätzliche Dienste**:|
||• Rechenleistung (z. B. AWS EC2)|
||• Speicherung (z. B. Google Drive)|
||• Virtualisierung (z. B. virtuelle Maschinen)|
||- **Cloud = mehr als nur Transportnetz**|

---------------------------------------

### 📡 Funkverbindung & Frequenz

|**Konzept**|**Beschreibung**|
|------|---|
|**Frequenz**|z. B. **WLAN bei 2412 MHz**, definiert die Trägerfrequenz des Signals|
|**Bandbreite**|z. B. **20 MHz**, bestimmt die Übertragungsrate (je breiter, desto schneller)|
|**Sender/Empfänger**|Transmitter & Receiver – meist mit **Antennen** ausgestattet|
|**Reichweite**|Abhängig von Leistung, Hindernissen, Frequenz|
|**Funkzellen**|Einteilung des Versorgungsgebiets – Wechsel bei Bewegung → **Handover**|

📌 **Beispiel**: Dein Handy bleibt im Zug mit dem Internet verbunden, weil es automatisch die Funkzellen wechselt.

---------------------------------------

### 🔐 Sicherheitsrisiken bei Funkverbindungen

|**Risiko**|**Erklärung**|
|------|---|
|**Signal-Abgriff über Distanz**|Mit Richtantennen kann man Funksignale über größere Strecken abhören|
|**→ Reichweite ≠ Sicherheit!**|Funkwellen machen Netzwerke **besonders anfällig** für Lauschangriffe|
|**Sicherheitsmaßnahmen nötig**|z. B. Verschlüsselung, Zugangskontrolle, Authentifizierung|

---------------------------------------

### 🔄 Transceiver & Kommunikationsmodi

|**Typ**|**Erklärung & Beispiel**|
|------|---|
|**Transceiver**|Geräte, die **sowohl senden als auch empfangen** (z. B. Smartphone, WLAN-Modul)|
|**Halbduplex**|Wechselweise Kommunikation (z. B. Walkie-Talkie)|
|**Vollduplex**|Gleichzeitiges Senden und Empfangen (z. B. Telefon, WhatsApp-Call)|

---------------------------------------

### 📶 Konfiguration mobiler Netzwerke

|**Typ**|**Beschreibung**|
|------|---|
|**Ad-hoc Netzwerke**|Direkte Verbindung ohne zentrale Steuerung (z. B. Bluetooth zwischen Laptops)|
|**Mit zentraler Einheit**|Access Point koordiniert Kommunikation (z. B. WLAN zu Hause)|
|**Netzbetreiber-Netzwerke**|Großflächig & organisiert (z. B. Telekom LTE-Netz)|

