## Graph Terminology
```mermaid
graph TD
    A[Undirected graph] --> D[Multi-graph]
    A[Undirected graph] --> E[Pseudo-graph]
    D[Multi-graph] --> G[Allowed Multi-edge]
    E[Pseudo-graph] --> G[Allowed Multi-edge]
    F[Mixed graph] --> G[Allowed Multi-edge]
    I[Directed Multi-graph] --> G[Allowed Multi-edge]
    E[Pseudo-graph] --> H[Allowed Loops]
    F[Mixed graph] --> H[Allowed Loops]
    I[Directed Multi-graph] --> H[Allowed Loops]
    A[Undirected graph] --> F[Mixed graph]
    A[Undirected graph] --> C[Simple graph]
    B[Directed graph] --> C[Simple graph]
    B[Directed graph] --> I[Directed Multi-graph]
    B[Directed graph] --> F[Mixed graph]
```
## Types of graphs

<table>
    <tr>
        <th>Graph</th>
        <th>|V|</th>
        <th>|E|</th>
        <th>Degree</th>
    </tr>
    <tr>
        <th>$$K_n, n \ge 1$$</th>
        <td>n</td>
        <td>$$\frac{n*(n-1)}{2}$$</td>
        <td>deg(u) = n-1, $$\forall u \in V$$</td>
    </tr>
    <tr>
        <th>$$K_{m, n} \ge 1$$</th>
        <td>$$m+n$$</td>
        <td>$$m*n$$</td>
        <td>$$deg(u) = n, \forall u \in V_1$$</br>$$deg(v) = m, \forall v \in V_2$$</td>
    </tr>
    <tr>
        <th>$$C_n, n \ge 3$$</th>
        <td>n</td>
        <td>n</td>
        <td>deg(u) = 2, $$\forall u \in V$$</td>
    </tr>
    <tr>
        <th>$$W_n, n \ge 3$$</th>
        <td>$$n+1$$</td>
        <td>n</td>
        <td>$$deg(u) = 3, \forall u \in C_n$$</br>$$deg(*) = n$$</td>
    </tr>
    <tr>
        <th>$$Q_n, n \ge 1$$</th>
        <td>$$2^n$$</td>
        <td>$$n*2^{n-1}$$</td>
        <td>deg(u) = n</td>
    </tr>
</table>

## Bipartite graphs
- Make colors two adjacent edges differently colored.
## Representing graphs
1. Using adjacency list:
2. Using adjacency Matrix:
    - All this kind of matrix is square - symmetric, the values are not less than 0.
    - The main diagonal is the number of loops.
    - The degree of a vertex is determined by the sum of the row or column in matrix (the value of the main diagonal is doubled).

    |     |$v_1$|$v_2$|$v_{...}$|$v_n$|
    |:---:|:---:|:---:|:---:|:---:|
    |$v_1$|-|-|-|-|
    |$v_2$|-|-|-|-|
    |$v_{...}$|-|-|-|-|
    |$v_n$|-|-|-|-|

3. Using incidence matrix:
    - The column is the sequence of the vertices, and the row is the sequence of the edges.
    - The entry $$m_{i,j} = 1$$ where $$v_i$$ is a node of $$e_j$$
    - The size of the matrix: |v|.|e|
    - $$m_{i,j} \in {0,1}$$

    |       |$$e_1$$|$$e_2$$|$$e_{...}$$|$$e_m$$|
    |:-----:|:-----:|:-----:|:---------:|:-----:|
    |$$v_1$$| - | - | - | - |
    |$$v_2$$| - | - | - | - |
    |$$v_{...}$$| - | - | - | - |
    |$$v_n$$| - | - | - | - |

## Isormophism of graphs
- There exists a bijection f from $$V_1$$ to $$V_2$$ and vice versa -> They are same the number of vertices, number of edges, degree.
- If the sphere discards a point, it is isormophic with the flat.
  *The way to identify*:
  1. Check whether they are same number of edges, number of vertices, the sequence of degree.
  2. If true, check whether adjacent vertices are same.
## Connectedness
1. Undirected graph:
    - There exists a path between the distinct vertices of the graph.
2. Directed graph:
    - **Strongly connected**: there is a path from a to b and vice versa whenever a and b are vertices of the graph.
    - **Weekly connected**: there is always a path between 2 vertices when the directions of the edges are disregraded.
## Counting paths between vertices
- Let A is a *adjacency matrix*, the number of different paths of **length r** from $v_i$ to $v_j$ **equals to the $$(i, j)_r$$ entry of $$A^{r}$$** ($$r \gt 0$$).
## Cut vertex & Cut edge
- Its removal will produce disconnected subgraphs from original connected graph.
## Euler paths and circuit (|V| $$\ge$$ 2)

|     | Path | Circuit |
|-----|:---:|:---:|
|Condition| No odd degree | Exactly 2 vertices of odd degree |

## Hamilton paths and circuits
G is a simple graph with n $$\ge$$ 3 vertices

|**Name**| **Theorem**  |
|:-----:|-----------------------------------------
|Dirac  |$$\forall v_i, deg(v_i) \ge \frac{n}{2}$$|
|Ore|$$\forall u, \forall v, non-adjacent, deg(u) + deg(v) \ge n$$|

## Dijkstra's algorithm

***[SEE HERE](ch07-graph.md)***
