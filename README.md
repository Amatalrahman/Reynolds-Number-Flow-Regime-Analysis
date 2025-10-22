# Reynolds-Number-Flow-Regime-Analysis


# 🔬 Assignment 01: Reynolds Number and Flow Regime Analysis

This project explores the fundamental principles of **fluid kinetics** by analyzing the dimensionless **Reynolds Number (Re)** and its critical role in classifying flow regimes (Laminar, Transitional, and Turbulent). The work was conducted as a group assignment for the **Biotransport (SBEG201)** course.

---

## 🎯 Project Objectives

1.  **Computational Modeling:** Develop a robust tool to calculate Re for various fluids (including biofluids like blood and CSF) and pipe geometries.
2.  **Visualization:** Generate comparative plots to visualize the profound shift in flow behavior: velocity profiles and friction factors ($f$).
3.  **Flow Regime Analysis:** Statistically analyze and visually conceptualize the differences between Laminar (orderly) and Turbulent (chaotic) flow.

---

## 🛠️ Technology Stack

| Component | Tool / Language | Purpose |
| :---: | :---: | :---: |
| **Core Analysis & Visualization** | MATLAB R2025a | Re Calculation, Velocity Profile Plotting, $f$ vs. Re Log-Log Plot, Interactive GUI, Streamline Visualization. |
| **Advanced Simulation** | OpenFOAM | Computational Fluid Dynamics (CFD) simulation of Lid-Driven Cavity Flow to model high-Re turbulent phenomena. |
| **Documentation** | LaTeX / PDF | Comprehensive academic report submission. |

---

## ✨ Key Findings & Deliverables

### 1. The Re Shift (Part 1)
The analysis confirmed that flow dynamics are determined by the $\mathbf{Viscous/Inertial}$ forces ratio. High viscosity (e.g., Honey) maintains low Re, while high velocity/diameter (e.g., Water at $V=2 \text{ m/s}$) rapidly pushes the flow into the **Turbulent** regime.

### 2. Profile Transformation (Part 2)
Visualization showed the dramatic change in velocity distribution:
* **Laminar:** Perfectly **Parabolic** profile ($\mathbf{V_{\text{max}} = 2 V_{\text{avg}}}$).
* **Turbulent:** **Flat/Blunt** profile ($\mathbf{V_{\text{max}} < 2 V_{\text{avg}}}$) due to intensive mixing.

### 3. Frictional Resistance (Part 3)
The log-log plot of $f$ vs. Re demonstrated the governing equations:
* **Laminar:** $f$ is highly sensitive to Re ($\mathbf{f \propto 1/Re}$).
* **Turbulent:** $f$ is less sensitive to Re ($\mathbf{f \propto 1/Re^{0.25}}$), as friction becomes dominated by inertial eddies.

### 4. Interactive Tool (Part 4)
A functional MATLAB GUI was created, providing instant $\text{Re}$ calculation and color-coded regime classification.

---

## 📄 Repository Structure

* `Assignment_Report.pdf`: The complete academic report (The main deliverable).
* `MATLAB_Scripts/`: Contains all `.m` files necessary for Part 1 through Part 5.
    * `part1_re_calculator.m`
    * `part2_velocity_profiles.m`
    * `part3_friction_analysis.m`
    * `part4_interactive_gui.m`
    * `part5_streamlines.m`
* `CFD_Bonus_Results/`: Simulation files and resulting images from the OpenFOAM analysis.
* `Figures/`: All generated plot images used in the report.


**Developed by:** [Your Group Member Names/IDs Here]
**Course:** SBEG201 Biotransport
