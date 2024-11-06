```mermaid
graph TD
    Undirected graph --> Simple graph
    Undirected graph --> Multi-graph
    Multi-graph --> Allowed Multi-edge
    Undirected graph --> Pseudo-graph
    Pseudo-graph --> Allowed Multi-edge
    Pseudo-graph --> Allowed Loops
    Undirected graph --> Mixed graph
    Directed graph --> Simple graph
    Directed graph --> Directed Multi-graph
    Directed Multi-graph --> Allowed Multi-edge
    Directed Multi-graph --> Allowed Loops
    Directed graph --> Mixed graph
    Mixed graph --> Allowed Multi-edge
    Mixed graph --> Allowed Loops
```
