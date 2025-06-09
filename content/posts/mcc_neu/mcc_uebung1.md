+++
title = 'MCC Übung 1'
date = 2025-04-08T18:23:41+02:00
categories = ['MCC Übung new']
tags = []
draft = false
+++

#### 1.1 Use Case: Video-Streaming zu Hause

**Szenario:**  
Sie streamen ein Video zu Hause, Audio über Bluetooth-Box, Bild auf dem Tablet.

**a) Topologie-Skizze:**

1. **Server (Provider X)**  
2. → **Internet**  
3. → **Router** (ortsgebunden, Heimnetzwerk)  
4. → **Tablet** (mobil, zeigt das Video über WLAN)  
5. → **Bluetooth Box** (mobil, empfängt Audio)

**b) Verbindungsarten:**

- **Festnetz:**  
  - Verbindung Server ↔ Internet ↔ Router  
  - WLAN (als Heimnetzwerk-Verbindung)

- **Funk:**  
  - Bluetooth zwischen Tablet ↔ Box

**c) Mobile vs. ortsfeste Knoten:**

- **Mobil:** Tablet, Bluetooth Box  
- **Ortsfest:** Server, Router

**d) Vermutete Funktechnologien:**

- **WLAN:** Wi-Fi (wahrscheinlich Wi-Fi 5/6)  
- **Bluetooth:** Version 4.0 oder 5.0 (für stabile Audioverbindung)


#### 1.2 Use Case: Video-Streaming an der Hochschule

**Szenario:**  
Video-Streaming im Gebäude der Westfälischen Hochschule mit Bluetooth-Box.

**a) Topologie-Skizze:**

1. **Server (Provider X)**  
2. → **Internet**  
3. → **Campus-Router (Westfälische Hochschule)**  
4. → **Tablet/Laptop (mobil, über WLAN)**  
5. → **Bluetooth Box (mobil)**

**b) Gemeinsamkeiten & Unterschiede zu 1.1**

- **Gleich:**
  - Grundstruktur identisch (Server → Router → Gerät → Audio)
  - Nutzung von WLAN & Bluetooth

- **Unterschiede:**
  - **Campus-Router** statt Heimrouter  
  - **Größere Nutzerzahl**, ggf. andere Netzqualität


#### 1.3 Use Case: Video-Streaming im Auto

**Szenario:**  
Streaming im fahrenden Auto, mit Tablet und Smartphone.

**a) Möglichkeiten für das Streaming:**

- **Smartphone als Hotspot (4G/5G)**  
- **Car Wi-Fi** (eigenes Netz des Autos)  
- **Bluetooth-Übertragung** (eher ungeeignet für Video)  
- **Auto-interne Netzwerke**

**b) Topologie für jede Option:**

- **Smartphone-Hotspot:**
  > Server → Internet → Mobilfunk → Smartphone → WLAN → Tablet

- **Car Wi-Fi:**
  > Server → Internet → Mobilfunknetz (Auto) → WLAN → Tablet

- **Direkte Verbindung:**
  > Server → Internet → Auto-Netzwerk → Tablet

**c) Gemeinsamkeiten & Unterschiede zu 1.1/1.2**

- **Gleich:**
  - Server-Quelle und Funkverbindung (Bluetooth) bleiben erhalten

- **Unterschiede:**
  - **Mobile Daten** statt WLAN  
  - **Höhere Mobilität**, aber potenziell instabiler Empfang

**d) Moderne Option im vernetzten Auto:**

- Direktes **5G-Streaming durch das Auto**  
- Kein Smartphone-Hotspot nötig  
- → *Komfortabler und stabiler bei guter Netzabdeckung*
