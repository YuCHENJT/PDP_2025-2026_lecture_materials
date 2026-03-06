# PDP 2025–2026 Lecture Materials

📧 Contact: [Yu Chen](mailto:Yu.Chen@lshtm.ac.uk 
)

This repository contains lecture materials for the **[Population Dynamics and Projections (PDP) 2025–2026] (https://ble.lshtm.ac.uk/course/view.php?id=5646)**, covering topics in kinship demography, orphanhood estimation and decomposition methods.

---

## 📂 Repository Structure

```
PDP_2025-2026_lecture_materials/
├── Kinship demography/
│   ├── Lecture notes/         
│   └── R lab/
│       └── Kinship-demography-practical_yc.html  
└── Decomposition method/
    ├── Lecture notes/          
    └── R lab/                  
```

---

## 📖 Topics

### 1. Kinship Demography
📅 *Lecture date: 06 Mar 2026*

An introduction to kinship demography and orphanhood estimation method, with an advanced topic on inequality analysis.

**R Lab contents:**
- Installing and loading [`DemoKin`](https://github.com/IvanWilli/DemoKin) and related packages (`dplyr`, `tidyr`, `ggplot2`)
- Loading Swedish mortality (survival probabilities) and fertility (age-specific fertility rates) data
- Fitting a **time-invariant kinship model** for Sweden
- Visualising the **kinship network** — expected number of living kin for a focal individual at a given age
- Plotting **age profiles of living kins** across the life course for selected kin types (mother, daughter, grandmother, granddaughter, sisters, aunts, nieces, cousins, etc.)

**Key R packages:**
| Package | Purpose |
|---------|---------|
| `DemoKin` | Kinship matrix model |
| `dplyr` | Data manipulation |
| `tidyr` | Data reshaping |
| `ggplot2` | Visualisation |

> 📌 Lecture notes and additional materials will be available after class.

### 2. Decomposition Techniques
📅 *Lecture date: 12 Mar 2026*

*(Materials coming soon)*

---

## 🚀 Getting Started

1. Clone this repository.
2. Open the `.Rmd` file in RStudio.
3. Install dependencies:
   ```r
   install.packages("devtools")
   devtools::install_github("IvanWilli/DemoKin")
   install.packages(c("dplyr", "tidyr", "ggplot2"))
   ```
4. Knit the `.Rmd` to reproduce the HTML output.



