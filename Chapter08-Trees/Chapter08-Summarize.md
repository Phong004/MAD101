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
