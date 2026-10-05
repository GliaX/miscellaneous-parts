# 3D-Printed FUJI CR/Type C Cassette Slider Replacement (P/N 124536)

⚠️ **WARNING: THIS MODEL IS CURRENTLY IN CLINICAL TESTING AND ACTIVE REFINEMENT.**

## 1. Project Overview
This open-source medical hardware project addresses a critical clinical maintenance bottleneck: the mechanical failure and breakage of the plastic slider closure devices (**OEM Part Number: 124536**) utilized in **FUJI Fujifilm Type CR and Type C X-ray cassettes**.

An X-ray computed radiography (CR) cassette protects and houses the internal photostimulable phosphor imaging plate during clinical exposures. The slider closure device consists of two mirrored parts on either side of the cassette boundaries that mechanically slide to lock and seal the housing securely.

### The Problem
* **Frequent Component Breakage:** The original OEM plastic clips degrade and snap over extended periods of heavy clinical workflow.
* **Catastrophic Reader Risks:** If a damaged or compromised cassette clasp is inserted into an automated CR reader, structural fragments can snap off inside the reader slots. This causes immediate jamming of internal transport tracks, mechanical system shutdown, and severe secondary damage to the high-cost diagnostic optics.
* **Clinical Downtime:** Due to severe supply chain disruptions and blockade constraints in Gaza, sourcing official OEM spare parts locally is nearly impossible, rendering critical diagnostic imaging cassettes entirely inoperable.

### The Solution
Through reverse-engineering, parametric CAD modification, and Fused Deposition Modeling (FDM) 3D printing, we optimized an exact functional physical replica of the P/N 124536 closure device to safely restore functional X-ray cassettes to clinical service.

---

## 2. Device & Component Information
* **Target Device:** FUJI Fujifilm Type CR and Type C Medical Imaging Cassettes.
* **Part Function:** Slider closure and locking clasp device (Mirrored set).
* **Mechanical Role:** Slides horizontally along the cassette framework to engage internal locking lips, ensuring the internal imaging plate remains light-sealed and structurally fixed during handling.
* **Failure Mechanism:** Constant impact, mechanical friction, and cyclical stress lead to structural stress-whitening and fracturing around the high-stress neck area of the clip.

---

## 3. Engineering & Material Design Evolution

The development of this component followed a structured, iterative engineering process to eliminate premature structural failure and streamline the manufacturing workflow.

### 🔴 Baseline Inheritance (Version 1)
* **Initial Status:** The project optimization began by inheriting an existing baseline CAD design file.
* **Reference Source File:** **`Cassette_Clip_Nasser_ScrewHoleLength_right`** (located within the `Design_Files` directory).
* **Clinical Outcome:** This baseline model was originally printed in **PETG** and field-tested under continuous diagnostic load at Nasser Hospital, where it suffered catastrophic fracturing after **2 weeks** of usage.
* **Identified Failures:** High sliding surface friction, material rigidity stress, and critical geometric deviations from the OEM part.

### 🟡 Advanced Engineering Optimizations (Version 2 - Current)
Taking over from the baseline failure, a comprehensive engineering review was conducted. Three critical geometric modifications were introduced within the CAD architecture to mirror the OEM part's performance:

1. **Interface Profile Matching (Friction Interface):** The geometric contact point where the clip interacts directly with the cassette frame was heavily modified to match the original OEM specifications. Because this area experiences continuous friction during everyday clinical use, precise alignment here is vital to extend the component's operational lifespan.
2. **Alignment Button Enlargement (Front Dial):** The diameter of the front circular button—which the CR reader mechanism physically pushes—was enlarged to match the original dimensions. The baseline design featured a smaller diameter, which caused axial misalignment during automatic loading cycles.
3. **Spring Housing Expansion (Internal Clearance):** The internal bore cavity for the spring housing was enlarged to reduce excessive compression during operation, preventing premature spring fatigue and ensuring smooth mechanical travel.

### 🔬 Material Optimization & Shrinkage Calibration (PETG to ABS)
* **The PETG Challenge:** Prototyping in PETG required intensive manual post-print processing, sanding, and filing (بردخة يدوية) to achieve smooth sliding movement. This introduced individual human error into the production line, causing severe geometric inconsistencies between parts and ruining batch replication.
* **The ABS Solution:** Switching to **ABS** yielded highly uniform, smooth sliding surfaces directly off the print bed, completely eliminating the need for manual post-processing error.
* **Printer Shrinkage Compensation:** To counter the high thermal contraction rate characteristic of ABS, the CAD file dimensions were precisely calibrated and expanded according to the specific metrics of the deployment 3D printer, successfully reaching exact OEM dimensions.

---

## 4. Validation & Clinical Testing History

### Revision History (Nasser Hospital - Gaza)
* **Version 1 (V1 - PETG Design Baseline):** Fractured after **2 weeks** due to stress concentration at the neck and high surface friction.
* **Version 2 (V2 - ABS Calibrated Design):** Handed over to the biomedical engineer at Nasser Hospital on **September 3, 2026**, with active clinical deployment starting on **September 4, 2026**. 
* **Current Status:** A total of **4 operational pairs (8 individual pieces)** were manufactured and deployed for active validation. **All 4 pairs remain fully functional and have operated flawlessly without a single mechanical fault or degradation for over a month under heavy clinical use.**

### Multi-Tier Quality Control Flowchart
```text
[3D Print Completed]
│
▼
1. Visual Inspection ───► Check structural geometry for ABS warping or splitting.
│
▼
2. Mechanical Bench ───► Install onto multiple functional FUJI CR cassettes to check fit.
│
▼
3. Cycle Slot Test ───► Cycle cassette into every physical slot of the operational CR reader.
│
▼
[Active Field Testing]
```
