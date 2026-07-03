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
| **Environment** | Laboratory (Rest + Walking + Running) |
| **Motion Artifact** | High |
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
| **Environment** | Laboratory (Rest + Walking + Running + Running while holding treadmill bar + Walking while holding treadmill bar) |
| **Motion Artifact** | High |
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
| **Environment** | Intensive Care Unit (ICU) |
| **Motion Artifact** | Low |
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
| **Environment** | Laboratory (Static left hand + Controlled finger motion) |
| **Motion Artifact** | High |
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
| **Environment** | Daily clinical environment (Nurses during work) |
| **Motion Artifact** | High |
| **Sensor Location** | Wrist |
| **Signals** | PPG (BVP), Accelerometer, Electrodermal Activity (EDA), Skin Temperature, Heart Rate (HR), Inter-Beat Interval (IBI), Event Tags |
| **Sampling Rate** | BVP 64 Hz, ACC 32 Hz, EDA 4 Hz, HR 1 Hz, Skin Temp 4 Hz, IBI event-based |
| **Ground Truth** | BVP-derived HR/IBI |

## GalaxyPPG

| 항목 | 내용 |
|------|------|
| **Task** | Stress Detection, Physiological Monitoring |
| **Subjects** | 36 healthy volunteers |
| **Rhythm** | Healthy population (AF ✗) |
| **Environment** | Laboratory (Stress-inducing protocols: TSST and SSST) |
| **Motion Artifact** | Moderate |
| **Sensor Location** | Wrist (Galaxy Watch, Empatica E4), Chest (Polar H10) |
| **Signals** | PPG, ECG, Accelerometer, Skin Temperature, Heart Rate (HR), Inter-Beat Interval (IBI) |
| **Sampling Rate** | Galaxy Watch PPG: 25 Hz, Galaxy Watch ACC: 25 Hz, 
\n E4 BVP: 64 Hz, E4 ACC: 32 Hz, 
\n Polar H10 ECG: 130 Hz, Polar H10 ACC: 200 Hz |
| **Ground Truth** | ECG (Polar H10) |

## 통합 비교표
| Dataset | AF | ECG | Motion | Peak Detection |
|---------|:--:|:---:|:------:|:--------------:|
| BAMI-1 | ✗ | ✓ | ✓ | ✓ |
| BIDMC | ✗ | ✓ | ✗ | ✓ |
| MIMIC-Perform | ✓ | ✓ | ✗ | ✓ |
| PulseDB-MIMIC | ✓ | ✓ | ✗ | ✓ |
