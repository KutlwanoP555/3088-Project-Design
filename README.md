****Reposotory for a power subsystem****

Group 127 
EEE3088F Design principals



# ⚡ Micro-Mouse Power Subsystem

This repository documents the design of a  **Power Subsystem** for the Micro-Mouse (MM) project. The power subsystem is responsible for delivering regulated power to all components of the micro-mouse.
---

## 📋 System Requirements

To meet the course requirements, the power subsystem must achieve the following:

- ✅ **Drive up to 4 motors bidirectionally**, using the assigned pins.
  - 2x brushed DC motors (200 mA each)
  - 2x auxiliary motors (500 mA each)
- ✅ **Integrate an INA219** for battery monitoring via I²C.
  - A0 and A1 pins must not both be tied to GND.
- ✅ **Charge the battery from a 9V input source.**
- ✅ **Support two charging modes**:
  - Low current: 200 mA
  - High current: 600 mA ±100 mA (from the battery's perspective)
- ✅ **Integrate USB-C** and negotiate a **9V supply** from a USB host.
- ✅ **Provide 2x external load switches**:
  - Must support 1 A each, with high-side connection to 5V.
- ✅ **Provide regulated 3.3V and 5V outputs**:
  - 3.3V @ 300 mA max ±5% accuracy
  - 5V @ 1.5 A max ±5% accuracy
- ✅ **Include an ON/OFF switch**:
  - OFF: Leakage current < 30 μA
  - ON: Must deliver up to 2 A peak current
  - Must shut down both 5V and 3.3V rails

---
