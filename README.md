# Torsion Link FEM Analysis – Landing Gear Simulation

This project presents a Finite Element Method (FEM) analysis of a **torsion link** component in a typical aircraft **landing gear system**. The primary objective is to investigate the structural performance of the torsion link under defined force loads and boundary constraints using **Altair HyperWorks**, across **multiple material configurations**.

## 📌 Objective

- Simulate the torsional and stress responses of a landing gear torsion link using FEM.
- Evaluate different material choices to observe how each behaves under the same loading conditions.
- Compare results to guide material selection for optimal structural performance.

## 🧪 Methodology

- **Tool Used:** Altair HyperWorks (HyperMesh + OptiStruct/Solver)
- **Geometry:** Torsion link from a landing gear (modeled or imported CAD).
- **Loads & Constraints:** Applied realistic force and constraint conditions relevant to a landing scenario.
- **Materials Tested:** Simulated with multiple materials (e.g., Aluminum alloys, Titanium alloys, Composites, etc.) with accurate elastic and yield properties.

### Steps Taken:

1. Meshed the torsion link using suitable 1D/2D/3D elements depending on geometry.
2. Applied consistent load and boundary conditions for all material tests.
3. Defined different material models and re-ran the solver for each.
4. Recorded key metrics: von Mises stress, displacement, strain energy, safety factor.
5. Visualized and compared results.

## 📊 Results

Results are stored in the `/results` folder, including:

- Stress and displacement contour plots (images)
- Result summaries (tables and plots)
- Comparative charts of material performance

## ⚙️ Optimization & Material Selection

In this experiment, manual comparison was done between different material outputs. However, **Altair HyperWorks does provide tools for material optimization**, including:

### ✅ Tools You Can Use for Optimization:

1. **OptiStruct’s Topology and Size Optimization:**
   - You can define design variables (e.g., material type, thickness) and constraints (e.g., weight, max stress).
   - Define objective functions like minimizing compliance or weight.
   - Use `MAT1`, `MAT2`, etc. to toggle material properties in iterations.

2. **Altair Material Data Center:**
   - Contains a library of material properties that you can integrate directly into your FEM simulations.

3. **Multi-Material Optimization (MMO):**
   - Advanced technique to let solver suggest material layouts for best performance.
   - Needs license extension for some features.

If you're aiming to find the most optimized material for a given set of loading conditions, it's recommended to use **response optimization** or define a **DOE (Design of Experiments)** setup within HyperStudy.

---

## 📁 Repository Structure

