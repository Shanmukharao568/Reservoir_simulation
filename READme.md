# Reservoir Simulation - Google Colab

## 📌 Project Title
**Reservoir Simulation using Finite Difference Method in Python (Google Colab Implementation)**

## 🧠 Project Overview

This project demonstrates a reservoir simulation model using the finite difference method to simulate single-phase flow in porous media. It is implemented in Python and run in a Google Colab environment for ease of access and reproducibility. The simulation provides insights into pressure behavior over time within a petroleum reservoir grid and can be used to understand fluid flow in subsurface formations.

## 📂 Project Structure

```
📁 Reservoir-Simulation-Colab/
│
├── reservoir_simulation.ipynb     # Main simulation notebook
├── input_parameters.csv           # Contains reservoir properties and simulation controls
├── README.md                      # Project documentation (this file)
└── output_graphs/                 # Plots of pressure maps and profiles
```

## 🛠 Features

- ✅ 1D/2D finite difference grid discretization
- ✅ Explicit and/or implicit time stepping
- ✅ Customizable grid size and simulation parameters
- ✅ Pressure evolution plots
- ✅ Google Colab compatibility for instant execution

## 🧪 Simulation Inputs

| Parameter            | Description                                  |
|----------------------|----------------------------------------------|
| Grid Dimensions      | Number of grid blocks in X (and Y) direction |
| Porosity             | Constant value per block                     |
| Permeability         | Uniform or variable                          |
| Viscosity            | Fluid viscosity (e.g., in cp)                |
| Initial Pressure     | Reservoir pressure before production starts  |
| Time Step            | ∆t for simulation                            |
| Total Time           | Total simulation period                      |
| Well Conditions      | Location and bottom-hole pressure (BHP)     |

## 📈 Outputs

- Pressure distribution as a 2D/3D plot
- Pressure profile vs time graphs
- CSV or JSON export of pressure data
- Well block pressure monitoring

## 📚 How to Run

### Option 1: Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the `reservoir_simulation.ipynb` file.
3. Execute each cell sequentially.
4. View outputs inline.

### Option 2: Local Jupyter Notebook

```bash
pip install numpy matplotlib pandas
jupyter notebook reservoir_simulation.ipynb
```

## 🔬 Theory and Background

This project applies **Darcy’s Law** and **mass conservation** to develop the governing equation for single-phase flow in porous media. The finite difference approximation is used to discretize the reservoir domain, leading to a linear system solved for pressure at each timestep.

**Equation used:**

\[
\frac{\partial P}{\partial t} = \frac{k}{\phi \mu c_t} \nabla^2 P
\]

Where:
- \( P \): Pressure
- \( k \): Permeability
- \( \phi \): Porosity
- \( \mu \): Viscosity
- \( c_t \): Total compressibility

## 📌 Applications

- Academic learning for reservoir simulation courses
- Benchmarking simple reservoir cases
- Foundation for machine learning datasets in reservoir engineering
- Extensible to multiphase or compositional modeling

## 🚀 Future Enhancements

- Add water/oil two-phase simulation
- Implement Crank-Nicolson method for better stability
- Interactive sliders in Colab for real-time parameter tuning
- Coupling with machine learning models for pressure prediction

## 👨‍💻 Developed With

- Python 3.8+
- Numpy
- Matplotlib
- Pandas
- Google Colab

## 📝 References

- Applications in Oil and Gas Industry (coursera) By L&T EduTech.
- SPE Petroleum Engineering Handbook
