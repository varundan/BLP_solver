# BLP_solver
Bi-level programming(BLP) framework used to observe a healthcare system subjected to a pandemic\\
Part of my Master's Degree at Oregon State University.

This framework is under active development. If you come across any bugs/errors or if you have any questions, feel free to contact me!

Packages required for running this framework - 
  1. SciPy
  2. NumPy
  3. Pandas
  4. SymPy
  5. itertools

A Bi-level optimization problem is solved using the 'double penalty approach' and built-in Python solvers. Also includes a preliminary convexity check for objective functions as well as several knobs to control model parameters. 
The case used to showcase the BLP is that of a healthcare system subjected to disease spread (COVID-19).
Within the bi-level framework,
the UPPER-LEVEL is a local population and a representative adminstrative body that is characterized by the SIR compartmental model of epidemiology.
the LOWER-LEVEL is a healthcare facility that controls staff parameters(no. of personnel, no. of hours and hourly wage) and personal protection equipment(PPE)(no. of PPE kits, cost of PPE kits) parameters.

The SIR model(leader) is made to react to an optimum decision made by the HCF(follower) in terms of PPE and staff quantity to disburse appropriate budget amount to combat disease spread within the population. 
