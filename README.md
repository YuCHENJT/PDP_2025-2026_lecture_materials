# PDP 2025–2026 Lecture Materials

📧 Contact: [Yu Chen](mailto:Yu.Chen@lshtm.ac.uk)

This repository contains lecture materials for the **[Population Dynamics and Projections (PDP) 2025–2026](https://ble.lshtm.ac.uk/course/view.php?id=5646)**, covering topics in kinship demography, orphanhood estimation and decomposition methods.

Lecture notes and R labs are also available on the module page.

> 💬 If you spot any errors in the slides or R labs, or have any questions or comments, please feel free to contact me. I hope you enjoy the lectures and have fun with the code! 😊

---

## 📂 Repository Structure

```
PDP_2025-2026_lecture_materials/
├── Kinship demography/
│   ├── Lecture notes/
│   │   ├── kinship-demography.pdf
│   │   └── orphanhood-inequality.pdf
│   └── R-lab/
│       └── Kinship-demography-practical_yc.html
└── Decomposition method/
    ├── Lecture notes/
    │   ├── stepwise-replacement.pdf
    │   └── stepwise_replacement_algorithm_dashboard.html
    └── R-lab/
        ├── Decomposition-CoD.html
        ├── Functions_5.R
        └── Decomp_Data_L4.RData
```

---

## 📖 Topics

### 1. Kinship Demography
📅 *Lecture date: 06 Mar 2026*

An introduction to kinship demography and orphanhood estimation method, with an advanced topic on inequality analysis.

**Lecture slides:**
- `kinship-demography.pdf` — Introduction to kinship demography and orphanhood estimation
- `orphanhood-inequality.pdf` — Advanced topic: inequality analysis

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

### 2. Decomposition Techniques
📅 *Lecture date: 12 Mar 2026*

An introduction to decomposition methods in demography, covering the Horiuchi (linear integral) decomposition and the stepwise replacement method, with applications to life expectancy and lifespan variation.

**Lecture slides:**
- `stepwise-replacement.pdf` — Stepwise replacement decomposition method
- `stepwise_replacement_algorithm_dashboard.html` — Interactive algorithm walkthrough

**R Lab contents:**
- Applying the **Horiuchi et al. (2008)** linear integral decomposition and **Andreev et al. (2002)** stepwise replacement method
- Decomposing changes in **life expectancy** (e₀) between 1996 and 2013 for Venezuelan males by age and **cause of death (CoD)**
- Comparing results from both decomposition methods side by side
- Extending the analysis to **lifespan variation** (standard deviation of age at death)

**Key R packages:**
| Package | Purpose |
|---------|---------|
| `DemoDecomp` | Horiuchi & stepwise replacement decomposition |
| `dplyr` / `tidyr` / `tidyverse` | Data manipulation and reshaping |
| `ggplot2` | Visualisation |
| `ggpubr` | Combining multiple plots |

---

## 🚀 Getting Started

1. Clone this repository.
2. Open RStudio and create your own `.Rmd` file — feel free to experiment and enjoy the coding journey! 🎉
3. Install dependencies:

   **Kinship Demography:**
   ```r
   install.packages("devtools")
   devtools::install_github("IvanWilli/DemoKin")
   install.packages(c("dplyr", "tidyr", "ggplot2"))
   ```

   **Decomposition Techniques:**
   ```r
   install.packages(c("DemoDecomp", "tidyr", "ggplot2", "ggpubr"))
   ```

4. Refer to the HTML outputs in the `R-lab/` folders to check your results.



