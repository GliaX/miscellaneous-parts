# 3D-Printed Infusion Pump (PG-801D) Drive Gear Replacement


> [!WARNING]
> **WARNING: DO NOT USE THIS PART YET**
> This model is currently in testing and refinement. It is NOT ready for clinical or deployment use.

## 1. Project Overview
This open-source medical hardware project addresses a critical clinical bottleneck: the downtime of **PG-801D Infusion Pumps** due to the premature wear and mechanical failure of the primary drive gear. 

An infusion pump is a life-critical medical device that delivers fluids, nutrients, or medications (such as chemotherapy, hormones, or antibiotics) into a patient’s body in controlled amounts. In resource-constrained clinical settings—such as hospitals in Gaza—the wear and tear of minor plastic gears often renders these expensive machines entirely inoperable, as replacement parts are difficult to source locally.

### The Problem
* **Frequent Component Wear:** The original injection-molded plastic gear suffers from tooth erosion over extended periods of continuous operation.
* **Low Tolerance for Error:** Even a minor slippage on these teeth results in precise sensor warnings (such as flow error/blockage alarms), triggering an immediate machine shutdown to ensure patient safety.
* **Widespread Downtime:** Dozens of infusion pumps are currently out of service in local medical facilities solely due to this single faulty component.

### The Solution
By FreeCAD and Fused Deposition Modeling (FDM) 3D printing with (ABS), we developed an exact physical replica of the primary drive gear. This repository provides the trial design file, print file(STL,3MF), media and user manual.

# 2. Device & Component Information
* **Target Device:** Infusion Pump PG-801D (Syringe/Volumetric Driver)
* **Part Function:** Primary drive gear for the main rotary drivetrain.
* **Mechanical Role:** Transfers continuous rotational torque directly from the main electric stepper motor to the lead screw (threaded drive shaft). As the gear rotates, it drives the lead screw, which translates rotational force into linear motion to push the syringe plunger at precise, micro-controlled flow rates.
* **Failure Mechanism:** Constant mechanical stress and frictional fatigue lead to tooth thinning and rounding. Any minor play or loss of motion transmission stops the lead screw, triggering immediate sensor faults on the device.

## 3. Engineering Process
To ensure the printed part functions identically to the manufacturer's original specification, the following engineering workflow was executed:

1. **Dimensional Analysis & Metrology:** Detailed caliper and micrometer measurements of the original (worn) gear were taken to define pitch circle diameter, outer diameter, tooth profile, shaft bore size, and keyway features.
2. **Parametric CAD Modeling (FreeCAD):** 
   * Formulated the exact gear module and tooth count within FreeCAD.
   * Modulated the core mounting hub to house the original locking brass screw insert.
   * Exported the final parametric model into standard interchange formats (`.FCStd`, `.stl`).
3. **Slicing and Flow Analysis:** Used PrusaSlicer to set up optimal layer bonding and wall strength, packaging the finalized print settings into a portable `.3mf` file.

---

## 4. Manufacturing Specifications


 Material Selection
* **Recommended Filament:** **ABS or PETG **
* **Why ABS?** ABS provides high impact resistance, dimensional stability under continuous torque.
* **Why PETG?** PETG offers excellent layer adhesion, high toughness, and ease of printing with low thermal shrinkage.


<h1 align="center" style="color:red;">⚠️ WARNING: DO NOT USE THIS PART YET ⚠️</h1>
<h3 align="center" style="color:red;">This model is currently in testing and refinement. It is NOT ready for clinical or deployment use.</h3>

### Recommended Slicer Settings ABS
| Parameter | Value | Details |
| :--- | :--- | :--- |
| **Nozzle Temperature** | **250°C** | High temperature ensures optimal inter-layer adhesion to prevent tooth shearing under torque. |
| **Bed Temperature** | **105°C** | Essential to prevent ABS warping on the print bed. |
| **Infill Percentage** | **100% (Solid)** | Solid infill is mandatory to maximize mechanical shear resistance of the gear teeth. |
| **Layer high**| **0.2** | Provides an optimal outer boundary definition. |
| **Support Material** | **Yes / Enabled** | Required to cleanly support the central overhanging mounting hub and gear face profile. |
| **Enclosure** | **Recommended** | An enclosed printer chamber is highly recommended to control ambient temperatures and eliminate ABS warping. |

### Recommended Slicer Settings PETG
| Parameter | Value | Details |
| :--- | :--- | :--- |
| **Nozzle Temperature** | **230°C** | 
| **Bed Temperature** | **85°C** | 
| **Infill Percentage** | **100% (Solid)** | Solid infill is mandatory to maximize mechanical shear resistance of the gear teeth. |
| **Layer high**| **0.2** | Provides an optimal outer boundary definition. |
| **Support Material** | **Yes / Enabled** | Required to cleanly support the central overhanging mounting hub and gear face profile. |



## 5. Validation & Functional Testing
Before deploying the manufactured gear into a clinical environment, each printed unit undergoes a strict multi-tier quality control protocol:
For details about tests, see the [Testing Protocol](Quality_control/README.md).


```
[3D Print Completed] 
       │
       ▼
 1. Visual Inspection  ───► Check tooth profiles for stringing, warping, or defects

       │
       ▼
 2. Hub & Thread Test  ───► Insert the locking brass screw to verify smooth, clean rotation
       │
       ▼
 3. Benchtop Testing   ───► Install inside PG-801D and run non-clinical tests (water-pumping)
       │
       ▼
[Clinical Approval]

```

## Medical & Safety Disclaimer

This design is provided "as is" for educational, experimental, and humanitarian evaluation only. The author accepts no responsibility or liability for any direct, indirect, incidental, or consequential damages, injuries, or device failures resulting from the manufacture, testing, or clinical use of this design. Use and deployment are entirely at the user's own risk.

---
## License
This design is shared under the [CERN Open Hardware Licence Version 2 - Permissive (CERN-OHL-P)](LICENSE.md).see the LICENSE file for details.
