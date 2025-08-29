# Live-cell Imaging of IEC Monolayer Infections

This repository contains the analysis script for live-cell imaging experiments on IEC monolayers.

---

## Experimental Setup

Live-cell imaging was performed on a **custom-built upright microscope**, based on the *Thorlabs Cerna upright microscopy system* (Thorlabs Inc., Newton, NJ, USA), equipped with:

- **Objective**: Heated 60/1.0 NA Nikon CFI APO NIR objective (2.8 mm WD)
- **Condenser**: Nikon d-CUO DIC oil condenser (1.4 NA)
- **Camera**: ORCA-Fusion (C14440-20UP; Hamamatsu Photonics, Hamamatsu City, Japan)
- **Pixel size**: 109 nm
- **Light source**: 530 nm Thorlabs LED (M530L3), to minimize phototoxicity and chromatic aberrations
- **Control software**: Micro-Manager 2.0[^1]

The imaging chamber was maintained at **37 °C** with moisturized **5% CO₂ air** and an objective heater.

---

## Sample Preparation

- IEC monolayers were grown within AICs.
- Samples were placed in **35 mm glass-bottom dishes** (Cellvis) in **3 ml DMEM/F12 without antibiotics**.
- Samples were equilibrated for 30 min in the microscope light path before infection.

---

## Infection and Imaging

- **Inoculum**: *Salmonella enterica* serovar Typhimurium (S.Tm).
- Added to the apical compartment directly under the objective.
- Imaging started immediately with:
  - **20 ms exposure time**
  - **15 sec frame rate**
  - Differential interference contrast (DIC) imaging

---

## Data Analysis

- Time-lapse movies were analyzed manually using **Trackmate for ImageJ**[^2].
- Events tracked manually:
  - Bacterial attachment
  - Division
  - Invasion
  - Detachment
- Track data exported and dendrogram plots generated with **custom R scripts** using:
  - `data.tree`
  - `dendextend`
  - `stats`

---

## License

GPL-3.0
