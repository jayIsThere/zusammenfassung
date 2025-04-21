+++
title = 'Vorlesung 3: Abgrenzung Festnetz/Cloud zum Mobilnetz'
date = 2025-04-15T18:22:16+02:00
categories = ['MCC']
tags = []
draft = false
+++

### 🔧 Messgeräte
- Spektrumanalysator: Zeigt Frequenzspektrum eines Signals.  
- Oszilloskop: Zeigt Zeitverlauf eines Signals.  

---------------------------------------

### 📈 Messgrößen & Vergleich zu Audio

|Funktechnik|Audiotechnik|
|------|---|
| Leistung       | Lautstärke     |
| Mittenfrequenz | Tonhöhe        |

### ⚡ Leistungsmessung
- Einheit: Watt (W), oft Milliwatt (mW)
- 1 W = 1000 mW

---------------------------------------

### 📊 Dynamik & logarithmische Darstellung

- Große Unterschiede: z.B. 20W ↔ 0.00000000003mW → Verhältnis = 666.7 Billionen
- Lösung: **logarithmischer Maßstab** mit **Bel** und **Dezibel (dB)**
  - 1 Bel = 10 dB
  - Beispiel: 20W = **43 dBm**

---------------------------------------

### 🔢 Berechnung: dBm

- Formel:

$$P_\mathrm{dBm} = 10 \cdot \log_{10} \left( \frac{P_\mathrm{mW}}{1~\mathrm{mW}} \right)$$

- Umrechnung dBW → dBm:

$$P_\mathrm{dBm} = P_\mathrm{dBW} + 30$$

---------------------------------------

### ⚠️ Vorsicht bei dB-Rechnungen

- dB, dBm, dBW sind **Pseudoeinheiten**
  - Beispiel:
  - 13 dBW + 30 = 43 dBm → mathematisch korrekt, aber nur im Kontext

---------------------------------------

### 📺 Oszilloskop

- Darstellung: **Zeitbereich**
- Zeigt z.B. Cosinusschwingung → Amplitude, Periodendauer

---------------------------------------

### 🌈 Spektrumanalyse

- Frequenzbereich: Darstellung der Frequenzen & Leistungen
- Gerät misst Leistung **innerhalb der RBW** um eine Mittenfrequenz

Wichtige Begriffe:
- **RBW (Resolution Bandwidth)**: Breite des analysierten Frequenzfensters
- **Center Frequency**, **Span**, **Start/Stop Frequenz**

---------------------------------------

### 📉 Darstellung auf dem Spektrumanalysator

- x-Achse: Frequenz
- y-Achse: Leistung (meist in dBm)
- Reine Sinusschwingung → Eine Linie im Spektrum
- Linien erscheinen wegen Filter-Eigenschaften als „Glocken“

---------------------------------------

### 👻 Geisterleistung

- Filter lassen auch Nachbarfrequenzen leicht durch → scheinbare Leistung
- Dämpfung abhängig von Filterabstand
- Genaue Anzeige nur bei Mittenfrequenz

---------------------------------------

### 🎛️ Einfluss von RBW

- **Kleinere RBW** → feinere Auflösung, längere Messzeit
  - Beispiel: RBW 300 kHz vs. 30 kHz → „schärfere“ Glocke im Spektrum

---------------------------------------

### 🔁 Zeit- vs. Frequenzbereich

- Zeitbereich: z.B. Cosinusschwingung
- Frequenzbereich: zeigt Frequenzanteile (Spektrum)

---------------------------------------

### 📡 Hochfrequenz & Modulation

- Basisbandinformationen müssen auf hohe Trägerfrequenzen gebracht werden
- Erfolgt mittels **Mischer**

