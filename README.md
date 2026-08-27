# Predictive-Maintenance-System
This is a Predictive Maintenance System . It is being trained for any machine with sensor readings and a log of maintenance. Hence can be applied on most of the machines.
# Predictive Maintenance of Radar Hardware using Machine Learning

Final Year Project — College of Aeronautical Engineering (CAE), NUST Risalpur
Supervisor: Wg Cdr Fakhar Abbas | Sponsor: Directorate of Long Range Radar (LRR)

## Overview
This project applies machine learning to predict maintenance needs of radar
hardware — specifically the Power Supply Unit (PSU) and its sub-components —
before failures occur. Instead of reactive repairs or fixed inspection
schedules, the system flags at-risk components early using historical
sensor and event data.

## Approach
- **Random Forest** (primary model) and **SVM** (comparison) for fault
  classification
- Trained and validated on the Azure Predictive Maintenance dataset as a
  public proxy, since no open radar-hardware dataset exists
- Feature engineering includes rolling telemetry statistics and error-log
  trends to capture early warning signs
- Cross-validation and threshold tuning applied to improve precision
  without sacrificing recall
- A synthetic dataset (motor/fan degradation model) is used to extend
  testing to radar-specific cooling hardware
- A Flask-based dashboard provides live fault prediction, health scoring,
  and batch scoring

## Status
Baseline and improved classification models complete. Time-series /
Remaining Useful Life (RUL) forecasting (planned, using NASA C-MAPSS as
benchmark) and integration of real sponsor maintenance records are next.

## Disclaimer
Built and validated on public proxy datasets (Azure PdM, NASA C-MAPSS).
Results reflect model methodology, not confirmed performance on classified
radar hardware, pending real sponsor data.
