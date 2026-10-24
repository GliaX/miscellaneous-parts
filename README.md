# Open-Source 3D-Printed Medical Replacement Components

This repository serves as a centralized, open-source registry for 3D-printed medical device replacement components. It is designed to assist biomedical engineers and clinical technicians in sourcing, manufacturing, and validating critical spare parts for medical equipment—especially in resource-constrained environments or crisis zones where supply chains are disrupted.

Every component listed in this repository represents a localized engineering solution aimed at reducing clinical downtime and restoring life-saving diagnostic and therapeutic machinery to active service.

## 📂 Repository Structure
The repository is organized into independent, self-contained project directories.

```
.
├── 📁 infusion-pump-gear/             # Project 1: Syringe Pump Drivetrain Replacement
│   ├── 📁 design-files/              # FreeCAD (.FCStd)
│   ├── 📁 print-files/               # Production-ready .stl
│   ├── 📁 docs-and-manuals/          # Equipment user/service manuals (PG-801D)
│   ├── 📁 media/                     # Inspection photographs and deployment videos
│   └── 📄 README.md                  # In-depth technical guide & validation workflow
│
├── 📁 Cassette_Clip_Slicer/           # Project 2: FUJI CR Cassette Slider Replacement
│   ├── 📁 Design_Files/               # CAD source files
│   ├── 📁 Print_Files/                # Production-ready .stl / .gcode
│   ├── 📁 Manual/                     # Equipment user/service manuals (FUJI CR Systems)
│   ├── 📁 Media/                      # Failure analysis and deployment photographs
│   └── 📄 README.md                   # Clinical testing history & risk mitigation protocol
│
└── 📄 README.md                      # This root registry overview documentation
```

## 🛠️ Featured Registry Projects

### 1. Infusion Pump Drivetrain Replacement
* **Description:** Engineering solution for syringe pump drivetrain components to reduce clinical downtime.
* **Documentation:** See the [infusion-pump-gear README](./infusion-pump-gear/README.md) for replication details.

### 2. FUJI CR Cassette Slider Replacement (P/N 124536)
* **Description:** A 3D-printed replica of the slider closure device used in FUJI Fujifilm Type CR and Type C X-ray cassettes to ensure secure locking and prevent critical reader damage.
* **Documentation:** See the [Cassette_Clip_Slicer README](./Cassette_Clip_Slicer/README.md) for validation history and safety protocols.
