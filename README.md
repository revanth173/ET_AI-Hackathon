# Sentinel Industrial Safety Intelligence Platform

An automated, real-time safety monitoring dashboard designed for industrial plant control rooms. The platform correlates IoT gas telemetry with digital Work Permit Systems (WPS) to detect hidden **compound hazards**—preventing workplace accidents, explosions, and regulatory non-compliance before they occur.

---

## 📌 Problem Context

In large industrial facilities (such as steel plants, chemical units, and refineries), safety monitoring systems often operate in isolated silos:
* **Gas Detection Systems (SCADA/IoT):** Trigger alarms only when gas concentrations cross absolute safety thresholds (e.g., Methane > 25 ppm).
* **Work Permit Systems (WPS):** Track active maintenance tasks (e.g., Hot Work / Welding permits) digitally.

### The Silent Danger: Compound Hazards
A gas reading of 18 ppm might be classified as "SAFE" by an isolated gas detector. However, if an active welding permit is simultaneously approved in the exact same zone, the combination of flammable gas and an open flame creates an immediate, critical explosion hazard.

---

## 🚀 Key Features

* **Real-Time SCADA/IoT Simulation:** Dynamic telemetry tracking for gas levels (Methane, Carbon Monoxide) across plant zones.
* **Multi-Agent Risk Correlation Engine:** Correlates active work permits with physical gas sensor readings to automatically detect compound risks in real time.
* **Automated Permit Revocation:** Automatically revokes active permits (e.g., Hot Work Permit #402) when a compound hazard is detected.
* **Emergency Alert System:** Instant on-screen modal dispatching emergency notifications configured for plant safety officers (`saipachipala8@gmail.com` and `+91 8184946886`).
* **Regulatory Compliance Audit Logging:** Auto-generates structured audit trails compliant with **OISD-STD-105** (Work Permit Systems) and **Factory Act Section 41** (Hazardous Processes).

---

## 🛠️ Tech Stack & Architecture

| Component | Technology / Library | Role in Project |
| :--- | :--- | :--- |
| **Frontend UI** | HTML5, Tailwind CSS | Responsive dashboard layout, control panels, and clean corporate theme |
| **Core Logic** | JavaScript (ES6+) | Live SCADA simulation, compound risk correlation logic, state management |
| **Icons** | Lucide React / Feather Icons | Visual status indicators, warning badges, and zone markers |
| **API Integration** | EmailJS / Fetch API (Mocked) | Emergency email and SMS alert notification handling |

---

## 🏢 Real-World Safety Compliance Standards

This platform enforces two core regulatory standards applicable to industrial manufacturing:

1. **OISD-STD-105 (Oil Industry Safety Directorate):** Standard governing Work Permit Systems in hazardous petroleum and gas environments (§7.1 Methane Thresholds, §7.3 Hot Work Safety Distances).
2. **Factory Act Section 41 (Section 41-B & 41-C):** Indian Labour Code statutory regulations for hazardous process safety management, compulsory disclosure of hazards, and worker safety controls.

---

## 📂 Project Structure

```text
├── index.html          # Main application dashboard containing UI, logic, and telemetry
├── README.md           # Project documentation
