# Trees
## Properties of the tree

<table>
    <tr>
        <th>Trees</th>
        <th>m-ary</th>
        <th>full m-ary</th>
    </tr>
    <tr>
        <td colspan="3">|E| = n - 1</td>
    </tr>
    <tr>
        <td colspan="3">n = i + l</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>$$n=m*i+1$$</br>$$l=(m-1)*i+1$$</td>
    </tr>
</table>

**Height and Level**
- A rooted m-ary is balanced if all leaves are at levels h or h-1.
- $$l\le m^h -> h\ge\lceil\log_m(l)\rceil$$
## Prefix code
1. Find frequencies of each character
2. Constructing a rooted binary tree:
   - Sort by freq from small to large
   - The larger weight sub-tree is on the left of the binary tree
## Tree Traversal
1. Pre-Order: <span style="color:red;">N</span> -> L -> R
2. In-Order: L -> <span style="color:red;">N</span> -> R
3. Post-Order: R -> P -> <span style="color:red;">N</span>
## Representing the expression
1. *Prefix*: + x y
2. *Infix*: x + y
3. *Postfix*: x y +
## Spa. Tree
1. DFS - Depth-First Search (backtracking)
2. BFS - Breadth-First Search (level)
## Min. Spa. Tree
1. **Prim's Algorithm**:</br>
   Step 1: Choosing any smallest weight edge and putting it into the spanning tree.</br>
   Step 2: Repeatly - that are incident to a vertex already in tree, but never forming a simple circuit.</br>
   Step 3: When |E| = n-1, stop.</br>
2. **Kruskal's Algorithm**:</br>
   Step 1: Choose an edge with minimum weight.</br>
   Step 2: Add edges with minimum weight, but never forming a simple circuit.</br>
   Step 3: When |E| = 1, stop.</br>
