# 🤖 Automated Fiber Encapsulation for Fused Layer Modeling (FLM)

---

This repository contains the documentation and core files for an engineering project focused on the automated encapsulation of continuous fibers for integration into a Fused Layer Modeling (FLM) 3D printer. The goal of this project is to create mechanically stronger and lighter components by embedding reinforced, continuous carbon fibers within a 3D-printed part.

## ✨ Project Goal

---

The primary objective is to automate the process of coating carbon fiber roving with a plastic granulate, which can then be fed into an FLM 3D printer. This work systematically follows an engineering design process, from foundational research to practical implementation and testing.

## ⚙️ Core Concepts & Approach

---

The project is structured into three main phases:

* **1. Technical Foundations:** An analysis of the FLM printing process, including the structure of the extruder and hotend. This section also explores the **Markforged concept**, a key inspiration for embedding encapsulated fibers to create reinforced components.

* **2. System Requirements & Concept Evaluation:**
    * **Requirements:** Critical system requirements were defined, including reliable heating of the granulate, kink-free deflection of the fibers, and a consistent feed mechanism.
    * **Concept Development:** A functional structure analysis was performed, leading to a morphological box for potential solutions. Key decisions included selecting a **stepper motor** for its superior control in fiber feeding and opting for a **direct drive** or belt drive system for simplicity and cost-effectiveness.

* **3. Implementation & Realization:**
    * **Hardware:** A stepper motor with a planetary gear was chosen, requiring a calculated torque of M = 35 Ncm. Custom 3D-printed parts were used to connect the motor to the spool.
    * **Software:** The **Marlin firmware**, commonly used in 3D printing, was adapted and uploaded to an Arduino board. This setup controls the stepper motor, cooling fan, heating cartridges, and thermistor. The **Pronterface** user interface was used for direct command and control.

## ✅ Project Results

---

The system was successfully tested, demonstrating that the heating block can reliably reach 185 °C to melt the granulate. The stepper motor effectively pulls the carbon fibers through the melt pool, and the final die shapes the encapsulated fiber. The result is a high-quality, evenly coated fiber suitable for reinforcing FLM-printed parts.

**Key Findings:**
* A stable connection between the thermistor and the heating block is crucial for accurate temperature readings.
* The system produced consistently good quality encapsulated fibers.
* Future work could explore a larger nozzle diameter depending on the desired fiber quality.

## 🚀 Next Steps

---

The successful production of encapsulated fibers paves the way for their use in a future bachelor's thesis, which will focus on their application to create stronger FLM-printed components.
