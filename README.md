# 🧪 DFT-Based Ductility Analysis using Pugh Criterion

Understanding whether a material bends or breaks starts at the atomic scale.

This project investigates the ductility of selected FCC metals using Density Functional Theory (DFT) and the Pugh criterion (B/G ratio), combining first-principles simulations with mechanical property analysis.

---

## 🔬 Overview

The study evaluates the mechanical behavior of:

- Lithium (Li)
- Platinum (Pt)
- Yttrium (Y)
- Zirconium (Zr)
- Tellurium (Te)

using DFT simulations performed in Quantum ESPRESSO.

Ductility is predicted using the **Pugh criterion**:

- B/G > 1.75 → Ductile  
- B/G < 1.75 → Brittle  

---

## ⚙️ Methodology

The computational workflow follows:

1. Structure initialization from CIF files  
2. Convergence testing (k-points and plane-wave cutoff)  
3. Geometry optimization  
4. Equation of State fitting (Birch-Murnaghan) → Bulk modulus (B)  
5. Elastic constant calculation → Shear modulus (G)  
6. Evaluation of Pugh ratio (B/G)  

---

## 📊 Key Results

| Element | B (GPa) | G (GPa) | B/G | Behavior |
|--------|--------|--------|-----|----------|
| Li | ~13.8 | ~2.9 | ~4.7 | Ductile |
| Pt | ~249 | ~62 | ~4.0 | Ductile |
| Y | ~39 | ~23 | ~1.66 | Brittle |

---

## 🧠 Insights

- Li and Pt show strong ductility due to high B/G ratios  
- Y exhibits brittle behavior  
- Mechanical properties can be reliably predicted using DFT  
- The Pugh criterion serves as a simple but effective screening tool  

---

## 📁 Repository Contents

- `data/` → Convergence and elastic property datasets (Excel files)  
- `structures/` → Crystal structure file used in simulations  
- `inputs/` → Pseudopotential details  
- `figures/` → Generated plots (if available)  
- `report/` → Full project report  

---

## 📊 Available Data

This repository includes:

- Convergence analysis for Li, Pt, and Y  
- Shear modulus calculations for Li and Pt  
- Example structure file (Pt.cif)  
- Pseudopotential information used in simulations  

> Note: Full raw DFT input/output files are not included. The available data captures the essential workflow and results.

---

## 🚀 Future Work

- Extend analysis to alloys and multi-component systems  
- Automate workflow using Python  
- High-throughput screening of materials  
- Integration with materials databases  

---

## 📄 Report

Detailed methodology and results are available in:

`/report/Pugh_criterion.pdf`

---

## 👨‍💻 Author

Vishwas Subramanian
