# Predictive Maintenance - Microsoft Azure Dataset

A comprehensive dataset for predictive maintenance modeling, featuring time-series telemetry data, error logs, maintenance records, and failure data from 100 machines collected throughout 2015.

**Dataset Source:** [Kaggle - Microsoft Azure Predictive Maintenance](https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance)

---

## 📋 Table of Contents

- [Dataset Overview](#dataset-overview)
- [Files Included](#files-included)
- [Data Categories](#data-categories)
- [File Details](#file-details)

---

## Dataset Overview

This dataset was originally part of the Azure AI Notebooks for Microsoft Predictive Maintenance. It contains 5 CSV files with different aspects of machine operating data, making it ideal for:
- Building predictive maintenance models
- Time-series analysis
- Component failure prediction
- Maintenance optimization

---

## 📁 Files Included

| File Name | Description |
|-----------|-------------|
| `PdM_telemetry.csv` | Hourly sensor readings (voltage, rotation, pressure, vibration) |
| `PdM_errors.csv` | Non-critical errors encountered during operation |
| `PdM_maint.csv` | Maintenance and component replacement records |
| `PdM_failures.csv` | Component failures and replacements |
| `PdM_Machines.csv` | Machine metadata (model type, age) |

---

## 📊 Data Categories

### Machine Conditions and Usage
Operating conditions of machines with data collected from sensors (e.g., voltage, vibration, pressure).

### Failure History
Historical record of machine and component failures within machines.

### Maintenance History
Repair history including error codes, previous maintenance activities, and component replacements.

### Machine Features
Metadata about machines including engine size, make, model, and location.

---

## 🔍 File Details

### Telemetry Time Series Data (`PdM_telemetry.csv`)
Contains hourly averages of:
- Voltage
- Rotation
- Pressure
- Vibration

**Coverage:** 100 machines throughout 2015

### Error Data (`PdM_errors.csv`)
Records non-critical errors encountered during machine operation. These errors do not shut down the machines and are therefore not classified as failures. Timestamps are rounded to the nearest hour to align with telemetry data collection frequency.

### Maintenance Records (`PdM_maint.csv`)
Captures component replacements under two scenarios:
1. **Proactive Maintenance:** Regular scheduled replacements by technicians
2. **Reactive Maintenance:** Unscheduled replacements due to component failure

**Coverage:** Records from 2014 and 2015 with hourly-rounded timestamps.

### Failure Data (`PdM_failures.csv`)
Represents component replacements due to failure. This is a subset of the maintenance data with hourly-rounded timestamps aligned to telemetry collection frequency.

### Machine Metadata (`PdM_Machines.csv`)
Contains machine characteristics including:
- Model type
- Age/manufacture year