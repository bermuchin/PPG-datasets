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
| **Task** | Heart Rate Estimation, Motion Artifact Removal, Signal Quality Assessment |
| **Subjects** | 24 healthy volunteers |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Environment** | Laboratory (Rest + Walking + Running) |
| **Motion Artifact** | High |
| **Sensor Location** | Wrist |
| **Signals** | PPG, ECG, Accelerometer, Gyroscope |
| **Sampling Rate** | PPG: 50 Hz, ECG: 125 Hz, ACC/Gyro: 50 Hz |
| **Ground Truth** | ECG available |

## BAMI-2

| 항목 | 내용 |
|------|------|
| **Task** | Heart Rate Estimation, Motion Artifact Removal, Signal Quality Assessment |
| **Subjects** | 23 healthy volunteers |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Environment** | Laboratory (Rest + Walking + Running + Running while holding treadmill bar + Walking while holding treadmill bar) |
| **Motion Artifact** | High |
| **Sensor Location** | Wrist |
| **Signals** | PPG, ECG, Accelerometer, Gyroscope |
| **Sampling Rate** | PPG: 50 Hz, ECG: 125 Hz, ACC/Gyro: 50 Hz |
| **Ground Truth** | ECG available |

## BIDMC

| 항목 | 내용 |
|------|------|
| **Task** | Respiratory Rate Estimation, Heart Rate Estimation |
| **Subjects** | 53 ICU patients |
| **Rhythm** | Mixed **(AF not explicitly annotated)** |
| **Environment** | Intensive Care Unit (ICU) |
| **Motion Artifact** | Low |
| **Sensor Location** | Finger |
| **Signals** | PPG, ECG, Impedance Respiration |
| **Sampling Rate** | PPG: 125 Hz, ECG: 125 Hz, Respiration: 125 Hz |
| **Ground Truth** | ECG available |



## 통합 비교표
| Dataset | AF | ECG | Motion | Peak Detection |
|---------|:--:|:---:|:------:|:--------------:|
| BAMI-1 | ✗ | ✓ | ✓ | ✓ |
| BIDMC | ✗ | ✓ | ✗ | ✓ |
| MIMIC-Perform | ✓ | ✓ | ✗ | ✓ |
| PulseDB-MIMIC | ✓ | ✓ | ✗ | ✓ |
