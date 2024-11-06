## Graph Terminology
```mermaid
graph TD
    A[Undirected graph] --> C[Simple graph]
    A[Undirected graph] --> D[Multi-graph]
    D[Multi-graph] --> G[Allowed Multi-edge]
    A[Undirected graph] --> E[Pseudo-graph]
    E[Pseudo-graph] --> G[Allowed Multi-edge]
    E[Pseudo-graph] --> H[Allowed Loops]
    A[Undirected graph] --> F[Mixed graph]
    B[Directed graph] --> C[Simple graph]
    B[Directed graph] --> I[Directed Multi-graph]
    I[Directed Multi-graph] --> G[Allowed Multi-edge]
    I[Directed Multi-graph] --> H[Allowed Loops]
    B[Directed graph] --> F[Mixed graph]
    F[Mixed graph] --> G[Allowed Multi-edge]
    F[Mixed graph] --> H[Allowed Loops]
```
## Types of graphs

| Graph | \|V\| | \|E\| | Degree |
|:---:  | :---: | :---: |---   |
|$$K_n, n \ge 1$$|n|$$\frac{n*(n-1)}{2}$$|deg(u) = n-1, $$\forall u \in V$$|
|$$K_{m, n} \ge 1$$|$$m+n$$|$$m*n$$|$$deg(u) = n, \forall u \in V_1; deg(v) = m, \forall v \in V_2$$|
|$$C_n, n \ge 3$$|n|n|deg(u) = 2, $$\forall u \in V$$|
|$$W_n, n \ge 3$$|$$n+1$$|n|$$deg(u) = 3, \forall u \in C_n; deg(*) = n$$|
|$$Q_n, n \ge 1$$|$$2^n$$|$$n*2^{n-1}$$|deg(u) = n|

## Bipartite graphs
- Make colors two adjacent edges differently colored.
## Representing graphs
1. Using adjacency list:
2. Using adjacency Matrix:
    - All this kind of matrix is square - symmetric, the values are not less than 0.
    - The main diagonal is the number of loops.
    - The degree of a vertex is determined by the sum of the row or column in matrix (the value of the main diagonal is doubled).
3. Using incidence matrix:
    - The column is the sequence of the vertices, and the row is the sequence of the edges.
    - The entry $$m_{i,j} = 1$$ where $$v_i$$ is a node of $$e_j$$
    - The size of the matrix: |v|.|e|
    - $$m_{i,j} \in {0,1}$$

|$$e_1$$|$$e_2$$|$$e_{...}$$|$$e_i$$|
|-------|:-----:|:---------:|:-----:|
|$$v_1$$| - | - | - |
|$$v_2$$| - | - | - |
|$$v_{...}$$| - | - | - |
|$$v_j$$| - | - | - |

