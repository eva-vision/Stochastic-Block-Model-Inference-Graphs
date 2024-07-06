# Inference in Stochastic Block Model Graphs and in Real Social Network

## 1. Create a SBM model which generates a network with _(K, s, Pij)_ parameters.
## 2. Write a function which calculates the likelihood for any network given by the set of parameters _(K, s, Pij)_
## 3. We will try to inference back the parameters with which we created the network.
## 4. Do the simulated annealing, several time for a given _K_. The elementary step is that for fixed _K_ we move a node from a block _i_ to block _j_. If the likelihood increases accept the new configuration otherwise accept it with probability _p_=exp(−(log(_Lold_)−log(_Lnew_))/_T_)

![image](https://github.com/eva-vision/Stochastic-Block-Model-Inference-Graphs/assets/52841811/78d969ff-408b-4d85-ab85-dfb7b067ee6d)
Figure 1: Simulated Annealing

## 5. Do the above for different _K_ and plot the best log likelihood. Try to identify the best partition.
## 6. Plot the network for the best partition with different colors for different block (color the nodes: if _c_ is an integer array with the same length as number of nodes in the graph, then the following line does the trick, if you do not like to colors (you won't) then change the colormap):nx.draw(G,node_color=c)

