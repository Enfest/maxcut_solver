# Novel Gradient-Descent Model for Max Cut Problem

This Jupyter Notebook demonstrates a novel approach to solving the Max Cut problem using a gradient-descent model. The Max Cut problem is a well-known problem in computer science and combinatorial optimization, where the goal is to partition the vertices of a graph into two subsets such that the number of edges between the subsets is maximized.

## Summary

The notebook is structured as follows:

1. **Library Imports**: Necessary libraries such as `numpy`, `time`, and `matplotlib` are imported for matrix operations, timing, and plotting, respectively.

2. **Data Loading and Initialization**: 
    - The adjacency matrix of the graph is loaded from a `.npy` file.
    - The matrix is processed to ensure all values are positive.
    - Row sums are calculated and used to normalize the adjacency matrix.
    - Initial codeword vector is set to ones.

3. **Visualization**:
    - The adjacency matrix is visualized using a heatmap to provide an initial understanding of the graph structure.

4. **Gradient-Descent Algorithm**:
    - Various parameters for the gradient-descent algorithm are initialized.
    - An annealing step function is defined to control the number of indices updated in each iteration.
    - The main loop of the gradient-descent algorithm iterates up to 2000 times, updating the adjacency matrix and codeword vector based on calculated gradients.
    - The satisfaction level of the current partition is calculated and tracked.
    - The algorithm includes mechanisms to escape local optima by flipping significant indices when the satisfaction level stagnates.

5. **Results**:
    - The final results, including the number of vertices, total iterations, maximum satisfaction level, and the best time to achieve this satisfaction, are printed.

This approach leverages gradient-descent techniques to iteratively improve the partitioning of the graph, aiming to maximize the cut value. The notebook provides a comprehensive workflow from data loading and preprocessing to algorithm implementation and result visualization.
