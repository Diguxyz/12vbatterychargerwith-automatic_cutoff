# 🔋 12V Battery Charger with Automatic Cut-off

## 📘 Project Overview
This project presents the design and simulation of a *12V Battery Charger* with an *Automatic Cut-off* feature.  
The charger converts AC mains voltage to a regulated DC output using a *bridge rectifier* and *voltage regulators* (7805, 7812, and LM317).  
The *LM317* controls the charging voltage and current, while a *relay module* automatically disconnects the battery when it reaches full charge, ensuring safe and efficient operation.

---

## ⚙ Circuit Description
- *AC Source:* Main input power supply (230V AC).
- *Transformer:* Steps down the voltage to 15–18V AC.
- *Bridge Rectifier:* Converts AC to DC using 1N5408 diodes.
- *Filter Capacitors:* Smooth the DC voltage.
- *Voltage Regulators:*  
  - *7805* – Provides regulated 5V output.  
  - *7812* – Provides regulated 12V output for the charger circuit.  
- *LM317:* Controls charging voltage and current, configured as an adjustable regulator.  
- *Relay Module:* Automatically cuts off charging when the battery is fully charged.

---

## 🧩 Components Used
| Component | Description |
|------------|-------------|
| Transformer | 230V to 15–18V AC, 1A |
| Bridge Rectifier | 4 × 1N5408 diodes |
| Capacitor | 4700µF / 35V filter capacitor |
| LM317 | Adjustable voltage regulator |
| 7805, 7812 | Fixed voltage regulators for stable DC |
| Relay Module | 12V DC relay for auto cut-off |
| Battery | 12V Lead-acid (7–20Ah) |
| Misc. | Resistors, diodes, PCB, wires, fuse |

---

## 🧠 Working Principle
1. AC voltage is stepped down by the transformer and converted to DC by the bridge rectifier.  
2. The output is filtered using capacitors and then regulated by 7812 and LM317.  
3. LM317 adjusts the charging voltage/current supplied to the battery.  
4. When the battery voltage reaches the preset threshold, the relay disconnects the charger to prevent overcharging.  
5. The circuit also provides an additional 5V output for powering low-voltage devices.

---

## 🧪 Simulation (eSIM)
In *eSIM*, the project was simulated step-by-step.  
However, due to limited component availability:
- The *relay module* and *LM317* were not available for simulation.  
- Only the *transformer, rectifier, and voltage regulators* were implemented.  
As a result, a *pure 12V DC output* was successfully obtained, and a *5V output* was also added for testing.

---

## 🚧 Problems Faced
- Transformer parameters in eSIM needed fine adjustment.  
- LM317 and relay components were not available in the eSIM library.  
- Limited simulation support for automatic cut-off feature.

---

## 🧰 Future Improvements
- Implement complete hardware prototype with LM317 and relay.  
- Add LED indicators for charging and full-charge status.  
- Integrate microcontroller-based voltage sensing for accuracy.  
- Test under load with real 12V battery and measure charge performance.

---

## 📄 License
This project is released under the *GNU General Public License (GPL v3)*.  
You are free to use, modify, and distribute it with proper attribution.

---

## ✍ Author
*Sujal Savarkar*  
Instrumentation Engineering Student  
Project: 12V Battery Charger with Automatic Cut-off  
Simulation: eSIM

---
