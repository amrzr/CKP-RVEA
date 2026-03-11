# Handling simulation failures of a computationally expensive multiobjective optimization problem in pump design

This repository contains the implementation for the paper [Handling simulation failures of a computationally expensive multiobjective optimization problem in pump design](https://www.sciencedirect.com/science/article/pii/S0952197624010558) (Engineering Applications of Artificial Intelligence,
Volume 136, Part A,2024). We consider data-driven multiobjective optimization of the diffusor of an axial pump and propose an approach to reduce the number of solutions that fail in expensive computational fluid dynamics simulations. The proposed approach utilizes Kriging surrogate models to approximate the objective functions and is inexpensive to evaluate. We utilize a probabilistic selection approach with constraints in a multiobjective evolutionary algorithm to find solutions with better objective function values, lower uncertainty, and lower probability of failing.

### Data and Results
* Results of the experiments can be found in the `primer_opt_results` folder.
* The dataset used for the tests is provided in the `primer_data` folder.

### Clone Repository
`gh repo clone amrzr/MOPrimer_Interactiv](https://github.com/amrzr/CKP-RVEA.git`

### Requirements:
* The project relies on the desdeo-emo, desdeo-tools, and desdeo-problems packages for the optimization algorithm used and defining the optimization problem.
* Python 3.7 or up

### Offline Optimization of Pump Design
To run the non-interactive version:
```
python main_project_files/Start_pump_opt.py
```
Set `is_interact=True` to execute the interactive version.
