# 🚀 Modeling, Analysis, and Fabrication of Solid Rocket Motor

<div align="center">

![SRM Header](srm_diagram.png)

**Bachelor of Technology — Aerospace Engineering**  
*Sandip University Nashik | Department of Aero Engineering | AY 2022–2023*

[![License](https://img.shields.io/badge/license-Academic-blue.svg)](LICENSE)
[![University](https://img.shields.io/badge/university-Sandip%20University-orange.svg)](https://sandipuniversity.edu.in)
[![Domain](https://img.shields.io/badge/domain-Aerospace%20Engineering-navy.svg)]()
[![Tools](https://img.shields.io/badge/tools-SolidWorks%20%7C%20ANSYS%20%7C%20OpenMotor-red.svg)]()

</div>

---

## 👥 Team

| Name | PRN |
|------|-----|
| Sanket Bansode | 190101051007 |
| Vaishnavi Sogalad | 190101051020 |
| Mitali Jadhav | 190101051028 |
| Pranay Malewar | 190101051030 |
| Utkarsh Ninawe | 190101051045 |

**Supervisor:** Dr. Ravi Krishna Swami Garigipati (Assistant Professor)  
**HOD:** Prof. Dr. Vishal N Sulakhe

---

## 📋 Abstract

This project presents the full design lifecycle of a **Solid Rocket Motor (SRM)** — from conceptual design and propellant formulation through CAD modeling, fabrication, and aerodynamic analysis. The motor uses **KNSU (Potassium Nitrate / Sucrose)** as propellant at an oxidizer-to-fuel ratio of **65:35**, with a convergent-divergent (CD) nozzle designed in **SolidWorks** and analyzed using **ANSYS Fluent** (1500 iterations). Simulation via **OpenMotor** software determined an expected thrust of **600–700 N**.

---

## 🎥 Demo Video

> *Watch the solid rocket motor propellant burn test and assembly demonstration*

📹 **[▶ View Demo Video](assets/video/srm_demo.mp4)**

The video showcases the propellant preparation (KNSU caramelization process), motor assembly, and test results.

---

## 📁 Repository Structure

```
solid-rocket-motor/
├── README.md
├── srm_diagram.png               # SRM overview diagram
├── grain_geometries.png          # Propellant grain types
├── tubular_grain_type.png        # Selected grain design
│
├── cad/                          # SolidWorks CAD Models & Drawings
│   ├── cad_3d_casing_model.png   # 3D casing model
│   ├── cad_3d_nozzle_model.png   # 3D nozzle model
│   ├── cad_assembly_view.png     # Full SRM assembly
│   ├── cad_section_view.png      # Section view assembly
│   ├── casing_2d_drawing.png     # 2D engineering drawing — casing
│   ├── nozzle_2d_drawing.png     # 2D engineering drawing — nozzle
│   └── nozzle_cross_section.png  # CD nozzle profile diagram
│
├── fabrication/                  # Physical Manufacturing
│   ├── fabricated_casing.png     # Machined MS casing
│   ├── fabricated_nozzle.png     # Lathe-machined nozzle
│   ├── srm_full_assembly.png     # Final assembled SRM
│   ├── cylindrical_casing.png    # Casing component
│   ├── nozzle_flange_front.png   # Nozzle-flange front view
│   └── nozzle_flange_top.png     # Nozzle-flange top view
│
├── propellant/                   # Propellant Materials & Preparation
│   ├── potassium_nitrate.png     # KNO₃ oxidizer
│   ├── sucrose_granular.png      # Sucrose fuel
│   └── liquified_knsu_mix.png   # Melted KNSU mixture
│
├── cfd/                          # CFD Analysis Results (ANSYS)
│   └── cfd_results.png           # Pressure & velocity contours
│
├── assets/
│   ├── video/srm_demo.mp4        # Demo recording
│   └── cropped/                  # Source page crops from report
│
└── docs/
    └── FINAL_BLACK_BOOK_2023.pdf # Complete project report
```

---

## 🛠️ Tools & Software

| Tool | Version | Purpose |
|------|---------|---------|
| **SolidWorks** | 2021 | 3D CAD modeling, 2D drafting, assembly |
| **ANSYS Fluent** | 2021 R2 | CFD analysis — pressure & velocity contours |
| **OpenMotor** | Open-source | Grain simulation, thrust/pressure prediction |
| **Meteor** | Open-source | Cross-validation of motor parameters |

---

## 🔩 CAD Design (SolidWorks)

All components were designed using **SolidWorks 2021** with a bottom-up modeling approach.

### 3D CAD Models

<div align="center">

| Casing Model | Nozzle Model |
|:---:|:---:|
| ![Casing 3D](cad/cad_3d_casing_model.png) | ![Nozzle 3D](cad/cad_3d_nozzle_model.png) |

</div>

### Assembly Views

<div align="center">

| Full Assembly | Section View |
|:---:|:---:|
| ![Assembly](cad/cad_assembly_view.png) | ![Section View](cad/cad_section_view.png) |

</div>

### Engineering Drawings (2D Drafting)

<div align="center">

| Motor Casing Drawing | Nozzle Drawing |
|:---:|:---:|
| ![Casing 2D](cad/casing_2d_drawing.png) | ![Nozzle 2D](cad/nozzle_2d_drawing.png) |

</div>

### CD Nozzle Cross-Section

<div align="center">
<img src="cad/nozzle_cross_section.png" width="60%" alt="Nozzle cross section"/>
</div>

The **Convergent-Divergent (De Laval) nozzle** features:
- Convergent section (45° half-angle)
- Throat diameter: 6 mm
- Divergent section (15° half-angle)
- Total nozzle length: 92.88 mm
- Flange OD: 128 mm with 8× M6 bolt holes at 88 mm PCD

---

## ⚙️ Fabrication

All components were fabricated from **Mild Steel (MS)** using a **lathe machine** for the nozzle and standard pipe + TIG welding for the casing. Total material weighed approximately **14.85 kg**.

### Manufactured Components

<div align="center">

| Fabricated Casing | Fabricated Nozzle |
|:---:|:---:|
| ![Casing](fabrication/fabricated_casing.png) | ![Nozzle](fabrication/fabricated_nozzle.png) |

| Casing Component | Nozzle-Flange |
|:---:|:---:|
| ![Cylindrical Casing](fabrication/cylindrical_casing.png) | ![Flange](fabrication/nozzle_flange_front.png) |

</div>

### Final Assembled SRM

<div align="center">
<img src="fabrication/srm_full_assembly.png" width="55%" alt="Full SRM Assembly"/>
</div>

### Motor Casing Dimensions

| Parameter | Value |
|-----------|-------|
| Outer Diameter (OD) | 128 mm |
| Inner Diameter (ID) | 88 mm (GI pipe) |
| Length | 250 mm |
| Flange PCD | 88 mm |
| Bolt size | M6 × 8 bolts |
| Material | Mild Steel (IS 2062) |

### Material Properties — Mild Steel

| Property | Value |
|----------|-------|
| Density | 7.8 g/cm³ |
| Carbon content | 0.05% – 0.25% |
| Tensile strength | ~400 MPa |
| Weldability | Excellent |
| Machining | Easy (Lathe) |

**Fabrication process:**
1. Nozzle machined on lathe (3–4 days)
2. Outer flange fabricated separately
3. TIG welding of nozzle + flange
4. GI pipe used for casing (ID = 85 mm)
5. Flanges TIG-welded to both ends
6. Bolt holes drilled at 45° pattern

---

## 🔥 Propellant — KNSU

**KNSU (Potassium Nitrate / Sucrose)** was chosen for its safety, availability, and moderate specific impulse.

### Propellant Materials

<div align="center">

| Potassium Nitrate (KNO₃) | Sucrose | Liquified KNSU Mix |
|:---:|:---:|:---:|
| ![KNO3](propellant/potassium_nitrate.png) | ![Sucrose](propellant/sucrose_granular.png) | ![Liquified](propellant/liquified_knsu_mix.png) |

</div>

### Formulation

| Parameter | Value |
|-----------|-------|
| Propellant | KNSU (Potassium Nitrate + Sucrose) |
| Oxidizer (KNO₃) | 65% |
| Fuel (Sucrose / C₁₂H₂₂O₁₁) | 35% |
| Binder | None required (KNO₃ acts as binder) |
| Surfactant | 0.1% (SLS — reduces surface tension) |
| Mixing temperature | 160–250°C |
| Cure time | 2–4 hours |

### Preparation Process

1. Measure KNO₃ (65 parts) and sucrose (35 parts) by weight
2. Mix dry ingredients until homogeneous
3. Heat on electric induction at 250°F (≈121°C) until molasses-like consistency
4. Add 0.1% surfactant to extend pour time
5. Pour into casting tube (PVC mold)
6. Insert Teflon coring rod to form tubular grain
7. Cure for 2–4 hours; remove coring tool

> ⚠️ **Safety Note:** KNSU is highly flammable. Handle only in open, ventilated areas with appropriate PPE. Never heat beyond 250°C to prevent caramelization loss.

---

## 🌀 Grain Geometry

### Types of Grain Geometries

<div align="center">
<img src="grain_geometries.png" width="80%" alt="Grain geometry types"/>
</div>

### Selected: Tubular Grain

<div align="center">
<img src="tubular_grain_type.png" width="50%" alt="Tubular grain"/>
</div>

The **tubular (internal burning cylindrical) grain** was selected because it:
- Provides a **neutral burn** profile (constant thrust over time)
- Has high volumetric efficiency
- Is easy to cast and core
- Offers structural stability during combustion

---

## 📊 CFD Analysis (ANSYS Fluent)

The CD nozzle was analyzed using **ANSYS Fluent 2021 R2** with 1500 iterations.

### Mesh & Boundary Conditions
- **Mesh type:** Unstructured mesh with sizing
- **Turbulence model:** k-ω SST
- **Inlet:** Pressure inlet (combustion chamber pressure)
- **Outlet:** Pressure outlet (atmospheric)
- **Iterations:** 1500

### CFD Results

<div align="center">
<img src="cfd/cfd_results.png" width="80%" alt="CFD Results"/>
</div>

Key findings:
- Supersonic flow achieved in the divergent section
- Pressure drops from chamber to exit as expected
- Velocity increases through the throat to supersonic values
- Minor turbulence observed at ~70% nozzle length near divergent wall

---

## 📈 Performance Parameters (OpenMotor)

| Parameter | Value |
|-----------|-------|
| Expected Thrust | **600–700 N** |
| Propellant | KNSU |
| O/F Ratio | 65/35 |
| Grain type | Tubular (circular core) |
| Nozzle type | Convergent-Divergent |

Cross-validation was performed using **Meteor** simulation software.

---

## 📚 References

1. Foltran et al., "Burning Rate Measurement of KNSu Propellant Obtained by Mechanical Press," *Journal of Aerospace Technology and Management*, May 2015
2. Mohammed Iliyaas et al., "Computational Analysis of CD Nozzle for Solid Propellant Rocket," Anna University, Aug 2016
3. Nevin Nelson et al., "Stress Analysis of Solid Rocket Motor Case," Bishop Jerome Institute, Mar 2020
4. Hartfield et al., "A Review of Analytical Methods for Solid Rocket Motor Grain Analysis," Auburn University, Jun 2012
5. P.G. Sutton & O. Biblarz, *Rocket Propulsion Elements*, John Wiley & Sons, 2001
6. Shaik Muzib, "Design and Analysis of Solid Propellant Rocket Nozzle and its Applications to RCS," Vol. 9, Oct 2019

---

## 🏫 Institution

**Sandip University Nashik**  
School of Engineering and Technology  
Department of Aero Engineering  
AY 2022–2023

---

<div align="center">
<sub>Final Year Capstone Project — B.Tech Aerospace Engineering</sub>
</div>
