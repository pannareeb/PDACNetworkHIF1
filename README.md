# BMA-PDAC-Model

This is the repository of BMA .json files for boolean networks of Pancreatic ductal adenocarcinoma (PDAC) that includes pancreatic cancer cell (PCC) connected with pancreatic stellate cell (PSC) and macrophage (that receive the input from helpter T-cell) which share intercellular environment (to which substances are secreted and detected). 

The files include 

1. The final connected completely boolean networks
2. The final connected boolean networks with all phenotype nodes of PCC and PSC being set to range from 0-3

3. The final separate completely boolean models of PCC, PSC, macrophage, and small helper T-cell, each of which to be used as an input for the function in the file 4. to create the formatted inputs for the spatial model, based on the paper by Aguilar B et al. (2020) (https://academic.oup.com/gigascience/article/9/7/giaa075/5874689) with this Github (https://github.com/boaguilar/multicell_boolean_networks)

4. The R code to change BMA .json output to these three required inputs for the spatial model
  - counting the number of input variables for each node (nodes that point towards each node) in a network
  - collecting the identity (ID number) of input variables for each node in a network
  - creating the truth table of all possible permutations of the input variables for each node in a network 

5. The output of drugging tests (no drug, single HIF1A inhibition, and double HIF1A/HIF2A inhibition) from BMA in .csv file with 20 steps.
  - 5.1 the output when using the final connected completely boolean networks (file 1.)
  - 5.2 the output when usign the final connected boolean networks with all phenotype nodes of PCC and PSC being set to range from 0-3 (file 2.)
  
 