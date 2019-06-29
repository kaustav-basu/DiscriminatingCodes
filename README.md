# DiscriminatingCodes
CRITIS 2018 Code

dcilp.py computes the Minimum Discriminating Code Set (MDCS) for a given graph. The MDCS ensures that every node in one partition of the graph has unique identification. Check CRITIS 2018 paper for further details.

## Getting Started

dcilp.py requires graphs as input. There are a few example graphs provided from MATPOWER, under the folder Graphs.

### Prerequisites

Firstly, the user must have a solver installed on their system. My code uses Gurobi, but it can be changed to other solvers, depending on the the solver installed in the user's system. 

Secondly, the user must have the following packages installed:

```
1. pandas 0.23.4
2. networkx 2.1
3. pulp 1.6.8
4. numpy 1.15.1
```

### Testing

Type the following to execute the code:
```
python dcilp.py
```
The program asks for the input filetype (csv or txt). Once provided, the program executes and displays the following:
```
1. The value of the indicator variables (0/1)
2. The optimal objective function value
3. The total number of nodes in the one partition requiring unique monitoring in the graph
4. The total % savings 
5. The amount of time taken for the execution of the code
```
