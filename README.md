# CS5073 - ANNE Final Project Source Code

## About

This is the source code for the ANNE final project for Zak Kastl. This source is located in a single jupyter notebook file that peforms all tasks related to the project. This source defines the functions for:
- Generating the random linear equations required for the test data.
- Defining the grammar the grammatical evolution uses to produce the programs.
- Evaluating the individual for a fitness score.
- Reduceing the output of the linear equations produced by the GE technique into the 'mx+b' format for comparision. Raw outputs can look something like X+x-2+10-x-x-x....

The next section sets up both experiments and generates the results graphs too. Before any experiments are run, the code generates 100 test equations of the format 'mx+b'. And generates an initial population of examples used in both approaches. The code also set up 10 experiments (defined in code) that:
- Runs the GE approach for 1000 generations.
- Determines the fitness in each generation
- Evolves and performs crossover after each fitness evaluation.
- Generates a new model for the ANN approach
- Evaluates the model over 1000 epochs.
- Stores the results (in terms of how many found solutions) as separate lists.

Finally, the code plots the results of the 10 experimetns in a graph comparing the number of solutions found for each experiment. A note: the results are stochastic, and so running the code may produce slightly different results than presented in the paper. 

## Assumptions

This code was bult and run originally using Tensorflow 2.15. Changes to Tensorflow, especially to 2.16 may not work. (I've seen a fair few amount of changes in these versions.)

Zak Kastl