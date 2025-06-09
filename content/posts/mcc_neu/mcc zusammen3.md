+++
title = 'Radio Access Stand'
date = 2025-04-15T18:22:16+02:00
categories = ['MCC new']
tags = []
draft = false
+++

### 1. 디지털 변조란?

- 정보를 전송하기 위해 아날로그 전파(사인파)의 특성을 **디지털 신호(0과 1)**에 맞게 바꾸는 것.

- 변조 시 바꿀 수 있는 세 가지:
  - 진폭 (Amplitude)
  - 주파수 (Frequenz)
  - 위상 (Phase)

---------------------------------------

### 2. Symbol과 Symbolrate (기초 개념)

- Symbol: 한 번에 전송하는 "신호 단위", 꼭 1비트일 필요 없음

- Symbolrate (R<sub>s</sub>)	: 초당 전송되는 심볼 수 (Symbole/s)

- Bitrate (R<sub>b</sub>): 초당 전송되는 비트 수 (bit/s) = Symbolrate × (bit/심볼 수)

  - 예: QPSK는 1개 심볼로 2비트를 전송하므로 R<sub>b</sub> = 2 × R<sub>s</sub>

---------------------------------------

### 3. Modulationsarten (변조 방식 종류)

- BPSK
  - 1 비트 심볼
  - 위상만 0° / 180°
  
- QPSK	
  - 2 비트 심볼
  - 위상: 0° / 90° / 180° / 270°
  
- 8-PSK	
  - 3 비트 심볼
  - 위상: 8가지
  
- 16-QAM	
  - 4 비트 심볼
  - 위상 + 진폭 조합 (4×4=16상태)
  
- 64-QAM
  - 6 비트 심볼
  - 8×8=64 상태
  
→ 더 많은 비트를 전송할수록 복잡하지만 효율↑
→ 오류에 약해짐!

---------------------------------------

### 4. Bandbreitenbedarf (대역폭 필요량)

- 얼마나 넓은 주파수 범위를 차지하느냐?
- Symbolrate가 높을수록 빠른 전송

- 기본 규칙:
  - Basisband (기저대역): 필요한 대역폭 = ½ × Symbolrate
  - Hochfrequenz (고주파대역): 대역폭 = Symbolrate

- 예시:
  - Symbolrate = 2 Sym/s →
  - Basisband 필요 대역폭: 1 Hz
  - HF 대역 필요 대역폭: 2 Hz

---------------------------------------

### 5. Bandbreiteneffizienz (스펙트럼 효율)


  <img src="/zusammenfassung/images/mcc8.jpg" style="display: block; margin: auto;"> 
  
- 스펙트럼 효율이 높을수록 더 많은 데이터를 좁은 공간에 전송 가능
- 단, 신호 품질(SNR)이 중요함!

---------------------------------------

### 6. Informationsgehalt pro Symbol

심볼이 가질 수 있는 상태 수를 x라고 할 때:

  <img src="/zusammenfassung/images/mcc9.jpg" style="display: block; margin: auto;"> 
  
- 예시:
  - BPSK: 2가지 상태 → log₂(2) = 1 bit
  - QPSK: 4가지 상태 → log₂(4) = 2 bit
  - 16-QAM: 16가지 상태 → log₂(16) = 4 bit
  
---------------------------------------

### 7. Hochmischen (상향 변환)

- 기저대역 신호(Basisband)를 **고주파(Trägerfrequenz)**로 올려 보내야 전파에 실을 수 있음

  - 방식: 신호 × 사인파 → 고주파 신호 (HF)
  - 모든 주파수 성분이 트래커 주파수 중심으로 ‘복사됨’

  - 예: 0.5 Hz 성분 → 2.4000005 MHz & 2.3999995 MHz

---------------------------------------

### 8. Mehrwertige Modulation: 장점 vs 단점

- 효율 ↑ (bit/s/Hz): 오류에 민감함 (BER↑)
- 높은 데이터 전송 가능: 높은 SNR 필요 (예: 64-QAM은 매우 깨끗한 채널 필요)

  - 예: QPSK가 BPSK보다 3 dB 더 많은 SNR 필요

---------------------------------------
