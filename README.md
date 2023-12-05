# Multi-feature-SEIR

Gurobi package is required to some the optimization problem defined. For installation, please see: https://www.gurobi.com.

The SEIR simulation.ipynb:

(1) In the begining, it simulates the epidemic given fixed inputs. 

(2) Then, it defines the simulation process (SEIR_simulation function) via multi-feauture SEIR model. 

(3) The vaccination is also considered in the function. 

(4) The SEIR_simulation_greedy function applies to the vaccination strategy provided by gurobi solver. 

(5) Section III defines several vaccination strategies. Specicically, the "optimal_vaccination" function prioritize vaccination by solving the optimization problem.

(6) Section IV defines the output format. 

(7) Section V defines the simulation input parameters. 

(8) Section VI gives epidemic simulations with different vaccination strategy. 

(9) Section VII displays the results. Section VIII compares the effect of changing population parameters under no vaccination.


The SEIR stochastic simulation.ipynb has the same sections as SEIR simulation.ipynb.


The SEIR vs Real.ipynb compares the infection cases from classic SEIR model, multi-feature SEIR model, and confirmed cases in Allegheny and Hamilton county in US.
