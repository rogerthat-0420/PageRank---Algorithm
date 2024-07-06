# PageRank Algorithm

## Introduction
This project demonstrates the implementation of the PageRank algorithm using NetworkX and Matplotlib in Python. The PageRank algorithm is a popular ranking algorithm used by Google Search to rank web pages in their search engine results. This project includes the following key components:

1. Implementation of the PageRank algorithm.
2. Visualization of the graph with node sizes proportional to their PageRank scores.
3. Visualization of the changes in PageRank scores across iterations.
   
## PageRank Algorithm
The PageRank algorithm computes a ranking of the nodes in a directed graph based on the structure of the incoming links. The algorithm assigns a numerical weighting to each element, with the purpose of measuring its relative importance within the graph. The core idea is that a node is more important if it is linked to by other important nodes.

## Parameters
- graph: The input graph represented as a dictionary where keys are nodes and values are lists of neighboring nodes.
- alpha: The damping factor, usually set to 0.85.
- ax_iterations: The maximum number of iterations to perform.
- tol: The tolerance level to check convergence.

## Algorithm Steps
1. Initialize each node's score to 1 / number_of_nodes.
2. Iterate for a maximum of max_iterations or until convergence:
   - For each node, update its score based on the scores of its predecessors and their out-degrees.
   - Apply the damping factor and adjust the score with the teleportation probability.
   - Check for convergence by comparing the change in scores with tol.



|Rank | Node  |	PageRank Score |
|-----|-------|----------------|
| 1	  |  A	  |  0.27          |
| 2	  |  B	  |  0.24          |
| 3	  |  C	  |  0.15          |
| 4	  |  F	  |  0.11          |
| 5	  |  D	  |  0.11          |
| 6	  |  E	  |  0.09          |
| 7	  |  G	  |  0.04          |


<img width="844" alt="Screenshot 2024-07-07 at 1 52 35 AM" src="https://github.com/rogerthat-0420/PageRank-Algorithm/assets/140241681/a0400331-9aa4-4a67-a3a8-589763a225cc">

<img width="634" alt="Screenshot 2024-07-07 at 1 52 48 AM" src="https://github.com/rogerthat-0420/PageRank-Algorithm/assets/140241681/bbb9cafe-215e-40d2-89cc-93817eab9509">

## Conclusion
This project showcases the implementation of the PageRank algorithm, along with visualizations that help in understanding the distribution and convergence of scores. By analyzing the final rankings and the changes across iterations, one can gain insights into the relative importance of nodes in a directed graph.
