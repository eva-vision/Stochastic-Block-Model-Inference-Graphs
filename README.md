# Inference in Stochastic Block Model Graphs and in Real Social Network

## 1. Create a SBM model which generates a network with (𝐾,𝑠𝑖,𝑃𝑖𝑗
) parameters.
## 2. Write a function which calculates the likelihood for any network given by the set of parameters (𝐾,𝑠,𝑃𝑖𝑗
)
## 3. We will try to inference back the parameters with which we created the network.
## 4. Do the simulated annealing, several time for a given 𝐾
. The elementary step is that for fixed 𝐾
 we move a node from a block 𝑖
 to block 𝑗
. If the likelihood increases accept the new configuration otherwise accept it with probability 𝑝=exp(−(log(𝐿𝑜𝑙𝑑)−log(𝐿𝑛𝑒𝑤))/𝑇)

![image](https://github.com/eva-vision/Stochastic-Block-Model-Inference-Graphs/assets/52841811/78d969ff-408b-4d85-ab85-dfb7b067ee6d)
Figure 1: Simulated Annealing

## 5. Do the above for different 𝐾
, and plot the best log likelihood as log−(𝐾−1)2
 vs. 𝐾
. Try to identify the best partition.
## 6. Plot the network for the best partition with different colors for different block (color the nodes: if 𝑐
 is an integer array with the same length as number of nodes in the graph, then the following line does the trick, if you do not like to colors (you won't) then change the colormap):
nx.draw(G,node_color=c)

