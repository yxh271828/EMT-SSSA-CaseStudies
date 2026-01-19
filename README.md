# EMT-SSSA Case Studies
This repository provides the case studies used in the paper for EMT-based small-signal stability analysis (SSSA).
All cases are implemented in DIgSILENT PowerFactory 2022.
The system models are provided in .pfd format and can be directly opened for EMT simulation.

## Case A: Motivating Example
The converter delivers 0.6 MW active power and 0 MVar reactive power to the grid. The power system parameters are shown in the following. The transmission line is modelled using both lumped- or distributed- parameter model. The converter is modeled using an average value model and operates under a grid-following (GFL) control strategy, which consists of an outer loop power control and inner loop current control. A phase-locked loop (PLL) is employed to maintain synchronization with the grid.

| Category | Parameter | Value | Unit |
|:-----:|:-----|:-----:|:-----:|
| 数据1 | Resistance per unit length | 数据3 | 数据3 |
| 数据4 | Reactance per unit length | 数据6 | 数据3 |
| 数据1 | Capacitance per unit length | 数据3 | 数据3 |
| 数据4 | Line length | 数据6 | 数据3 |
| 数据4 | Rated voltage | 数据6 | 数据3 |
