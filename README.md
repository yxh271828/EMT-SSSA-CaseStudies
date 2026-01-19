# EMT-SSSA Case Studies
This repository provides the case studies used in the paper for EMT-based small-signal stability analysis (SSSA).
All cases are implemented in DIgSILENT PowerFactory 2022.
The system models are provided in .pfd format and can be directly opened for EMT simulation.

## Case A: Motivating Example
The converter delivers 0.6 MW active power and 0 MVar reactive power to the grid. The power system parameters are shown in the following. The transmission line is modelled using both lumped- or distributed- parameter model. The converter is modeled using an average value model and operates under a grid-following (GFL) control strategy, which consists of an outer loop power control and inner loop current control. A phase-locked loop (PLL) is employed to maintain synchronization with the grid.

| Category | Parameter | Value | Unit |
|:-----:|:-----|:-----:|:-----:|
| Line | Resistance per unit length | 0.025547 | Ohm/km |
|  | Reactance per unit length | 0.3 | Ohm/km |
|  | Capacitance per unit length | 3.599926 | μF/km |
|  | Line length | 150 | km |
|  | Rated voltage | 30 | kV |
| Transformer | Short-circuit voltage | 6 | kW |
|  | Copper loss | 2.799611 | kW |
|  | Rated power | 2.8 | MVA |
|  | Rated power | 30 | kV |
|  | High-voltage side rated voltage | 1.5 | kV |
| Outer loop power control | Active power proportional gain | 3 |  |
|  | Active power integral gain | 0.8 |  |
|  | Reactive power proportional gain | 2 |  |
|  | Reactive power integral gain | 0.5 |  |
| Inner loop current control | d-axis proportional gain | 1 |  |
|  | d-axis integral gain | 500 |  |
|  | q-axis proportional gain | 0.5 |  |
|  | q-axis integral gain | 313 |  |
| PLL | Proportional gain | 5 |  |
|  | Integral gain | 300 |  |
| Filter | Inductance | 0.5 | mH |
| Converter | Rated Power | 2.778 | MVA |

## Case B: A Practical EMT Study of a Regional Power Grid
The case is based on a real regional power grid in China, which has been desensitized for confidentiality. The system consists of 42 buses, including 1 equivalent external grid, 1 thermal power plant, and 9 wind power plants, with renewable generation contributing more than 50% of the total power output. It contains 27 transmission lines and 22 trans-formers, with voltage levels ranging from 0.8 kV, 35 kV, 220 kV up to 525 kV. The detailed system configuration and parameters are provided in the corresponding .pfd file.
