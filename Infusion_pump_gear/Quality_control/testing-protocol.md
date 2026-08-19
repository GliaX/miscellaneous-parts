# 🧪 Testing & Validation Protocol - Infusion Pump Gear (PG-801D)

This document outlines the standard operating procedures for verifying and validating the 3D-printed infusion pump drivetrain gear.

---

## 1. Visual & Dimensional Inspection (Static Phase)

- [ ] **Dimensional Tolerance:** Verify pitch and outer diameter within ±0.1 mm accuracy using calipers.
- [ ] **Tooth Surface Finish:** Inspect gear teeth faces for zero stringing, blobs, or under-extrusion artifacts.
- [ ] **Shaft Alignment Test:** Mount on the motor/pump shaft to confirm a secure, precise fit without mechanical play or slippage.
- [ ] **Manual Mesh Test:** Manually rotate in mesh with the mating gear inside the pump housing to verify smooth, continuous rotation without binding.

---

## 2. Dynamic Functional Testing (Device Phase)

Once the visual inspection is passed, install the gear into the **PG-801D Infusion Pump** unit to execute active operational testing under load.

### Required Test Equipment & Setup
* **Target Device:** PG-801D Infusion Pump Unit
* **Fluid Source:** 500 mL IV Solution Bag (Normal Saline / Water)
* **Administration Set:** Standard Infusion / IV Tubing Set
* **Output Measurement:** 500 mL Calibrated Graduated Cylinder / Measuring Vessel

### Operating Parameters
| Parameter | Target Specification |
| :--- | :--- |
| **Test Equipment** | PG-801D Infusion Pump |
| **Test Fluid** | 500 mL Normal Saline / Water|
| **Flow Rate Setting** | 100 mL/hr |
| **Target Runtime** | ~5 Hours |

### Test Procedure
1. Install the gear into the drivetrain assembly and secure housing cover.
2. Set up a calibrated measuring cylinder at the pump discharge tube.
3. Initiate the pumping cycle at **100 mL/hr** and start the timer.
4. Periodically inspect for abnormal mechanical noise, motor heat, or gear tooth wear.
5. Record total discharged volume at completion and compare against target volume.

---

## 3. Historical Test Execution Logs

| Test ID | Date | Tested By | Setup / Target | Measured Output | Flow Accuracy | Result | Notes & Observations |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **TEST-01** | 2026-07-22 | Amer | 300 mL/h (1 Hr) | 260 mL/h | 86.6% (-40 mL/h) | ⚠️ Needs improve  |  |


