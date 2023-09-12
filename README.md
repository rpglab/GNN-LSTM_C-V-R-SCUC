## Spatio-tempoeral GNN-LSTM model for constraint and variable reduced-SCUC (C-V-R-SCUC)
This program implements our TPWRS paper "Spatio-Temporal Deep Learning-Assisted Reduced Security-Constrained Unit Commitment".

This set of codes implements our TPWRS paper "Spatio-Temporal Deep Learning-Assisted Reduced Security-Constrained Unit Commitment". LSTM-GNN is used to reduce variables and constraints for SCUC; warm-start is enabled for remaining variables.

The detailed data and generated graph samples can be found at the following link:
https://figshare.com/articles/dataset/Spatio-Temporal_Deep_Learning-Assisted_Reduced_Security-Constrained_Unit_Commitment/24116394


## Overview:
A spatio-temporal (ST) machine learning (ML) model for security-constrained unit commitment (SCUC) solution acceleration. The ML architecture with GNN and LSTM layers. Includes two models, one for node prediction to predict generator commitment status, and another for edge prediction, which predicts congested lines in the system. The predictions from the two models are then used to reduce the number of variables and constraints in a SCUC problem.


## Python Environment:
Codes are implemented in Python. ML model uses Keras, Tensorflow and Spektral (GNN) libraries. Optimization is implemented using Pyomo in python. A solver license (cplex/gurobi) is required for pyomo to run.


## Test Power Systems
There are four test power systems used in this work:
1. IEEE 24-bus system: one area of the IEEE 73-bus system.
2. IEEE 73-bus system: the original data of this test system are described in this reference: "The IEEE Reliability Test System-1996. A report prepared by the Reliability Test System Task Force of the Application of Probability Methods Subcommittee" and link is <a class="" target="_blank" href="https://ieeexplore.ieee.org/document/780914">here</a>.
3. IEEE 118-bus system: the original data of this test case are from the link below (in IEEE Common Data Format (ieee118cdf.txt)): https://labs.ece.uw.edu/pstca/pf118/ieee118cdf.txt
4. South-Carolina (SC) synthetic 500-bus system: the original data of this test system are from https://electricgrids.engr.tamu.edu/electric-grid-test-cases/activsg500/


## Citation:
If you use any of our codes/data for your work, please cite the following papers as your reference:

Arun Venkatesh Ramesh and Xingpeng Li, “Spatio-Temporal Deep Learning-Assisted Reduced Security-Constrained Unit Commitment”, *IEEE Transactions on Power Systems*, Sep. 2023. 

(DOI: 10.1109/TPWRS.2023.3313430)

Paper website: https://rpglab.github.io/papers/ArunR_ST-C-V_R-SCUC/


## Contributions:
Arun Venkatesh Ramesh developed this set of programs/data. Xingpeng Li supervised this work.


## Contact:
Dr. Xingpeng Li

University of Houston

Email: xli83@central.uh.edu

Website: https://rpglab.github.io/


## License:
This work is licensed under the terms of the <a class="off" href="https://creativecommons.org/licenses/by/4.0/"  target="_blank">Creative Commons Attribution 4.0 (CC BY 4.0) license.</a>


## Disclaimer:
The author doesn’t make any warranty for the accuracy, completeness, or usefulness of any information disclosed; and the author assumes no liability or responsibility for any errors or omissions for the information (data/code/results etc) disclosed.