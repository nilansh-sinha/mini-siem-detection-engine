# Full-Stack Detection Engineering Platform (Mini SIEM)

A production-style detection engineering simulation that ingests logs, normalizes events, applies logic-based detection rules, and visualizes alerts. Inspired by enterprise SEIMs (Splunk, Sentinel, Elastic).

## 🚀 Features
- **Log Ingestion & Normalization**: Converts raw Auth/Web logs into a standard schema (ECS-like).
- **Detection-as-Code**: YAML-based rules with MITRE mapping and false positive handling.
- **Correlation Engine**: Stateful detection logic (e.g., Brute Force -> Successful Login).
- **Red Team Simulation**: Scripts to generate realistic attack telemetry.
- **Dashboard**: Simple visualization of alerts and severity.

## 🏗 Architecture
See [ARCHITECTURE.md](ARCHITECTURE.md) for detailed design.

## 🛠 Setup & Usage
1. **Install Dependencies**:
   ```bash
   pip install pyyaml
   ```
2. **Run Attack Simulation**:
   ```bash
   python red_team/brute_force.py
   ```
3. **Run Detection Engine**:
   ```bash
   python engine/main.py
   ```
4. **View Dashboard**:
   Open `dashboard/index.html` in your browser.

## 🛡 MITRE ATT&CK Coverage
See [MITRE_MAPPING.md](MITRE_MAPPING.md).

## ⚠️ Disclaimer
This project is an educational detection-engineering simulation. The "attacks" are simulated locally and do not target external systems.
