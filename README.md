# Efficiency-Aware Optimization of Wind-Powered Electrolyzer Operation

This repository contains a Python implementation of a mixed-integer linear programming (MILP) model for the optimal scheduling of a grid-connected, wind-powered alkaline electrolyzer with hydrogen storage.

The model incorporates power-dependent electrolyzer efficiency using piecewise-linear electrical loss curves while maintaining computational tractability for annual hourly simulations. It evaluates different operating strategies, including **ON/OFF** and **ON/OFF/STANDBY** modes, and considers minimum-load constraints, start-up costs, electricity market participation, and hydrogen storage dynamics.

## Features

- MILP-based electrolyzer scheduling using Gurobi
- Piecewise-linear approximation of electrolyzer losses
- ON/OFF and ON/OFF/STANDBY operating strategies
- Hydrogen storage modeling and terminal storage constraints
- Grid electricity import and export optimization
- Temperature sensitivity analysis
- Computational performance and convergence diagnostics
- Automated generation of result tables and figures

## Requirements

```bash
pip install pandas numpy matplotlib gurobipy
```

## Outputs

The model generates:

- Annual performance metrics (profit, hydrogen production, losses, grid imports/exports)
- Hourly operational schedules
- Computational performance tables
- Temperature sensitivity results
- Publication-quality comparison figures

## License

This project is provided for research and academic purposes.
