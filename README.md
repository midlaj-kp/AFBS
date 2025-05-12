# 🚗 Automatic Fuel Blending System

## 📌 Description

The **Automatic Fuel Blending System** is a smart, real-time IoT-based embedded solution designed to **reduce automotive emissions** and **improve fuel efficiency**. By continuously monitoring exhaust gases (CO, CO₂, HC, PM), the system calculates the required amount of additive to blend with the fuel to optimize combustion and performance. This ensures dynamic, intelligent fuel management that adapts to engine conditions while minimizing environmental impact.

---

## 🎯 Problem Addressed

India is among the top global polluters, and road transport plays a major role:
- 🔴 24% of global CO₂ emissions
- 🔴 30% of PM pollution
- 🔴 High levels of CO and HC in urban air

**Limitations in Current Additive Usage**:
- Manual mixing without any emission feedback
- Overuse or underuse of fuel additives
- Poor optimization of engine performance
- No real-time adjustment based on pollution output

### ✅ Our Solution

A **real-time embedded system** that:
- Monitors CO, CO₂, HC, PM using sensors
- Calculates required additive dose based on emission deviation
- Automatically injects additives to maintain ideal emission levels
- Uses IoT for data logging and cloud integration

---

## 🧭 Objectives

- 📉 Reduce toxic emissions dynamically
- ⛽ Improve engine efficiency and mileage
- 🧠 Automate fuel-additive blending based on sensor data
- 🌐 Enable real-time monitoring through IoT dashboards

---

## 🔍 Research Gap & Novelty

| Sr. No. | Patent ID         | Research Gap                                                           | Our Novelty                                                                 |
|--------:|-------------------|------------------------------------------------------------------------|------------------------------------------------------------------------------|
| 1       | EP0733796B1       | Octane blending with no emission feedback                              | Emissions-based intelligent fuel-additive optimization                      |
| 2       | US5163586A        | Lacks real-time gas monitoring                                         | Integrated CO, HC, PM, CO₂ sensor feedback loop                             |
| 3       | US20110233233A1   | Static blending at fuel stations, not onboard                          | Embedded on-vehicle real-time micro-blending system                         |

---

## ⚙️ System Architecture

### 🧩 Hardware Components

- **Arduino UNO** – Base microcontroller
- **ESP32** – Wi-Fi enabled module for IoT
- **MQ2, MQ9, MQ135 Sensors** – Detect CO, CH₄, NOx, CO₂
- **GP2Y1010AU0F** – Dust sensor for PM detection
- **DHT22** – Temperature and humidity sensing
- **Fuel Gauge** – Fuel level monitoring
- **L293D Motor Driver** – Controls dosing pump motors
- **DC Pumps** – Dispenses additive into fuel tank

---

## 🔁 Working Principle

1. Sensors continuously read emission values from vehicle exhaust
2. Controller compares current emission vs. target thresholds
3. If emissions exceed safe levels, Arduino triggers pump dosing system
4. Additive is blended into fuel based on pollutant type and required reduction
5. ESP32 uploads data to cloud dashboard for monitoring and logging

---

## 📊 Sample Calculation

### Emission-based Additive Dosage Formula:

| Pollutant | Current (ppm) | Target Reduction (ppm) | Additive Used               | Efficiency (K) | Required Dose (ml) |
|-----------|----------------|--------------------------|------------------------------|----------------|---------------------|
| CO        | 1800           | 500                      | HiTEC® 5000 (Fuel-borne)     | 72 ppm/ml      | 18.05               |
| HC        | 100            | 20                       | Amsoil Injector Cleaner      | 5 ppm/ml       | 16                  |
| CO₂       | 80000          | 130000                   | Amsoil Cetane Booster        | 4400 ppm/ml    | 11.36               |
| PM        | 35             | 10                       | HiTEC® 5000                  | 1.9 ppm/ml     | 13.15               |

---

## 📈 Benefits

- 🔄 **Dynamic Additive Injection**: Real-time correction, no manual input
- 🌱 **Environmental Friendly**: Actively reduces harmful emissions
- 🔧 **Better Engine Health**: Cleans deposits, reduces wear
- 📶 **IoT Cloud Logging**: Remote access to emission and fuel data
- 💰 **Cost Effective**: Improves mileage and reduces additive waste

---

## 🧠 Technical Summary

- **Programming Languages**: C/C++ (Arduino), MicroPython (ESP32)
- **Communication**: UART/I2C between sensors and controller
- **IoT**: ESP32 + Firebase / Thingspeak / Blynk
- **Actuation**: Relay or motor driver triggering peristaltic pump

---

## 🧪 Future Scope

- 🔬 Integration with vehicle OBD-II port
- 📲 Mobile app for monitoring and fuel diagnostics
- 💡 AI/ML integration for predictive blending
- 🛠️ Custom ECU firmware for factory vehicles

---

## 📝 Conclusion

The **Automatic Fuel Blending System** is a practical, embedded innovation for improving combustion, reducing environmental impact, and enhancing fuel economy. By incorporating emissions-based logic, cloud integration, and automatic control, the project bridges the gap between environmental responsibility and smart automotive engineering.

---

## 📚 References

- [Afton Chemical HiTEC® Additives](https://www.aftonchemical.com)
- [Amsoil Fuel System Products](https://www.amsoil.com)
- [MQ Sensor Datasheets – Sparkfun](https://www.sparkfun.com)
- [Sharp GP2Y1010AU0F Dust Sensor](https://www.sharpsma.com)

---


