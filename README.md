# Garden Planting Plan Optimization

A collection of Jupyter notebooks and data files to model, solve, and visualize an optimal planting plan for a home garden using linear programming.

---

## 📋 Table of Contents

1. [Overview](#overview)
2. [Project Structure](#project-structure)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Data](#data)
7. [Notebooks](#notebooks)
8. [Presentation](#presentation)
9. [Contributing](#contributing)
10. [License](#license)

---

## Overview

Gardeners often need to decide how much area to allocate to each crop to maximize yield, respect rotations, and work within space and sunlight constraints.
This project demonstrates how to:

* Formulate a garden-layout problem as a linear program
* Solve with [IBM Decision Optimization CPLEX Modeling for Python (DOcplex)](https://github.com/IBMDecisionOptimization/docplex)
* Visualize the resulting planting plan and yield distributions

---

## Project Structure

```
.
├── garden_capstone_code.ipynb                  # Core LP model: data loading, problem formulation, solver
├── garden_optimization_with_visualization.ipynb# Full pipeline: optimization + plots
├── garden_with visualization.ipynb             # Additional visualization experiments
├── garden_capstone_data.xlsx                   # Input dataset: crop requirements & garden specs
├── Garden Planting Plan Optimization.pptx      # Slide deck summarizing methodology & results
└── README.md                                   # You are here
```

---

## Prerequisites

* **Python** ≥ 3.7
* **Jupyter Notebook** or **JupyterLab**
* **Python packages**:

  * `pandas`
  * `numpy`
  * `matplotlib`
  * `docplex`
  * `openpyxl`

---

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/tahidul94/Garden-Planting-Plan-Optimization.git
   cd Garden-Planting-Plan-Optimization
   ```

2. **(Optional) Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate      # Linux / macOS
   venv\Scripts\activate         # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install pandas numpy matplotlib docplex openpyxl jupyter
   ```

---

## Usage

1. Launch Jupyter:

   ```bash
   jupyter notebook
   ```
2. Open any `.ipynb` file to run the analyses.
3. Modify parameters in `garden_capstone_data.xlsx` (e.g., total area, crop yields) and rerun notebooks to see updated plans.

---

## Data

**`garden_capstone_data.xlsx`**

* Defines each crop’s space requirements, expected yield per unit area, and rotation compatibility
* Specifies total garden area and bed configurations

---

## Notebooks

* **`garden_capstone_code.ipynb`**: Build and solve the LP model, inspect raw outputs.
* **`garden_optimization_with_visualization.ipynb`**: Adds plotting of layout maps and yield bar charts.
* **`garden_with visualization.ipynb`**: Extra visualization experiments (heatmaps, density plots).

---

## Presentation

The **`Garden Planting Plan Optimization.pptx`** slide deck walks through motivation, methodology, results, and recommendations for next steps.

---

## Contributing

1. Fork the repo
2. Create a branch (`git checkout -b feature/YourFeature`)
3. Commit changes (`git commit -m "Add new feature"`)
4. Push (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## License

This project is released under the **MIT License**. See the [LICENSE](LICENSE) file for details.
