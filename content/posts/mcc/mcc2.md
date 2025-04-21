+++
title = 'Vorlesung 2: Was ist Bit? & Übung'
date = 2025-04-08T18:22:14+02:00
categories = ['MCC']
tags = []
draft = false
+++

### Informationen und Informationsgehalt

Der **Informationsgehalt** beschreibt, wie viel „Überraschung“ oder „Neuigkeit“ in einem Ereignis steckt – je unwahrscheinlicher ein Ereignis, desto mehr Information trägt es.

**Formel zur Berechnung:**

  > I(p) = −log₂(p)

- **p** ist die Wahrscheinlichkeit des Ereignisses  
- Ein **sicheres Ereignis** (p = 1) hat **keinen Informationsgehalt**  
- Ein **zufälliges Ereignis** (p = 0,5) liefert **1 Bit Information**  
- Ein **seltenes Ereignis** (z.B. Lottogewinn mit p = 0,0000001) liefert **~26,57 Bit**

---------------------------------------

### Beispiel 1: Münzwurf

- Wahrscheinlichkeit: **p = 0,5**
- Informationsgehalt:  
  > I(0,5) = −log₂(0,5) = **1 Bit**

Ein häufiger, aber unvorhersehbarer Ausgang → *relativ wenig Überraschung*

---------------------------------------

### Beispiel 2: Lotto-Gewinn

- Wahrscheinlichkeit: **p = 0,0000001**
- Informationsgehalt:  
  > I(0,0000001) = −log₂(0,0000001) ≈ **26,57 Bit**

Ein extrem seltenes Ereignis → *hohe Überraschung, viel Information*

---------------------------------------

### Zusammenfassung

- Wahrscheinlichkeit ↓ → Informationsgehalt ↑  
- Bei **p = 1**: keine neue Info  
- Bei **p ≪ 1**: viel neue Info

📌 *Bedeutung für: Informatik, Kommunikation, Datenkompression, Verschlüsselung, Codierung*

---------------------------------------

### Beispiel: Informationsgehalt eines Bildes

**Gegeben:**
- Bildgröße: **1024 × 1024 Pixel** (= 1.048.576 Pixel)
- Nur **1 schwarzes Pixel**, Rest ist weiß

**Berechnung:**

- Position (welches Pixel ist schwarz?):  
  > log₂(1.048.576) ≈ **20 Bit**
- Farbinformation: **irrelevant**, da nur ein Pixel abweicht
- **Gesamtinformationsgehalt ≈ 20 Bit**

📌 *Nur die Position des schwarzen Pixels zählt → geringe Information*

---------------------------------------

### Fazit

- Informationsgehalt ist eng verknüpft mit **Unwahrscheinlichkeit**
- Ein einfach scheinendes Bild kann sehr wenig Information tragen, auch wenn es groß ist

