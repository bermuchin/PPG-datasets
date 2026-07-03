# PPG Datasets

A curated collection of publicly available photoplethysmography (PPG) datasets for physiological signal processing research.

This repository summarizes each dataset from a research perspective, including:

- Task
- Subjects
- Rhythm (e.g., AF)
- Environment
- Motion artifacts
- Sensor location
- Signals
- Sampling rate
- Ground truth

## BAMI-1

| 항목 | 내용 |
|------|------|
| **Task** | Heart Rate Estimation, Motion Artifact Removal, Signal Quality Assessment |
| **# of Subjects** | 24 |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Motion Artifact** | Rest + Walking + Running |
| **Sensor Location** | Wrist |
| **Signals** | PPG, ECG, Accelerometer, Gyroscope |
| **Sampling Rate** | PPG: 50 Hz, ECG: 125 Hz, ACC/Gyro: 50 Hz |
| **Ground Truth** | ECG |

## BAMI-2

| 항목 | 내용 |
|------|------|
| **Task** | Heart Rate Estimation, Motion Artifact Removal, Signal Quality Assessment |
| **# of Subjects** | 23 |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Motion Artifact** | Rest + Walking + Running + Running while holding treadmill bar + Walking while holding treadmill bar |
| **Sensor Location** | Wrist |
| **Signals** | PPG, ECG, Accelerometer, Gyroscope |
| **Sampling Rate** | PPG: 50 Hz, ECG: 125 Hz, ACC/Gyro: 50 Hz |
| **Ground Truth** | ECG |

## BIDMC

| 항목 | 내용 |
|------|------|
| **Task** | Respiratory Rate Estimation, Heart Rate Estimation |
| **# of Subjects** | 53 |
| **Rhythm** | ICU patients - Mixed **(AF not explicitly annotated)** |
| **Motion Artifact** | Low (ICU) |
| **Sensor Location** | Finger |
| **Signals** | PPG, ECG, Impedance Respiration |
| **Sampling Rate** | PPG: 125 Hz, ECG: 125 Hz, Respiration: 125 Hz |
| **Ground Truth** | ECG |

## CIME

| 항목 | 내용 |
|------|------|
| **Task** | Motion Artifact Removal, Heart Rate Estimation, Pulse Rate Variability Estimation |
| **# of Subjects** | 48 |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Motion Artifact** | Static left hand + Controlled finger motion |
| **Sensor Location** | Fingertip |
| **Signals** | PPG, Accelerometer, Gyroscope, Reference PPG |
| **Sampling Rate** | PPG: 100 Hz (downsampled, originally 200 Hz), ACC/Gyro: 100 Hz |
| **Ground Truth** | Reference PPG |

## Dryad Nurse Dataset

| 항목 | 내용 |
|------|------|
| **Task** | Stress Detection, Physiological Monitoring |
| **# of Subjects** | 15 |
| **Rhythm** | Normal Sinus Rhythm only (AF ✗) |
| **Motion Artifact** | Nurses during work |
| **Sensor Location** | Wrist |
| **Signals** | PPG (BVP), Accelerometer, Electrodermal Activity (EDA), Skin Temperature, Heart Rate (HR), Inter-Beat Interval (IBI), Event Tags |
| **Sampling Rate** | BVP 64 Hz, ACC 32 Hz, EDA 4 Hz, HR 1 Hz, Skin Temp 4 Hz, IBI event-based |
| **Ground Truth** | BVP-derived HR/IBI |

## GalaxyPPG

| 항목 | 내용 |
|------|------|
| **Task** | Heart Rate Estimation, Heart Rate Variability Estimation, Stress Detection, Motion Artifact Analysis |
| **# of Subjects** | 24 |
| **Rhythm** | Healthy population (AF ✗) |
| **Motion Artifact** | Rest, TSST, SSST, Screen Reading, Keyboard Typing, Mobile Typing, Standing, Walking, Jogging, Running |
| **Sensor Location** | Wrist (Galaxy Watch 5, Empatica E4), Chest (Polar H10) |
| **Signals** | PPG, ECG, Accelerometer, Skin Temperature, Heart Rate (HR), Inter-Beat Interval (IBI) |
| **Sampling Rate** | Galaxy Watch: PPG 25 Hz, ACC 25 Hz, HR 1 Hz; Empatica E4: BVP 64 Hz, ACC 32 Hz, Temp 4 Hz, HR 1 Hz; Polar H10: ECG 130 Hz, ACC 200 Hz, HR 1 Hz |
| **Ground Truth** | ECG (Polar H10) |

## 통합 비교표
| Dataset | AF | ECG | Motion | Peak Detection |
|---------|:--:|:---:|:------:|:--------------:|
| BAMI-1 | ✗ | ✓ | ✓ | ✓ |
| BIDMC | ✗ | ✓ | ✗ | ✓ |
| MIMIC-Perform | ✓ | ✓ | ✗ | ✓ |
| PulseDB-MIMIC | ✓ | ✓ | ✗ | ✓ |
