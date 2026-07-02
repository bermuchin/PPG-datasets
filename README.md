# PPG Datasets

A curated collection of publicly available photoplethysmography (PPG) datasets for physiological signal processing research.

This repository summarizes each dataset from a research perspective, including:

- Subjects
- Sensor location
- Available signals (PPG, ECG, ACC, etc.)
- Sampling rate
- Recording environment
- Rhythm information (e.g., AF)
- Motion artifacts
- Potential research tasks (Peak Detection, HR, BP, AF, etc.)

## BAMI-1

| 항목 | 내용 |
|------|------|
| **목적 (Task)** | Heart Rate Estimation, Motion Artifact Removal, Signal Quality Assessment |
| **Subjects** | 24 healthy volunteers |
| **Rhythm** | Normal Sinus Rhythm (NSR) only (AF ✗) |
| **Environment** | Laboratory (Rest + Walking + Running) |
| **Motion Artifact** | High |
| **Sensor Location** | Wrist |
| **Signals** | PPG, ECG, Accelerometer, Gyroscope |
| **Sampling Rate** | PPG: 50 Hz, ECG: 125 Hz, ACC/Gyro: 50 Hz |
| **Ground Truth** | ECG available (R-peak 기반 label 생성 가능) |
| **우리 연구 활용도** | Motion robustness 검증에는 적합, AF Peak Detection에는 제한적 |
