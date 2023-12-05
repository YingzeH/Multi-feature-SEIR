# Multi-feature-SEIR

Gurobi package is required to solve the optimization problem defined. For installation, please see: https://www.gurobi.com.

The SEIR simulation.ipynb:

(1) In the begining, it simulates the epidemic given fixed inputs. 

(2) Then, it defines the simulation process (SEIR_simulation function) via multi-feature SEIR model. Vaccination is also considered in the function. 

(3) The SEIR_simulation_greedy function applies to the vaccination strategy provided by gurobi solver. 

(4) Section III defines several vaccination strategies. Specifically, the "optimal_vaccination" function prioritizes vaccination by solving the optimization problem (minimizing the affected susceptible population).

(5) Section IV defines the output format. 

(6) Section V defines the simulation input parameters. 

(7) Section VI gives epidemic simulations with different vaccination strategies. 

(8) Section VII displays the results. 

(9) Section VIII compares the effect of changing population parameters under no vaccination.


The SEIR stochastic simulation.ipynb has the same sections as SEIR simulation.ipynb. It further defines a vaccination strategy considering uncertainty in estimation.

(1) Section II defines the pandemic simulation process using multi-feature SEIR model.

(2) Section III defines several vaccination strategies. Section 3.5 CCP optimization defines the chance-constraint version of the optimization (minimizing the affected susceptible population), allowing the uncertainty of change in the susceptible population.

(3) Section IV defines the output format for computation.

(4) Section V defines the simulation input parameters. 

(5) Section VI gives epidemic simulations with different vaccination strategies. 

(6) Section VII displays the results. 


The SEIR vs Real.ipynb compares the infection cases from the classic SEIR model, multi-feature SEIR model, and confirmed cases in Allegheny and Hamilton County in US. It uses the file "covid infection Allegheny County.xlsx" and "covid infection Hamilton County.xlsx" (confirmed cases) to check the performance of SEIR models. These two files are summarized from the file "covid_confirmed_usafacts.csv".

S1.File summarizes the performance (highest infection and cumulative death) for vaccination strategies in different situations (High-High, Low-High, High-Low, Low-Low). It can be produced by SEIR simulation.ipynb.
