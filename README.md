# Circle Antipode Experiment Trajectory Dataset

## Overview

This repository provides trajectory datasets from the **Circle Antipode Experiment**, which explores pedestrian movement and behavior under various densities and radii. The data were extracted using [PeTrack](http://petrack.org) and can support research on pedestrian dynamics, simulation model validation, and related analyses.

## Dataset Structure

The compressed archive includes **4 × 8 groups of experiments**, comprising:

- **Radii:** 5m and 10m  
- **Participants per experiment:** 8, 16, 32, and 64  
- **Repetitions:** 4 for each setup  

This results in 8 unique experimental configurations (2 radii × 4 group sizes), each repeated 4 times.

*Refer to the actual archive for the precise organization.*

## Data Format

Each data file is in CSV format and includes the following fields:

| Column | Description                                   | Type    |
|--------|-----------------------------------------------|---------|
| id     | Unique individual identifier                  | Integer |
| t      | Time step (frame number or timestamp)         | Float   |
| x      | X coordinate (meters)                         | Float   |
| y      | Y coordinate (meters)                         | Float   |
| z      | Z coordinate (meters, typically 0 in 2D data) | Float   |

**Sample (first few rows):**

id, t, x, y, z

1, 0.00, 1.23, 2.34, 0.00

1, 0.04, 1.28, 2.39, 0.00

2, 0.00, -0.71, 0.89, 0.00

…

## Data Extraction

All trajectory data in this dataset were extracted using [PeTrack](http://petrack.org), a dedicated video tracking software for pedestrian experiments.

## Usage

This dataset is provided for non-commercial research, educational, or benchmarking purposes. Example use cases include:

- Analysis of pedestrian collective behavior
- Model validation and benchmarking
- Academic coursework and visualization

If you use this dataset for publications or presentations, please cite the related papers described below.

## Citation

Please cite both of the following papers if you use this dataset in your work:

1. Xiao, Y., Gao, Z., Jiang, R., Huang, Q. and Yang, H., 2021.  
   **Exploration of pedestrian side preference behavior with circle antipode experiments: analysis, simulation and implication.**  
   _Transportmetrica B: Transport Dynamics, 9(1), pp.266-282._  
   [https://doi.org/10.1080/21680566.2020.1838729](https://doi.org/10.1080/21680566.2020.1838729)

2. Xiao, Y., Gao, Z., Jiang, R., Li, X., Qu, Y. and Huang, Q., 2019.  
   **Investigation of pedestrian dynamics in circle antipode experiments: Analysis and model evaluation with macroscopic indexes.**  
   _Transportation Research Part C: Emerging Technologies, 103, pp.174-193._  
   [https://doi.org/10.1016/j.trc.2019.04.013](https://doi.org/10.1016/j.trc.2019.04.013)

**BibTeX entries:**
```bibtex
@article{xiao2021exploration,
  title={Exploration of pedestrian side preference behavior with circle antipode experiments: analysis, simulation and implication},
  author={Xiao, Y., Gao, Z., Jiang, R., Huang, Q. and Yang, H.},
  journal={Transportmetrica B: Transport Dynamics},
  volume={9},
  number={1},
  pages={266--282},
  year={2021}
}

@article{xiao2019investigation,
  title={Investigation of pedestrian dynamics in circle antipode experiments: Analysis and model evaluation with macroscopic indexes},
  author={Xiao, Y., Gao, Z., Jiang, R., Li, X., Qu, Y. and Huang, Q.},
  journal={Transportation Research Part C: Emerging Technologies},
  volume={103},
  pages={174--193},
  year={2019}
}


