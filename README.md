# Multi-feature-SEIR

Gurobi package is required to some the optimization problem defined. For installation, please see: https://www.gurobi.com.

The SEIR simulation.ipynb simulates the epidemic given fixed inputs. It defines the simulation process (SEIR_simulation function) via multi-feauture SEIR model. The vaccination is also considered in the function. The SEIR_simulation_greedy function applies to the vaccination strategy provided by gurobi solver. Section III defines several vaccination strategies. Section IV defines the output format. Simulation input parameters are defined in section V.  Section VI gives epidemic simulations with different vaccination strategy. Section VII displays the results. Section VIII compares the effect of changing population parameters under no vaccination.

The SEIR stochastic simulation.ipynb. Each section does the same thing as SEIR simulation.ipynb.

The SEIR vs Real.ipynb compares the infection cases from classic SEIR model, multi-feature SEIR model, and confirmed cases in Allegheny county in US (covid_confirmed_usafacts.csv).
